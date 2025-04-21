# Architecture Haiku: Sistema de Pagamentos

## Contexto em Haiku

```
Dinheiro flui já
Gateway guarda o caminho
Kafka observa
```

## Decisões Arquiteturais Essenciais

### Padrão de API
- REST/HTTP para sincronismo
- Kafka para eventos assíncronos
- Circuit Breaker em integrações

### Persistência
- PostgreSQL para ACID
- Eventos para audit log
- Cache distribuído (Redis)

### Segurança
- OAuth2 + JWT
- TLS em todas conexões
- Secrets em Vault

## Trade-offs Principais

1. **Consistência vs Disponibilidade**
   - Escolha: Consistência para saldos
   - Motivo: Requisito regulatório

2. **Acoplamento vs Autonomia**
   - Escolha: Serviços autônomos
   - Custo: Duplicação controlada

3. **Performance vs Complexidade**
   - Escolha: Cache distribuído
   - Impacto: Mais infraestrutura

## Métricas Chave

- Latência < 500ms (P95)
- Disponibilidade 99.95%
- Recovery Point 0 (saldos)
- Recovery Time < 5min 