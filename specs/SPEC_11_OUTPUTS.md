# SPEC_11_OUTPUTS — Entregáveis

## Objetivo

Definir quais entregáveis o BrandOS pode gerar, em que formato e em que ordem.

## Estrutura de saída recomendada

```txt
brandos-output/
├── memory/
│   ├── brand-dna.json
│   ├── strategic-memory.json
│   ├── creative-memory.json
│   ├── audience-memory.json
│   ├── decision-memory.json
│   ├── conversation-memory.json
│   ├── production-memory.json
│   └── campaign-memory.json
├── 01-brand-system/
│   ├── 01-overview.md
│   ├── 02-discovery.md
│   ├── 03-brand-context.md
│   ├── 04-competitive-research.md
│   ├── 05-audience.md
│   ├── 06-strategy.md
│   ├── 07-brand-dna.md
│   ├── 08-verbal-identity.md
│   ├── 09-visual-identity.md
│   ├── 10-ux-product-experience.md
│   ├── 11-governance-qa.md
│   └── brand-system.md
├── 02-pdf/
│   └── brand-guidelines.pdf
├── 03-production/
│   ├── social-posts.md
│   ├── landing-page-copy.md
│   ├── prompt-visual.md
│   └── campaign-ideas.md
└── 04-assets/
    └── README.md
```

## Entregáveis principais (obrigatórios)

| Arquivo | Conteúdo | Gerado na fase |
|---------|----------|----------------|
| `02-discovery.md` | Briefing estruturado | Fase 2 |
| `03-brand-context.md` | Auditoria de materiais | Fase 3 (condicional) |
| `04-competitive-research.md` | Pesquisa de mercado | Fase 4–5 |
| `05-audience.md` | Público e personas | Fase 6 |
| `06-strategy.md` | Posicionamento e proposta | Fase 7 |
| `07-brand-dna.md` | Brand DNA consolidado | Fase 8 (gate) |
| `08-verbal-identity.md` | Identidade verbal completa | Fase 9 |
| `09-visual-identity.md` | Direção visual conceitual | Fase 10 |
| `11-governance-qa.md` | Scorecard de qualidade | Fase 12 (gate) |
| `brand-system.md` | Brand book completo | Fase 13 |

## Entregáveis opcionais

- `10-ux-product-experience.md` — fase condicional para produto digital
- `social-posts.md` — posts para redes sociais
- `landing-page-copy.md` — copy para landing page
- `prompt-visual.md` — prompts para geração de imagens
- `campaign-ideas.md` — ideias de campanha

## Entregáveis adicionais via Production System

- calendário de conteúdo
- bio para Instagram e LinkedIn
- pitch comercial
- apresentação institucional
- roteiro de vídeo
- guia de campanha
- plano de lançamento
- naming (quando necessário)
- tagline
- manifesto expandido
- guia de aplicação em materiais físicos

## Critérios de qualidade dos outputs

Os outputs devem ser:

- claros e organizados
- com nomes padronizados e numerados
- úteis para consulta imediata
- compatíveis entre si (sem contradições)
- prontos para uso sem edição adicional
- nomeados corretamente (sem espaços, em kebab-case)

## Regras de nomenclatura

- Usar kebab-case: `verbal-identity.md`
- Usar prefixo numérico: `08-verbal-identity.md`
- Sem espaços ou caracteres especiais
- Sem abreviações ambíguas
- Incluir nome da marca quando há múltiplas marcas

## Agente responsável

`export-agent` (organização e geração) + `production-agent` (materiais opcionais)
