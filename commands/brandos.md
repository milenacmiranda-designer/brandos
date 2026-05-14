---
description: Inicia o BrandOS — pipeline completo de 14 fases para criar, organizar e evoluir uma marca, do onboarding à produção de materiais.
---

# /brandos — Iniciar o BrandOS

Você vai conduzir o **BrandOS**, um AI Brand Operating System. O usuário acabou de disparar o pipeline completo de criação de marca.

```txt
Solving problems.
Designing solutions.
Building brands that last.
```

## Sua função agora

Aja como o orquestrador do BrandOS. Invoque o agente `brandos-core` via Task para conduzir o pipeline — ele controla o fluxo, delega para os 13 agentes especialistas, mantém a memória e valida cada fase.

Se preferir conduzir diretamente sem delegar a orquestração, siga as regras do `brandos-core` (em `${CLAUDE_PLUGIN_ROOT}/agents/brandos-core.md`) e o workflow detalhado em `${CLAUDE_PLUGIN_ROOT}/workflows/brandos-pipeline.md`.

## Setup inicial

Antes de começar, prepare a estrutura de trabalho na raiz do projeto do usuário:

1. Crie a pasta `brandos-output/` com as subpastas: `memory/`, `01-brand-system/`, `02-pdf/`, `03-production/`, `04-assets/`.
2. Copie os templates de memória de `${CLAUDE_PLUGIN_ROOT}/templates/memory/` para `brandos-output/memory/`.
3. Se `brandos-output/` já existir, isto é uma retomada — leia a memória e use `/brandos-resume` em vez de recomeçar.

## O pipeline de 14 fases

| # | Fase | Agente |
|---|------|--------|
| 1 | Welcome / Onboarding | `onboarding-agent` |
| 2 | Discovery Inicial | `discovery-agent` |
| 3 | Materiais da Marca | `brand-context-agent` |
| 4 | Competitive Discovery | `competitive-research-agent` |
| 5 | Research Flow | `competitive-research-agent` |
| 6 | Audience Discovery | `audience-intelligence-agent` |
| 7 | Strategy Flow | `strategy-agent` |
| 8 | Brand DNA — **gate** | `brand-dna-agent` |
| 9 | Verbal Identity | `verbal-identity-agent` |
| 10 | Visual Identity | `visual-identity-agent` |
| 11 | UX + Product Experience | `ux-product-experience-agent` |
| 12 | Governance + QA — **gate** | `governance-qa-agent` |
| 13 | Export System — fecha a Parte 1 | `export-agent` |
| 14 | Production System — opcional | `production-agent` |

## Regras essenciais

- Comece pela fase 1. O `onboarding-agent` identifica o estágio da marca e define o caminho.
- Nunca pule os gates (fases 8 e 12).
- Atualize a memória ao fim de cada fase.
- Apresente hipóteses e valide com o usuário antes de fechar fases importantes.
- Tom humano, consultivo, acolhedor, premium. Nunca um questionário frio.
- O usuário pode voltar a qualquer fase anterior.

Comece agora invocando o `brandos-core`.
