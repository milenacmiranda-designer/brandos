# SPEC_00_OVERVIEW — Visão Geral do Sistema

## Objetivo

Explicar a lógica geral do BrandOS e como todas as partes se conectam.

## Entrada necessária

- PRD do BrandOS
- lista de workflows
- lista de agentes
- lista de skills
- estrutura de outputs

## Processo

Esta Spec deve organizar:

1. a visão geral do sistema
2. a relação entre PRD, Specs e Scaffold
3. a relação entre agentes e workflows
4. a relação entre skills e entregas
5. as regras globais de funcionamento
6. o padrão de qualidade esperado

## Saída esperada

Uma visão geral clara da arquitetura do BrandOS.

## Critérios de qualidade

A visão geral deve ser:

- fácil de entender
- organizada
- completa
- compatível com o uso no Claude Code
- útil para orientar futuras alterações

## Relação entre componentes

```txt
PRD
↓
Specs
↓
Scaffold
↓
Agents (14 agentes principais)
↓
Subagents (9 especialistas)
↓
Skills (11 habilidades reutilizáveis)
↓
Workflows (6 fluxos)
↓
Templates
↓
Outputs
↓
Review
```

## Pipeline de 14 fases

```txt
DESCOBERTA
 01  Welcome / Onboarding
 02  Discovery Inicial
 03  Materiais da Marca (condicional)
 04  Competitive Discovery
 05  Research Flow
 06  Audience Discovery

ESTRATÉGIA
 07  Strategy Flow
 08  Brand DNA ◆gate

IDENTIDADE
 09  Verbal Identity
 10  Visual Identity
 11  UX + Product Experience (condicional)

VALIDAÇÃO + ENTREGA
 12  Governance + QA ◆gate
 13  Export System ★
 14  Production System (condicional)
```

## Regras globais

1. Nenhum agente trabalha de forma isolada
2. Todo agente consulta PRD + Spec + Workflow + Templates + Harness
3. Gates obrigatórios bloqueiam avanço até aprovação
4. Memória persistente mantém consistência entre fases
5. Linguagem sempre adaptada ao nível do usuário
