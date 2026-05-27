# SPEC_10_KEY_VISUAL — Key Visual & Direção de Aplicações

## Objetivo

Transformar a identidade visual conceitual em uma direção visual aplicada e coesa — a imagem-mãe da marca que orienta todos os layouts e desdobramentos gráficos futuros.

## Posição no pipeline

Entra após a Fase 10 (Visual Identity) e antes da Fase 11 (UX + Product Experience) e das Propostas de Layout.

## Trigger

Executar após a conclusão da fase de Visual Identity.

## Agente responsável

`key-visual-agent`

## Required Inputs

- `brand_name`
- `segment`
- `target_audience`
- `positioning`
- `brand_dna`
- `verbal_identity`
- `color_palette`
- `typography`
- `visual_references`
- `image_style`
- `application_goals`
- `priority_channels`

## Optional Inputs

- logo existente
- símbolo
- materiais antigos
- benchmark de concorrentes
- estilos proibidos

## Processing Rules

- Não gerar layouts finais antes de consolidar a direção visual aplicada.
- Usar o Brand DNA como filtro de consistência em todas as decisões.
- Validar se a direção visual reforça o posicionamento.
- Criar pelo menos uma composição principal e variações de aplicação.
- Gerar checklist de validação antes de liberar para Propostas de Layout.
- Se o usuário pular esta fase: registrar `key_visual.status = "skipped"` na memória e avisar que os layouts serão gerados sem referência visual central.

## Output principal

`09-key-visual-direcao-aplicacoes.md`

## Campos do output

```md
# Key Visual & Direção de Aplicações

## 1. Conceito visual central
## 2. Objetivo do Key Visual
## 3. Elementos principais da composição
## 4. Direção tipográfica aplicada
## 5. Direção cromática aplicada
## 6. Direção de imagem
## 7. Grafismos e elementos de apoio
## 8. Grid e composição
## 9. Headline visual principal
## 10. Variações do Key Visual
## 11. Aplicações recomendadas
## 12. Regras de consistência
## 13. Checklist de validação
```

## Outputs secundários

- `key_visual_summary` — bloco curto para uso pelo export-agent no PDF
- `application_guidelines` — regras de desdobramento para layouts
- `consistency_checklist` — checklist aprovado

## Checklist de validação (gate interno)

- [ ] O Key Visual reflete o posicionamento da marca?
- [ ] O Key Visual traduz o Brand DNA?
- [ ] A composição tem hierarquia clara?
- [ ] A paleta foi aplicada de forma coerente?
- [ ] A tipografia foi aplicada de forma funcional?
- [ ] O estilo de imagem está alinhado ao território visual?
- [ ] Os grafismos reforçam a identidade da marca?
- [ ] O sistema visual pode ser desdobrado em diferentes peças?
- [ ] Existe consistência entre verbal e visual?
- [ ] O Key Visual orienta layouts futuros?
- [ ] A direção está clara para designers e não-designers?
- [ ] O material pode entrar no PDF final da marca?

## Integração com outros módulos

- **Propostas de Layout:** usa `key_visual` como referência base. Se não existir, usa `visual_identity + brand_dna + positioning`.
- **Swiss Editorial PDF (SPEC_15):** inclui seção "Key Visual & Direção de Aplicações" com conceito, composição, cor, tipografia, imagem, grafismos, variações e regras.
- **Memória persistente:** salva campo `key_visual` em `creative-memory.json`.

## Critérios de aprovação da fase

A fase é concluída quando:

1. Conceito visual central documentado
2. Elementos principais definidos
3. Orientação de composição entregue
4. Cor aplicada documentada
5. Tipografia aplicada documentada
6. Estilo de imagem definido
7. Grafismos definidos
8. Aplicações sugeridas
9. Checklist de consistência aprovado
10. Usuário validou ou solicitou ajustes

## Regras de qualidade

O Key Visual deve ser: estratégico, visualmente coerente, aplicável, escalável, conectado ao Brand DNA e compreensível para designers e não-especialistas.

Não deve ser: genérico, apenas decorativo, desconectado da estratégia, limitado a uma única peça, contraditório com o tom de voz.
