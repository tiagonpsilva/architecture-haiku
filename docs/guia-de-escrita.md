# Guia para Escrever Architecture Haikus

## Princípios Fundamentais

### 1. Minimalismo com Propósito
- Cada palavra deve ter valor
- Elimine redundâncias
- Foque no essencial

### 2. Estrutura Clara

Como um haiku tradicional japonês (5-7-5), um Architecture Haiku deve ter uma estrutura clara:

1. **Contexto** (O quê?)
   - Propósito do sistema
   - Stakeholders principais
   - Restrições críticas

2. **Decisões** (Como?)
   - Escolhas arquiteturais chave
   - Padrões utilizados
   - Tecnologias core

3. **Consequências** (Por quê?)
   - Trade-offs principais
   - Impactos esperados
   - Métricas de sucesso

## Técnicas de Escrita

### Usando Haikus Reais

Um haiku arquitetural pode começar com um haiku real que capture a essência do sistema:

```
API responde
Microserviços dançam
Cache acelera
```

### Seções Essenciais

1. **Visão Geral**
   - Um parágrafo
   - Máximo 50 palavras
   - Foco no valor

2. **Decisões Chave**
   - 3-5 pontos principais
   - Formato bullet point
   - Justificativa concisa

3. **Trade-offs**
   - Máximo 3 trade-offs
   - Formato "Se X, então Y"
   - Impacto claro

### Diagramas C4

- Contexto: Uma página
- Contêineres: Uma página
- Componentes: Seletivo
- Código: Apenas crítico

## Anti-Padrões

❌ **Evite**:
- Detalhes de implementação
- Decisões óbvias
- Documentação extensa
- Diagramas complexos

✅ **Prefira**:
- Decisões impactantes
- Trade-offs não óbvios
- Diagramas claros
- Métricas objetivas

## Exemplo de Estrutura

```markdown
# [Nome do Sistema] Architecture Haiku

## Haiku
[Haiku capturando essência]

## Contexto
[Um parágrafo conciso]

## Decisões Chave
- Decisão 1: Razão
- Decisão 2: Razão
- Decisão 3: Razão

## Trade-offs
1. Escolha A > B porque X
2. Sacrificou X para ganhar Y

## Métricas
- Métrica 1: Alvo
- Métrica 2: Alvo
```

## Dicas Finais

1. **Revise e Refine**
   - Primeira versão: Capture tudo
   - Segunda versão: Elimine 50%
   - Versão final: Refine linguagem

2. **Mantenha Vivo**
   - Revise periodicamente
   - Atualize quando necessário
   - Valide com stakeholders

3. **Compartilhe**
   - Torne acessível
   - Colete feedback
   - Itere com equipe 