---
description: Retoma o BrandOS de onde parou, carregando a memória da marca e continuando o pipeline.
---

# /brandos-resume — Retomar o pipeline

O usuário quer continuar um BrandOS já iniciado. Retome sem recomeçar e sem repetir perguntas já respondidas.

## O que fazer

1. Verifique se existe `brandos-output/` na raiz do projeto. Se não existir, informe que não há nada para retomar e sugira `/brandos`.
2. Leia **toda** a memória em `brandos-output/memory/`:
   - `brand-dna.json`
   - `strategic-memory.json`
   - `creative-memory.json`
   - `audience-memory.json`
   - `decision-memory.json`
   - `conversation-memory.json`
   - `production-memory.json`
   - `campaign-memory.json`
3. Leia os documentos já gerados em `brandos-output/01-brand-system/`.
4. Determine a fase atual e o caminho de onboarding.
5. Faça um resumo curto para o usuário do que já foi construído.
6. Invoque o `brandos-core` via Task, passando todo o contexto da memória, e continue da próxima fase pendente.

## Resumo de retomada (mostre antes de continuar)

```txt
Retomando o BrandOS — [Nome da Marca] ✨

O que já construímos:
- Caminho: ...
- Fases concluídas: ...
- Posicionamento: ...
- Decisões aprovadas: ...

Vamos continuar da fase [N]: [nome da fase].
```

## Regras

- Nunca repita uma pergunta já respondida. A memória é a fonte da verdade.
- Se o usuário pedir para revisar uma fase anterior em vez de continuar, atenda — e propague as mudanças para a memória e para as fases dependentes.
- Se a memória estiver corrompida ou incompleta, diga exatamente o que está faltando antes de continuar.
