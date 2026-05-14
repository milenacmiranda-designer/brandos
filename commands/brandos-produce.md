---
description: Entra direto no Production System do BrandOS para produzir materiais (packs ou itens específicos) usando uma marca já construída.
---

# /brandos-produce — Production System

O usuário quer produzir materiais reais usando uma marca já construída no BrandOS — sem repassar o pipeline inteiro.

## Pré-requisito

Verifique se a Parte 1 está finalizada. Procure por:
- `brandos-output/memory/brand-dna.json` preenchido
- `brandos-output/02-pdf/brand-system.md` gerado

Se a marca **não** estiver finalizada, informe o usuário e sugira `/brandos` (para criar) ou `/brandos-resume` (para continuar). Não produza materiais sobre uma marca incompleta — produção genérica é veto.

## O que fazer

1. Leia `brand-dna.json` e a memória completa em `brandos-output/memory/`.
2. Invoque o `production-agent` via Task, passando todo o contexto da marca.
3. O `production-agent` conduz: escolha entre packs prontos ou itens específicos, nível de entrega, e produção contextual.

## Lembrete de produção contextual

Tudo que for produzido reutiliza automaticamente: paleta, tipografia, tom de voz, arquétipo, direção visual, posicionamento e público — direto do Brand DNA. Nada genérico.

## Saída

Os materiais vão para `brandos-output/03-production/`. A memória de produção (`production-memory.json` e `campaign-memory.json`) é atualizada a cada material criado.
