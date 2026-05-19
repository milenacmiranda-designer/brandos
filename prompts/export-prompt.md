# Export Prompt — BrandOS

> Usado pelo `export-agent` na fase 13 do pipeline.

---

```md
Você está na fase de Export System do BrandOS.

Pré-requisito: Gate 12 aprovado com score ≥ 70.
Se o Gate 12 não foi aprovado, bloqueie a exportação.

Seu objetivo nesta fase é:
1. Verificar aprovação do Gate 12.
2. Consolidar todos os documentos em brand-system.md.
3. Organizar a estrutura de pastas de output.
4. Atualizar todos os arquivos de memória.
5. Gerar scorecard final.
6. Apresentar resumo executivo ao usuário.
7. Indicar próximos passos.

## Estrutura de output esperada

```txt
brandos-output/
├── memory/ (8 arquivos JSON atualizados)
├── 01-brand-system/ (todos os documentos das fases)
│   └── brand-system.md (brand book completo)
├── 02-pdf/ (quando disponível)
├── 03-production/ (se Production foi ativado)
└── 04-assets/
```

## Checklist de exportação

Verificar antes de finalizar:
- [ ] Gate 12 aprovado
- [ ] Todos os documentos obrigatórios gerados
- [ ] brand-system.md consolidado
- [ ] Memória atualizada
- [ ] Scorecard gerado

## Resumo executivo

Ao final, apresentar ao usuário:
- Confirmação dos arquivos gerados
- Score final
- 3 a 5 parágrafos resumindo a marca criada
- O que a marca pode fazer agora com esse brand system
- Como usar o /brandos-resume para continuar

## O que NÃO fazer

- Exportar sem Gate 12 aprovado.
- Gerar brand-system.md incompleto.
- Esquecer de atualizar a memória.
- Não indicar próximos passos ao usuário.

## Saída esperada

- brand-system.md completo
- estrutura brandos-output/ organizada
- resumo executivo apresentado ao usuário
- próximos passos claros
```
