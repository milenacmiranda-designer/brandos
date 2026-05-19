# Guia de Uso — BrandOS

Como usar o BrandOS no Claude Code.

---

## Início rápido

```
/brandos
```

Isso inicia o pipeline completo. O sistema vai:
1. Receber você no Onboarding
2. Entender o estágio da sua marca
3. Adaptar a experiência ao seu nível
4. Conduzir o processo fase a fase

---

## Comandos disponíveis

| Comando | Quando usar |
|---------|-------------|
| `/brandos` | Primeira vez ou novo projeto |
| `/brandos-status` | Ver em que fase está e o que falta |
| `/brandos-resume` | Continuar de onde parou |
| `/brandos-produce` | Gerar materiais extras (posts, copy, campanhas) |

---

## Os 3 caminhos de entrada

O BrandOS se adapta ao estágio da sua marca:

**1. Só tenho uma ideia**
O sistema conduz Discovery completo, pesquisa, estratégia e criação do zero.

**2. Tenho uma marca mas quero organizar**
O sistema faz auditoria, preserva o que funciona e estrutura o que falta.

**3. Quero redesign ou reposicionamento**
O sistema analisa a marca atual, diagnostica e cria nova estratégia.

---

## O que o BrandOS entrega

```txt
brandos-output/
├── memory/                  ← 8 arquivos de memória persistente
├── 01-brand-system/         ← documentos de cada fase
│   └── brand-system.md      ← brand book completo
├── 02-pdf/                  ← brand-guidelines.pdf
├── 03-production/           ← materiais do Production System
└── 04-assets/               ← referências e arquivos
```

---

## Como funciona a memória

O BrandOS salva progresso automaticamente. Se você precisar parar, use `/brandos-resume` para continuar exatamente de onde parou.

A memória fica em `brandos-output/memory/` e contém 8 arquivos:
- `brand-dna.json` — essência da marca
- `strategic-memory.json` — decisões estratégicas
- `creative-memory.json` — direção criativa
- `audience-memory.json` — público e personas
- `decision-memory.json` — decisões aprovadas
- `conversation-memory.json` — histórico resumido
- `production-memory.json` — materiais produzidos
- `campaign-memory.json` — campanhas e desdobramentos

---

## Os gates de qualidade

**Gate 8 — Brand DNA**
Nada avança sem estratégia aprovada. O sistema vai apresentar a base estratégica e pedir sua validação.

**Gate 12 — Governance + QA**
Nada é exportado sem revisão de qualidade. O sistema gera um scorecard antes de liberar o brand book.

---

## Perguntas frequentes

**Posso interromper e continuar depois?**
Sim. Use `/brandos-resume` para retomar de onde parou.

**O BrandOS cria logotipos?**
Não diretamente. Ele cria direção visual conceitual e prompts para geradores de imagem, Canva e Figma.

**Preciso responder tudo de uma vez?**
Não. O sistema faz perguntas em blocos pequenos e avança progressivamente.

**E se eu não souber responder alguma coisa?**
Diga que não sabe. O BrandOS vai ajudar com exemplos ou inferir com transparência.

**O BrandOS pesquisa na internet?**
Na fase 5 (Research Flow), se tiver acesso à web configurado, sim.
