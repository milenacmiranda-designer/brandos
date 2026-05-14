# BrandOS — Workflow Completo (14 Fases)

Este é o workflow mestre do BrandOS. O `brandos-core` usa este documento como referência para conduzir o pipeline.

```txt
contexto → investigação → interpretação → hipóteses → memória →
estratégia → identidade → validação → exportação → produção opcional → evolução contínua
```

---

## Mapa do pipeline

```txt
01 Welcome / Onboarding        ┐
02 Discovery Inicial           │ DESCOBERTA
03 Materiais da Marca          │
04 Competitive Discovery       │
05 Research Flow               │
06 Audience Discovery          ┘
07 Strategy Flow               ┐ ESTRATÉGIA
08 Brand DNA  ◆ gate           ┘
09 Verbal Identity             ┐ IDENTIDADE
10 Visual Identity             │
11 UX + Product Experience     ┘
12 Governance + QA  ◆ gate     ┐ VALIDAÇÃO + ENTREGA
13 Export System  ★ fecha P1   ┘
14 Production System  (opcional)
```

---

## Detalhamento das fases

| # | Fase | Agente | Depende de | Tipo | Saída principal |
|---|------|--------|-----------|------|-----------------|
| 1 | Welcome / Onboarding | `onboarding-agent` | — | Sempre | caminho de onboarding |
| 2 | Discovery Inicial | `discovery-agent` | 1 | Sempre | `02-discovery.md` |
| 3 | Materiais da Marca | `brand-context-agent` | 1 | Condicional¹ | `03-brand-context.md` |
| 4 | Competitive Discovery | `competitive-research-agent` | 2 | Sempre | parte de `04-competitive-research.md` |
| 5 | Research Flow | `competitive-research-agent` | 4 | Sempre | `04-competitive-research.md` |
| 6 | Audience Discovery | `audience-intelligence-agent` | 2 | Sempre | `05-audience.md` |
| 7 | Strategy Flow | `strategy-agent` | 2,4,5,6 | Sempre | `06-strategy.md` |
| 8 | Brand DNA | `brand-dna-agent` | 7 | **Gate** | `brand-dna.json` + `07-brand-dna.md` |
| 9 | Verbal Identity | `verbal-identity-agent` | 8 | Sempre | `08-verbal-identity.md` |
| 10 | Visual Identity | `visual-identity-agent` | 8 | Sempre | `09-visual-identity.md` |
| 11 | UX + Product Experience | `ux-product-experience-agent` | 8,9,10 | Condicional² | `10-ux-product-experience.md` |
| 12 | Governance + QA | `governance-qa-agent` | 9,10,11 | **Gate** | `11-governance-qa.md` |
| 13 | Export System | `export-agent` | 12 | **Fecha Parte 1** | `brand-system.md` + PDF |
| 14 | Production System | `production-agent` | 13 | **Opcional** | `03-production/` |

¹ Fase 3 roda nos caminhos `has-references` e `existing-brand`. No caminho `from-scratch`, é pulada.
² Fase 11 roda quando a marca tem ou terá produto digital.

---

## Os três caminhos de onboarding

```txt
from-scratch     →  1 → 2 → 4 → 5 → 6 → 7 → 8 → 9 → 10 → (11) → 12 → 13 → (14)
has-references   →  1 → 3 → 2 → 4 → 5 → 6 → 7 → 8 → 9 → 10 → (11) → 12 → 13 → (14)
existing-brand   →  1 → 3* → 2 → 4 → 5 → 6 → 7 → 8 → 9 → 10 → (11) → 12 → 13 → (14)
                    (3* = modo diagnóstico + reposicionamento)
```

---

## Gates

Um gate **bloqueia** o avanço do pipeline até ser aprovado.

- **Fase 8 — Brand DNA:** o `brand-dna.json` precisa estar completo (sem campos vazios) e validado pelo usuário. É a fonte da verdade para tudo que vem depois.
- **Fase 12 — Governance + QA:** score ≥ 70. Abaixo disso, o pipeline volta para revisão das fases com problema. Conflito de severidade ALTA não documentado também bloqueia.

---

## Regras de orquestração

1. Atualizar a memória ao fim de **cada** fase.
2. Ler a memória relevante **antes** de invocar cada agente.
3. Apresentar hipóteses e validar com o usuário antes de fechar fases importantes (2, 7, 8, 10).
4. Nada genérico passa — output genérico volta para revisão.
5. O usuário pode voltar a qualquer fase; mudanças propagam para a memória e para as fases dependentes.
6. Fase 13 fecha a Parte 1. A fase 14 só começa depois do export completo.

---

## Memória — arquivos e responsáveis

| Arquivo | Escrito por | Contém |
|---------|-------------|--------|
| `brand-dna.json` | fase 8 (lido por 9-14) | fonte única da verdade |
| `strategic-memory.json` | fases 2,3,5,7 | hipóteses, posicionamento, gaps, territórios |
| `creative-memory.json` | fases 3,9,10,11 | padrões visuais, sistema verbal e visual |
| `audience-memory.json` | fase 6 | público, dores, desejos, emoções |
| `decision-memory.json` | fases 7,8,12 | decisões aprovadas e descartadas |
| `conversation-memory.json` | fases 1,2 | onboarding, confirmações do usuário |
| `production-memory.json` | fase 14 | materiais produzidos |
| `campaign-memory.json` | fase 14 | campanhas geradas |

---

## Estrutura de saída no projeto do usuário

```txt
brandos-output/
├── memory/                    ← 8 arquivos JSON de memória
├── 01-brand-system/           ← documentos .md das fases 2-12
├── 02-pdf/                    ← brand-system.md + brand-guidelines.pdf
├── 03-production/             ← materiais do Production System
└── 04-assets/                 ← JPEG final e referências
```
