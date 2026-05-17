---
description: Executa auditoria estrutural do BrandOS, validando arquivos, agentes, comandos, templates, workflows, riscos e score de integridade do projeto.
---

# /brandos-harness — Auditoria e QA estrutural do BrandOS

Você vai executar o **BrandOS Harness**, uma camada de auditoria, validação e controle de qualidade do projeto BrandOS.

Este comando não cria uma marca para o usuário.  
Este comando verifica se o **sistema BrandOS** está completo, consistente e pronto para rodar dentro do Claude Code.

```txt
Audit the system.
Find the gaps.
Protect the brand engine.
```

---

## Objetivo do comando

Quando o usuário rodar:

```bash
/brandos-harness
```

ou:

```bash
/brandos-harness audit
```

você deve verificar a estrutura do projeto BrandOS e gerar um relatório claro, simples e acionável.

A auditoria deve responder:

1. O projeto tem os arquivos obrigatórios?
2. O projeto tem os agentes esperados?
3. O projeto tem os comandos principais?
4. O projeto tem os templates de memória?
5. O pipeline principal existe?
6. Há riscos estruturais?
7. O sistema está pronto para uso?
8. O que precisa ser corrigido?

---

## Linguagem da resposta

Use linguagem clara, amigável e simples.

Explique como se estivesse ajudando uma pessoa que está aprendendo a organizar um plugin no Claude Code.

Evite linguagem técnica demais sem explicar.

Sempre que usar um termo técnico, explique de forma rápida.

Exemplo:

```md
O arquivo existe, mas ainda falta transformar essa parte em comando operacional.
Isso significa que a ideia está documentada, mas ainda não roda sozinha.
```

---

## Modos disponíveis

O comando pode aceitar estes modos:

```bash
/brandos-harness audit
/brandos-harness agent-check
/brandos-harness command-check
/brandos-harness memory-check
/brandos-harness workflow-check
/brandos-harness qa
/brandos-harness score
/brandos-harness repair-plan
```

Se o usuário rodar apenas:

```bash
/brandos-harness
```

execute o modo padrão:

```bash
/brandos-harness audit
```

---

# 1. Modo padrão: /brandos-harness audit

## Função

Executar uma auditoria completa da estrutura do BrandOS.

## O que verificar

Verifique se existem estes arquivos e pastas obrigatórios:

```txt
.claude-plugin/plugin.json
.claude-plugin/marketplace.json
README.md
LICENSE
BRANDOS_HARNESS.md
agents/
commands/
workflows/brandos-pipeline.md
templates/memory/
```

Depois, conte e valide:

```txt
14 agentes esperados
4 comandos principais esperados
8 templates de memória esperados
1 workflow principal esperado
```

---

## Checklist obrigatório

### Arquivos de plugin

Verifique:

```txt
.claude-plugin/plugin.json
.claude-plugin/marketplace.json
```

Critérios:

- Os arquivos existem?
- Estão dentro da pasta `.claude-plugin/`?
- Parecem compatíveis com um plugin Claude Code?

---

### Arquivos raiz

Verifique:

```txt
README.md
LICENSE
BRANDOS_HARNESS.md
```

Critérios:

- O `README.md` explica o projeto?
- O `LICENSE` existe?
- O `BRANDOS_HARNESS.md` existe como documentação de auditoria?

---

### Pasta de agentes

Verifique se a pasta existe:

```txt
agents/
```

E se contém os 14 agentes esperados:

```txt
agents/audience-intelligence-agent.md
agents/brand-context-agent.md
agents/brand-dna-agent.md
agents/brandos-core.md
agents/competitive-research-agent.md
agents/discovery-agent.md
agents/export-agent.md
agents/governance-qa-agent.md
agents/onboarding-agent.md
agents/production-agent.md
agents/strategy-agent.md
agents/ux-product-experience-agent.md
agents/verbal-identity-agent.md
agents/visual-identity-agent.md
```

Critérios:

- Existem 14 agentes?
- Os nomes estão corretos?
- Existe um agente orquestrador chamado `brandos-core.md`?
- Existe um agente de QA/governança chamado `governance-qa-agent.md`?
- Existe um agente de exportação chamado `export-agent.md`?
- Existe um agente de produção chamado `production-agent.md`?

---

### Pasta de comandos

Verifique se a pasta existe:

```txt
commands/
```

E se contém os comandos principais:

```txt
commands/brandos.md
commands/brandos-produce.md
commands/brandos-resume.md
commands/brandos-status.md
```

Além disso, verifique se este novo comando existe:

```txt
commands/brandos-harness.md
```

Critérios:

- Existem os 4 comandos principais?
- Existe o comando de auditoria `brandos-harness.md`?
- Os comandos possuem frontmatter com `description`?
- Os comandos explicam claramente quando devem ser usados?

Observação importante:

Se `commands/brandos-harness.md` não existir, marque como alerta médio ou alto, porque a auditoria está documentada, mas ainda não virou comando operacional.

---

### Pasta de workflows

Verifique se existe:

```txt
workflows/brandos-pipeline.md
```

Critérios:

- O workflow principal existe?
- Ele descreve as 14 fases?
- Ele indica agentes responsáveis por fase?
- Ele respeita os gates obrigatórios?

Gates esperados:

```txt
Fase 8 — Brand DNA
Fase 12 — Governance + QA
```

---

### Templates de memória

Verifique se a pasta existe:

```txt
templates/memory/
```

E se contém os 8 templates esperados:

```txt
templates/memory/audience-memory.json
templates/memory/brand-dna.json
templates/memory/campaign-memory.json
templates/memory/conversation-memory.json
templates/memory/creative-memory.json
templates/memory/decision-memory.json
templates/memory/production-memory.json
templates/memory/strategic-memory.json
```

Critérios:

- Existem 8 templates?
- Os arquivos estão em `.json`?
- A memória cobre estratégia, audiência, criatividade, decisões, produção e conversa?

---

# 2. Modo: /brandos-harness agent-check

## Função

Verificar somente os agentes do projeto.

## O que responder

Retorne:

```md
# Auditoria de Agentes BrandOS

## Agentes encontrados
- ✅ agente encontrado
- ❌ agente ausente

## Total
Encontrados: X/14

## Avaliação
Explique se a camada de agentes está completa ou incompleta.

## Recomendações
Liste o que precisa ser criado, renomeado ou revisado.
```

## Critérios adicionais

Verifique se o projeto tem agentes cobrindo estas áreas:

```txt
Onboarding
Discovery
Contexto de marca
Pesquisa competitiva
Inteligência de audiência
Estratégia
DNA de marca
Identidade verbal
Identidade visual
UX e produto
Governança e QA
Exportação
Produção
Orquestração central
```

Se uma área estiver faltando, sinalize.

---

# 3. Modo: /brandos-harness command-check

## Função

Verificar somente os comandos do projeto.

## Comandos esperados

```txt
commands/brandos.md
commands/brandos-produce.md
commands/brandos-resume.md
commands/brandos-status.md
commands/brandos-harness.md
```

## O que responder

```md
# Auditoria de Comandos BrandOS

## Comandos encontrados
- ✅ /brandos
- ✅ /brandos-produce
- ✅ /brandos-resume
- ✅ /brandos-status
- ✅ /brandos-harness

## Comandos ausentes
Liste aqui.

## Avaliação
Explique se o usuário consegue iniciar, produzir, retomar, consultar status e auditar o sistema.
```

---

# 4. Modo: /brandos-harness memory-check

## Função

Verificar somente os templates de memória.

## Templates esperados

```txt
audience-memory.json
brand-dna.json
campaign-memory.json
conversation-memory.json
creative-memory.json
decision-memory.json
production-memory.json
strategic-memory.json
```

## O que responder

```md
# Auditoria de Memória BrandOS

## Templates encontrados
- ✅ arquivo encontrado
- ❌ arquivo ausente

## Total
Encontrados: X/8

## Avaliação
Explique se o sistema tem memória suficiente para salvar progresso, decisões e entregas.
```

---

# 5. Modo: /brandos-harness workflow-check

## Função

Verificar somente o pipeline principal.

## Arquivo esperado

```txt
workflows/brandos-pipeline.md
```

## Verificar se o workflow possui

```txt
14 fases
Agente responsável por fase
Gates de validação
Fluxo de início
Fluxo de retomada
Fluxo de exportação
Fluxo de produção opcional
```

## Fases esperadas

```txt
1. Welcome / Onboarding
2. Discovery Inicial
3. Materiais da Marca
4. Competitive Discovery
5. Research Flow
6. Audience Discovery
7. Strategy Flow
8. Brand DNA
9. Verbal Identity
10. Visual Identity
11. UX + Product Experience
12. Governance + QA
13. Export System
14. Production System
```

## O que responder

```md
# Auditoria de Workflow BrandOS

## Workflow principal
✅ Encontrado ou ❌ Ausente

## Fases identificadas
Liste as fases encontradas.

## Fases ausentes
Liste as fases ausentes.

## Gates
Verifique se as fases 8 e 12 aparecem como pontos de validação.

## Avaliação
Explique se o pipeline está completo.
```

---

# 6. Modo: /brandos-harness qa

## Função

Fazer uma leitura crítica do projeto.

Aqui, não basta contar arquivos. Avalie se a estrutura faz sentido.

## Verificar riscos

Classifique riscos em:

```txt
Baixo
Médio
Alto
Crítico
```

## Exemplos de riscos

### Risco baixo

```txt
README poderia explicar melhor como instalar.
```

### Risco médio

```txt
Existe documentação de auditoria, mas não existe comando de auditoria.
```

### Risco alto

```txt
Faltam agentes essenciais para o pipeline.
```

### Risco crítico

```txt
Falta o plugin.json ou o workflow principal.
```

## O que responder

```md
# QA Estrutural BrandOS

## Riscos encontrados
| Risco | Gravidade | Impacto | Correção recomendada |
|---|---|---|---|

## Pontos fortes
Liste o que está bem estruturado.

## Pontos frágeis
Liste o que precisa de atenção.

## Recomendação final
Explique o próximo passo ideal.
```

---

# 7. Modo: /brandos-harness score

## Função

Gerar uma nota de integridade do projeto.

## Pontuação

Use uma escala de 0 a 100.

Distribuição sugerida:

```txt
Arquivos de plugin: 15 pontos
Arquivos raiz: 10 pontos
Agentes: 25 pontos
Comandos: 15 pontos
Workflow: 15 pontos
Templates de memória: 15 pontos
Clareza geral: 5 pontos
```

## Interpretação

```txt
90–100: Excelente — pronto para uso
75–89: Bom — pequenos ajustes necessários
60–74: Regular — precisa de correções importantes
40–59: Frágil — estrutura incompleta
0–39: Crítico — não recomendado rodar ainda
```

## O que responder

```md
# Score de Integridade BrandOS

## Nota final
XX/100

## Classificação
Excelente / Bom / Regular / Frágil / Crítico

## Pontuação por categoria
| Categoria | Pontos | Status |
|---|---:|---|

## Resumo
Explique em linguagem simples o que essa nota significa.
```

---

# 8. Modo: /brandos-harness repair-plan

## Função

Gerar um plano de correção para deixar o BrandOS mais completo.

## O que responder

```md
# Plano de Correção BrandOS

## Prioridade 1 — Corrigir primeiro
Liste problemas críticos ou altos.

## Prioridade 2 — Melhorar depois
Liste problemas médios.

## Prioridade 3 — Refinar
Liste melhorias pequenas.

## Arquivos a criar
Liste arquivos que precisam ser criados.

## Arquivos a revisar
Liste arquivos que precisam ser revisados.

## Próximo comando recomendado
Diga qual comando o usuário deve rodar depois.
```

---

# Formato obrigatório da resposta da auditoria completa

Quando executar `/brandos-harness audit`, responda sempre neste formato:

```md
# Auditoria BrandOS

## 1. Status geral
Explique em 2 ou 3 linhas se o projeto está completo, quase completo ou incompleto.

## 2. Checklist de arquivos obrigatórios
| Item | Status | Observação |
|---|---|---|
| .claude-plugin/plugin.json | ✅ / ❌ | ... |
| .claude-plugin/marketplace.json | ✅ / ❌ | ... |
| README.md | ✅ / ❌ | ... |
| LICENSE | ✅ / ❌ | ... |
| BRANDOS_HARNESS.md | ✅ / ❌ | ... |
| agents/ | ✅ / ❌ | ... |
| commands/ | ✅ / ❌ | ... |
| workflows/brandos-pipeline.md | ✅ / ❌ | ... |
| templates/memory/ | ✅ / ❌ | ... |

## 3. Agentes
Encontrados: X/14

### Agentes encontrados
Liste os agentes encontrados.

### Agentes ausentes
Liste os agentes ausentes.

## 4. Comandos
Encontrados: X/5

### Comandos encontrados
Liste os comandos encontrados.

### Comandos ausentes
Liste os comandos ausentes.

## 5. Templates de memória
Encontrados: X/8

### Templates encontrados
Liste os templates encontrados.

### Templates ausentes
Liste os templates ausentes.

## 6. Workflow
Diga se o workflow principal existe e se parece completo.

## 7. Riscos
| Risco | Gravidade | Como corrigir |
|---|---|---|

## 8. Score de integridade
XX/100

## 9. Diagnóstico simples
Explique de forma fácil o que está acontecendo.

Exemplo:
O projeto está bem montado. A maior melhoria agora é criar o comando `brandos-harness.md`, porque a auditoria já existe como ideia, mas precisa virar um comando operacional.

## 10. Próximo passo recomendado
Diga exatamente o que o usuário deve fazer agora.
```

---

# Regras de comportamento

## 1. Não invente arquivos

Se não conseguir confirmar que um arquivo existe, marque como não confirmado ou ausente.

Não diga que algo existe se não foi encontrado.

---

## 2. Seja direto

A usuária quer entender com clareza.

Evite respostas longas demais quando a dúvida for simples.

Use resumos como:

```md
Resumo simples:
A auditoria agora virou um comando.
Antes ela era só uma checklist.
```

---

## 3. Sempre explique o impacto

Não diga apenas:

```md
Falta commands/brandos-harness.md
```

Explique:

```md
Falta commands/brandos-harness.md.
Isso significa que a auditoria está planejada, mas ainda não pode ser rodada como comando dentro do Claude Code.
```

---

## 4. Dê correções práticas

Sempre que encontrar problema, diga como corrigir.

Exemplo:

```md
Correção recomendada:
Criar o arquivo commands/brandos-harness.md com este conteúdo de auditoria.
```

---

## 5. Use status visual

Use:

```txt
✅ Encontrado
⚠️ Atenção
❌ Ausente
```

Mas não exagere.

---

# Resultado esperado

Depois que este arquivo existir em:

```txt
commands/brandos-harness.md
```

O BrandOS passa a ter uma auditoria operacional.

Isso significa:

```txt
Antes: auditoria como checklist/manual
Depois: auditoria como comando do Claude Code
```

---

# Mensagem final padrão

Ao terminar qualquer auditoria, finalize com uma conclusão simples:

```md
Resumo simples:
O BrandOS está [pronto/quase pronto/incompleto].
O principal ajuste agora é [ação recomendada].
```
