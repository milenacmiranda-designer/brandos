# Skill — Briefing Analysis

**Tipo:** Skill reutilizável  
**Usada por:** `discovery-agent`, `onboarding-agent`, `brand-dna-agent`

---

## O que esta skill faz

Analisa qualquer briefing recebido e extrai:
- o que está claro
- o que está vago ou incompleto
- o que é essencial e ainda falta
- os próximos passos recomendados

---

## Quando usar

- Ao receber o briefing inicial do usuário
- Antes de avançar para qualquer fase estratégica
- Quando o usuário trouxer informações soltas e desestruturadas
- Para validar se há informação suficiente para começar

---

## Processo

```
1. Ler o briefing disponível
2. Categorizar as informações recebidas:
   - Identidade: nome, tipo de projeto, segmento
   - Objetivo: o que a marca precisa alcançar
   - Público: quem vai ser atendido
   - Oferta: produto ou serviço
   - Diferenciais: o que torna única
   - Referências: o que o usuário admira
   - Restrições: o que não pode fazer
3. Identificar lacunas críticas (bloqueiam estratégia)
4. Identificar lacunas secundárias (podem ser inferidas)
5. Gerar relatório de análise
6. Recomendar próximas perguntas ou avançar para a estratégia
```

---

## Saída

```md
## Análise do Briefing

### O que está claro
- 

### O que está vago
- 

### O que está ausente (crítico)
- 

### O que está ausente (secundário)
- 

### Recomendação
[ ] Avançar para a estratégia — informações suficientes
[ ] Fazer mais perguntas antes de avançar
[ ] Perguntas prioritárias: ...
```

---

## Critérios de uso

- Usar antes de qualquer fase estratégica
- Não bloquear o usuário por lacunas secundárias
- Lacunas críticas devem ser preenchidas antes de avançar
- Informações ausentes não críticas podem ser inferidas com transparência
