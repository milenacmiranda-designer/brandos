# BrandOS — Visão Geral do Sistema

## O que é o BrandOS

O BrandOS é um sistema operacional de branding com IA, criado para conduzir o usuário por um processo completo de construção de marca.

Ele não é um gerador de logotipo, slogan ou paleta. É uma estrutura estratégica que conecta:

- diagnóstico e briefing
- pesquisa de mercado
- personas e público
- posicionamento e proposta de valor
- personalidade de marca
- identidade verbal
- identidade visual
- brand book completo

---

## Como o sistema funciona

```txt
PRD → Specs → Scaffold → Agents → Subagents → Skills → Workflows → Templates → Outputs → Review
```

Cada camada tem uma função:

| Camada | Função |
|--------|--------|
| PRD | Define o que o BrandOS é e para que serve |
| Specs | Define como cada etapa funciona |
| Scaffold | Define onde cada arquivo fica |
| Agents | Executam as 14 fases do pipeline |
| Subagents | Especialistas para tarefas pontuais |
| Skills | Habilidades reutilizáveis por múltiplos agentes |
| Workflows | Orquestram a ordem de execução |
| Templates | Padronizam o formato das entregas |
| Outputs | Armazenam os resultados finais |
| Review | Garante qualidade, coerência e aplicabilidade |

---

## O pipeline de 14 fases

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
 08  Brand DNA ◆ gate obrigatório

IDENTIDADE
 09  Verbal Identity
 10  Visual Identity
 11  UX + Product Experience (condicional)

VALIDAÇÃO + ENTREGA
 12  Governance + QA ◆ gate obrigatório
 13  Export System
 14  Production System (condicional)
```

---

## Os dois gates obrigatórios

**Gate 8 — Brand DNA**
Nenhuma decisão de identidade verbal ou visual avança sem a base estratégica aprovada.

**Gate 12 — Governance + QA**
Nenhum brand book é exportado sem passar pela revisão de consistência e qualidade.

---

## Como usar o BrandOS

| Comando | O que faz |
|---------|-----------|
| `/brandos` | Inicia o pipeline completo |
| `/brandos-status` | Mostra progresso e fase atual |
| `/brandos-resume` | Retoma de onde parou |
| `/brandos-produce` | Gera materiais do Production System |

---

## Estrutura de arquivos

Ver [SPEC_00_OVERVIEW.md](../specs/SPEC_00_OVERVIEW.md) para a arquitetura completa.
