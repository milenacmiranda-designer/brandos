# SPEC_12_REVIEW — Revisão de Qualidade (Gate 12)

## Objetivo

Definir como o BrandOS deve revisar a qualidade e consistência das entregas antes da exportação final.

## Quando ativar

Esta spec é o Gate 12 — obrigatório. Nenhum output final deve ser exportado sem passar por esta revisão.

## Entrada necessária

- todos os documentos gerados nas fases anteriores
- scorecard parcial acumulado
- Brand DNA aprovado no Gate 8
- decisões registradas na memória

## Processo

O agente deve verificar:

1. coerência entre briefing e estratégia
2. coerência entre personas e posicionamento
3. clareza e especificidade da proposta de valor
4. coerência entre personalidade e tom de voz
5. coerência entre identidade verbal e visual
6. ausência de contradições entre documentos
7. profundidade estratégica adequada ao projeto
8. aplicabilidade prática das entregas
9. qualidade da linguagem (natural, não genérica)
10. utilidade real dos entregáveis para o usuário

## Critérios de aprovação

### Aprovação automática

Score geral ≥ 80/100 e nenhum critério crítico abaixo de 7.

### Aprovação com ajustes obrigatórios

Score entre 70 e 79 — pode avançar após correções identificadas.

### Reprovação automática

Score < 70 OU qualquer um dos seguintes:

- posicionamento genérico ou não defensável
- Brand DNA contradiz o briefing
- identidade verbal desalinhada com a personalidade
- identidade visual sem conceito estratégico
- inconsistência grave entre duas ou mais seções
- entregáveis obrigatórios ausentes

## Rubrica de pontuação

| Critério | Peso | É crítico? |
|----------|------|------------|
| Clareza estratégica | 10 | Não |
| Coerência com briefing | 10 | Sim |
| Público-alvo | 10 | Não |
| Posicionamento | 10 | Sim |
| Diferenciação | 10 | Sim |
| Brand DNA | 10 | Sim |
| Identidade verbal | 10 | Não |
| Identidade visual | 10 | Não |
| Aplicabilidade | 10 | Não |
| Consistência geral | 10 | Sim |

Critérios críticos (marcados com Sim) devem ter nota ≥ 7, independente do score total.

## Saída esperada

Uma revisão contendo:

- score por critério (0 a 10 cada)
- score total (0 a 100)
- status: Reprovado / Aprovado com ajustes / Aprovado / Excelente
- pontos fortes identificados
- pontos a melhorar
- inconsistências encontradas
- ajustes obrigatórios (se houver)
- recomendações de refinamento
- recomendação final: exportar ou revisar primeiro

## Template de saída

```md
# Governance + QA — [Nome da Marca]

## Score por critério

| Critério | Nota | Observação |
|----------|------|------------|
| Clareza estratégica | /10 | |
| Coerência com briefing | /10 | |
| Público-alvo | /10 | |
| Posicionamento | /10 | |
| Diferenciação | /10 | |
| Brand DNA | /10 | |
| Identidade verbal | /10 | |
| Identidade visual | /10 | |
| Aplicabilidade | /10 | |
| Consistência geral | /10 | |

**Score total:** /100
**Status:** 

## Pontos fortes

- 

## Inconsistências encontradas

- 

## Ajustes obrigatórios

- 

## Recomendações

- 

## Decisão final

[ ] Aprovado para exportação
[ ] Aprovado com ajustes obrigatórios antes de exportar
[ ] Reprovado — revisar antes de avançar
```

## Agente responsável

`governance-qa-agent`
