# SPEC_13_EXPORT — Exportação Final

## Objetivo

Definir como o BrandOS deve organizar e exportar os arquivos finais do Brand System.

## Pré-requisito

A exportação só pode ocorrer após aprovação no Gate 12 (SPEC_12_REVIEW).

Se o score for < 70, a exportação deve ser bloqueada.

## Processo

O agente deve:

1. Verificar aprovação do Gate 12
2. Consolidar todos os documentos das fases
3. Gerar o `brand-system.md` completo
4. Organizar a estrutura de pastas
5. Atualizar arquivos de memória
6. Gerar scorecard final em JSON
7. Gerar log da execução
8. Apresentar resumo da entrega ao usuário
9. Indicar próximos passos

## Estrutura de exportação

```txt
brandos-output/
├── memory/
│   ├── brand-dna.json
│   ├── strategic-memory.json
│   ├── creative-memory.json
│   ├── audience-memory.json
│   ├── decision-memory.json
│   ├── conversation-memory.json
│   ├── production-memory.json
│   └── campaign-memory.json
├── 01-brand-system/
│   ├── 01-overview.md
│   ├── 02-discovery.md
│   ├── 03-brand-context.md         ← se aplicável
│   ├── 04-competitive-research.md
│   ├── 05-audience.md
│   ├── 06-strategy.md
│   ├── 07-brand-dna.md
│   ├── 08-verbal-identity.md
│   ├── 09-visual-identity.md
│   ├── 10-ux-product-experience.md ← se aplicável
│   ├── 11-governance-qa.md
│   └── brand-system.md             ← brand book completo
├── 02-pdf/
│   └── brand-guidelines.pdf        ← quando disponível
├── 03-production/                  ← se Production System foi ativado
│   ├── social-posts.md
│   ├── landing-page-copy.md
│   ├── prompt-visual.md
│   └── campaign-ideas.md
└── 04-assets/
    └── README.md
```

## Saída esperada

Ao final da exportação, o agente deve apresentar:

- confirmação de todos os arquivos gerados
- checklist de entregáveis completa
- score final do projeto
- resumo executivo da marca (3 a 5 parágrafos)
- próximos passos recomendados
- instrução sobre como usar o `/brandos-resume` para continuar

## Regras de exportação

Os arquivos finais devem:

- ter nomes em kebab-case sem espaços
- seguir numeração sequencial
- evitar duplicidade de conteúdo
- manter linguagem consistente em todo o Brand System
- respeitar o PRD e as Specs
- ser fáceis de localizar e consultar

## Checklist de exportação

```txt
[ ] Gate 12 aprovado com score ≥ 70
[ ] Pasta brandos-output/ criada
[ ] Arquivos de memória atualizados
[ ] Todos os documentos obrigatórios gerados
[ ] brand-system.md consolidado
[ ] Scorecard final gerado
[ ] Log de execução registrado
[ ] Resumo executivo apresentado ao usuário
[ ] Próximos passos indicados
```

## Agente responsável

`export-agent`
