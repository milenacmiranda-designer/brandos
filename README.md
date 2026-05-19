# BrandOS — AI Brand Operating System

```txt
Solving problems.
Designing solutions.
Building brands that last.
```

> Um plugin para Claude Code que transforma uma ideia em uma marca completa — e mantém essa marca viva.

O BrandOS não é um gerador de brandbook. É um **sistema operacional de marca**: ele entende a marca, investiga o mercado, interpreta materiais existentes, estrutura posicionamento, cria identidade verbal e visual, valida consistência, exporta a documentação final e ainda produz materiais reais. Tudo com memória persistente — ele lembra das decisões e evolui a marca continuamente.

---

## Instalação

No Claude Code:

```txt
/plugin marketplace add milenacmiranda-desinger/brandos
/plugin install brandos
```

Ou, para instalar localmente a partir desta pasta:

```txt
/plugin marketplace add ./caminho/para/brandos
/plugin install brandos
```

---

## Como usar

| Comando | O que faz |
|---------|-----------|
| `/brandos` | Inicia o pipeline completo de 14 fases |
| `/brandos-status` | Mostra em que fase a marca está e o que falta |
| `/brandos-resume` | Retoma de onde parou, carregando a memória |
| `/brandos-produce` | Vai direto ao Production System (marca já pronta) |

Comece com `/brandos`. O sistema pergunta em qual estágio você está e conduz o resto.

---

## O pipeline de 14 fases

```txt
DESCOBERTA
 01  Welcome / Onboarding        identifica o estágio da marca
 02  Discovery Inicial           conversa adaptativa sobre a ideia
 03  Materiais da Marca          analisa links e arquivos existentes
 04  Competitive Discovery       entende a concorrência
 05  Research Flow               pesquisa ativa de mercado
 06  Audience Discovery          mapeia público, dores e desejos

ESTRATÉGIA
 07  Strategy Flow               posicionamento, arquétipo, valores
 08  Brand DNA            ◆gate  consolida a fonte única da verdade

IDENTIDADE
 09  Verbal Identity             tom de voz, manifesto, mensagens
 10  Visual Identity             paleta, tipografia, direção visual
 11  UX + Product Experience     a marca dentro de produtos digitais

VALIDAÇÃO + ENTREGA
 12  Governance + QA      ◆gate  valida consistência — score /100
 13  Export System        ★      brand-system.md + PDF editorial A4
 14  Production System    (opcional)  packs e materiais reais
```

Os **gates** (fases 8 e 12) bloqueiam o avanço até serem aprovados — nada incoerente passa.

---

## Os 14 agentes

| Agente | Papel |
|--------|-------|
| `brandos-core` | Orquestrador — comanda o pipeline e a memória |
| `onboarding-agent` | Boas-vindas e identificação do estágio da marca |
| `discovery-agent` | Discovery conversacional e adaptativo |
| `brand-context-agent` | Análise de materiais existentes (links e arquivos) |
| `competitive-research-agent` | Concorrência, gaps e territórios livres |
| `audience-intelligence-agent` | Público, dores, desejos, emoções |
| `strategy-agent` | Posicionamento, arquétipo, diferenciação, valores |
| `brand-dna-agent` | Consolida o Brand DNA — a fonte da verdade |
| `verbal-identity-agent` | Tom de voz, manifesto, tagline, mensagens |
| `visual-identity-agent` | Paleta, tipografia, moodboard, sistema visual |
| `ux-product-experience-agent` | Experiência da marca em produtos digitais |
| `governance-qa-agent` | Validação de consistência — score e gate |
| `export-agent` | Exportação final — MD + PDF editorial |
| `production-agent` | Production System — packs e itens |

---

## O que o BrandOS entrega

No projeto onde você roda o `/brandos`, ele cria:

```txt
brandos-output/
├── memory/                ← 8 arquivos de memória persistente
├── 01-brand-system/       ← documentos de cada fase
├── 02-pdf/                ← brand-system.md + brand-guidelines.pdf
├── 03-production/         ← materiais do Production System
└── 04-assets/             ← referências e arquivos
```

---

## O que torna o BrandOS diferente

- **Memória interpretada** — não guarda histórico, guarda significado. Lembra das decisões e evolui a marca.
- **Brand DNA** — uma fonte única da verdade (`brand-dna.json`) de onde tudo deriva. Sem isso, cada fase puxaria para um lado.
- **3 caminhos de entrada** — funciona se você tem só uma ideia, se tem referências, ou se já tem uma marca para reposicionar.
- **Conversa, não questionário** — perguntas leves, exemplos de apoio, profundidade adaptativa.
- **Gates de qualidade** — nada incoerente ou genérico chega à exportação.
- **Continua depois da entrega** — o Production System transforma a marca em materiais reais.

---

## Estrutura do plugin

```txt
brandos/
├── .claude-plugin/
│   ├── plugin.json              ← manifesto do plugin
│   └── marketplace.json         ← catálogo para distribuição
├── agents/                      ← os 14 agentes principais
├── subagents/                   ← 9 especialistas pontuais
│   ├── naming-subagent.md
│   ├── tagline-subagent.md
│   ├── competitor-analysis-subagent.md
│   ├── audience-insight-subagent.md
│   ├── tone-of-voice-subagent.md
│   ├── manifesto-subagent.md
│   ├── color-palette-subagent.md
│   ├── typography-subagent.md
│   └── visual-references-subagent.md
├── skills/                      ← 11 habilidades reutilizáveis
│   ├── skill-briefing-analysis.md
│   ├── skill-brand-audit.md
│   ├── skill-market-research.md
│   ├── skill-persona-generation.md
│   ├── skill-positioning.md
│   ├── skill-value-proposition.md
│   ├── skill-brand-personality.md
│   ├── skill-verbal-identity.md
│   ├── skill-visual-direction.md
│   ├── skill-brandbook-generation.md
│   └── skill-quality-review.md
├── specs/                       ← especificações de cada etapa
│   ├── SPEC_00_OVERVIEW.md
│   ├── SPEC_01_BRIEFING.md
│   ├── SPEC_02_BRAND_AUDIT.md
│   ├── SPEC_03_RESEARCH.md
│   ├── SPEC_04_PERSONAS.md
│   ├── SPEC_05_POSITIONING.md
│   ├── SPEC_06_VALUE_PROPOSITION.md
│   ├── SPEC_07_BRAND_PERSONALITY.md
│   ├── SPEC_08_VERBAL_IDENTITY.md
│   ├── SPEC_09_VISUAL_IDENTITY.md
│   ├── SPEC_10_BRAND_BOOK.md
│   ├── SPEC_11_OUTPUTS.md
│   ├── SPEC_12_REVIEW.md
│   └── SPEC_13_EXPORT.md
├── commands/                    ← /brandos e comandos auxiliares
├── workflows/
│   └── brandos-pipeline.md      ← o workflow mestre de 14 fases
├── prompts/                     ← prompts-base por agente
│   ├── system-prompt.md
│   ├── onboarding-prompt.md
│   ├── briefing-prompt.md
│   ├── audit-prompt.md
│   ├── research-prompt.md
│   ├── strategy-prompt.md
│   ├── verbal-prompt.md
│   ├── visual-prompt.md
│   ├── review-prompt.md
│   └── export-prompt.md
├── templates/
│   └── memory/                  ← templates dos 8 arquivos de memória
├── docs/                        ← documentação complementar
│   ├── overview.md
│   ├── glossary.md
│   ├── usage-guide.md
│   └── concepts.md
├── examples/                    ← exemplos de uso por tipo de projeto
│   ├── example-new-brand.md
│   ├── example-rebrand.md
│   ├── example-personal-brand.md
│   └── example-digital-product.md
├── tests/                       ← casos de teste e validação
│   ├── test-new-brand.md
│   ├── test-rebrand.md
│   ├── test-personal-brand.md
│   ├── test-digital-product.md
│   └── test-quality-review.md
├── outputs/                     ← entregáveis gerados pelo BrandOS
│   └── README.md
├── PRD.md                       ← product requirements document
├── BRANDOS_HARNESS.md           ← harness de auditoria e QA
├── LICENSE
└── README.md
```

---

## Requisitos

- Claude Code com suporte a plugins
- Para a fase 5 (Research Flow): acesso à web
- Para a fase 14 com entrega integrada: MCPs de Canva/Figma/Adobe (opcional — sem eles, o BrandOS entrega arquivos + briefing editável)

---

*BrandOS v1.0 — De uma ideia a uma marca que dura.*
