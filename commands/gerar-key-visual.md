---
name: gerar-key-visual
description: Gera o Key Visual da marca — a imagem-mãe que orienta todos os layouts e aplicações visuais. Use após concluir a identidade visual.
---

# /gerar-key-visual

Aciona a fase de **Key Visual & Direção de Aplicações** do BrandOS.

## Quando usar

Use este comando depois que a identidade visual da marca estiver definida (cores, tipografia, moodboard, estilo de imagem). Use antes de criar layouts, posts, landing pages ou brand book.

## O que o sistema faz

1. Verifica se Brand DNA, Verbal Identity e Visual Identity estão concluídos.
2. Lê os dados consolidados das fases anteriores.
3. Identifica lacunas e solicita complemento se necessário.
4. Gera a direção de Key Visual completa.
5. Salva o arquivo `09-key-visual-direcao-aplicacoes.md`.
6. Atualiza `creative-memory.json` com o campo `key_visual`.
7. Libera a etapa de propostas de layout.

## Output gerado

`09-key-visual-direcao-aplicacoes.md` contendo:

- conceito visual central
- composição principal
- direção tipográfica aplicada
- direção cromática aplicada
- estilo de imagem
- grafismos e elementos de apoio
- grid e hierarquia
- headline visual principal
- variações
- aplicações recomendadas
- regras de consistência
- checklist de validação

## Regra importante

Se você ainda não tiver concluído a identidade visual, o sistema vai alertar e pedir que você complete essa etapa primeiro.

Se quiser pular o Key Visual e ir direto para layouts, o sistema vai registrar isso na memória e avisar que os layouts serão criados sem referência visual central.
