# Skill — Quality Review

**Tipo:** Skill reutilizável  
**Usada por:** `governance-qa-agent`

---

## O que esta skill faz

Revisa coerência, consistência e qualidade de qualquer entrega do BrandOS antes de aprovação ou exportação.

---

## Quando usar

- Gate 8 (Brand DNA) — revisar base estratégica
- Gate 12 (Governance + QA) — revisar sistema completo
- Qualquer fase que precisar de validação parcial

---

## 10 critérios de avaliação

| # | Critério | Peso | É crítico? |
|---|----------|------|------------|
| 1 | Clareza estratégica | 10 | Não |
| 2 | Coerência com briefing | 10 | Sim |
| 3 | Público-alvo | 10 | Não |
| 4 | Posicionamento | 10 | Sim |
| 5 | Diferenciação | 10 | Sim |
| 6 | Brand DNA | 10 | Sim |
| 7 | Identidade verbal | 10 | Não |
| 8 | Identidade visual | 10 | Não |
| 9 | Aplicabilidade | 10 | Não |
| 10 | Consistência geral | 10 | Sim |

Critérios críticos devem ter nota ≥ 7, independente do score total.

---

## Regras de aprovação

| Score | Status |
|-------|--------|
| 0–69 | Reprovado |
| 70–79 | Aprovado com ajustes obrigatórios |
| 80–89 | Aprovado |
| 90–100 | Excelente |

---

## Processo

```
1. Ler todos os documentos disponíveis
2. Avaliar cada critério com nota de 0 a 10
3. Registrar observações por critério
4. Identificar inconsistências entre documentos
5. Calcular score total
6. Determinar status
7. Listar ajustes obrigatórios (se houver)
8. Fazer recomendações de refinamento
9. Emitir decisão final
```

---

## Saída

```md
## Governance + QA — [Nome da Marca]

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

## Inconsistências

## Ajustes obrigatórios

## Recomendações

## Decisão: [ ] Aprovado / [ ] Revisar antes de exportar
```

---

## Reprovação automática

Reprovar imediatamente se:

- posicionamento genérico ou não defensável
- contradição grave entre estratégia e Brand DNA
- identidade verbal desalinhada da personalidade
- identidade visual sem conceito estratégico
- entregáveis obrigatórios ausentes
