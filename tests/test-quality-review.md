# Teste — Revisão de Qualidade (Gate 12)

**Tipo:** Teste de falha e QA  
**Objetivo:** Validar que o Governance + QA funciona como esperado

---

## Caso A — Briefing incompleto

**Entrada:**
```
Nome: Lume
Segmento: (não informado)
Público: (não informado)
Objetivo: "Quero uma marca bonita."
```

### Comportamento esperado

- [ ] O sistema NÃO gerou brand system completo imediatamente
- [ ] O sistema ativou Discovery e fez perguntas
- [ ] O sistema manteve linguagem amigável
- [ ] O sistema explicou por que precisa de mais informações
- [ ] O sistema NÃO inventou segmento ou público
- [ ] O sistema NÃO criou visual sem estratégia

---

## Caso B — Brand book genérico (teste de reprovação)

**Cenário:** Brand system foi gerado mas com posicionamento genérico.

```
Posicionamento: "Somos uma empresa inovadora que oferece qualidade e excelência."
```

### Comportamento esperado do Gate 12

- [ ] O Gate 12 reprovou o posicionamento
- [ ] O score de diferenciação ficou abaixo de 7
- [ ] O sistema identificou a falha como crítica
- [ ] O sistema não avançou para exportação
- [ ] O sistema listou ajustes obrigatórios claros

---

## Caso C — Contradição entre estratégia e verbal

**Cenário:** Brand DNA definiu tom "sério e técnico" mas verbal criou comunicação "informal e bem-humorada".

### Comportamento esperado do Gate 12

- [ ] O Gate 12 identificou a contradição
- [ ] O score de consistência geral ficou abaixo de 7
- [ ] O sistema sinalizou qual elemento está em conflito
- [ ] O sistema NÃO aprovou a entrega
- [ ] O sistema sugeriu como resolver a contradição

---

## Caso D — Aprovação correta

**Cenário:** Brand system completo e coerente, score ≥ 80.

### Comportamento esperado

- [ ] O Gate 12 aprovou a entrega
- [ ] O scorecard foi apresentado completo
- [ ] O sistema avançou para a fase de exportação
- [ ] O brand book foi gerado com todos os campos preenchidos
- [ ] O resumo executivo foi apresentado ao usuário

---

## Regras gerais do Gate 12

- [ ] Reprovação automática se score < 70
- [ ] Reprovação automática se critério crítico < 7
- [ ] Exportação bloqueada se Gate 12 não aprovado
- [ ] Checklist de exportação verificado antes de finalizar

---

## Status do teste de QA

- [ ] Aprovado
- [ ] Aprovado com ajustes
- [ ] Reprovado — ver falhas abaixo

**Falhas identificadas:**
