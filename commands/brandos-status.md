---
description: Mostra o progresso do BrandOS — em qual fase a marca está, o que já foi decidido e o que falta.
---

# /brandos-status — Progresso do pipeline

Mostre ao usuário onde a marca dele está no pipeline do BrandOS.

## O que fazer

1. Verifique se existe `brandos-output/` na raiz do projeto. Se não existir, informe que o BrandOS ainda não foi iniciado e sugira `/brandos`.
2. Leia os arquivos de memória em `brandos-output/memory/` e os documentos em `brandos-output/01-brand-system/`.
3. Determine a fase atual com base em quais documentos já existem.

## Formato do relatório

```txt
BrandOS — [Nome da Marca]

Caminho: [from-scratch / has-references / existing-brand]

Progresso:
✓ 1. Onboarding
✓ 2. Discovery Inicial
✓ 3. Materiais da Marca
→ 4. Competitive Discovery  (fase atual)
  5. Research Flow
  6. Audience Discovery
  ...
  14. Production System (opcional)

Já decidido:
- Posicionamento provisório: ...
- Hipóteses confirmadas: ...

Gates:
- Brand DNA (fase 8): pendente
- QA (fase 12): pendente

Próximo passo: [o que fazer para avançar]
```

## Regras

- Seja conciso. Status é um panorama rápido, não um relatório completo.
- Se um gate já foi aprovado, mostre o score (no caso do QA).
- Sempre termine indicando o próximo passo concreto.
- Para retomar a execução, oriente o usuário a usar `/brandos-resume`.
