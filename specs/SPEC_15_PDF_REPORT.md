# SPEC_14_PDF_REPORT — PDF Report Design System: Swiss Editorial Layout

## Objetivo

Definir como o BrandOS deve transformar o conteúdo estratégico coletado no briefing em um relatório PDF completo, editorial e visualmente profissional, inspirado no Swiss Design / International Typographic Style.

## Quando esta fase é ativada

Esta fase é ativada pelo Output Decision Gate, após a consolidação do briefing estratégico, quando o usuário escolhe a opção "Gerar Relatório PDF Completo".

```txt
Briefing Estratégico
↓
Consolidação das Respostas
↓
Validação do Briefing pelo Usuário
↓
Output Decision Gate
↓
Escolha do Usuário:
  1. Gerar Relatório PDF Completo  → SPEC_14_PDF_REPORT (esta fase)
  2. Avançar para Propostas de Layout → Layout Proposal Studio
  3. Revisar ou Complementar Respostas → retorna ao briefing
```

## Pré-requisito

- Briefing estratégico completo e validado pelo usuário.
- Esta fase não exige Gate 12. É uma entrega intermediária que pode ser gerada antes da identidade completa.

## Direção visual obrigatória

O relatório deve seguir estética inspirada no **Swiss Design / International Typographic Style**:

- Clareza, ordem, racionalidade, precisão
- Grid modular (6 ou 12 colunas)
- Hierarquia tipográfica forte
- Alinhamento preciso (preferência: à esquerda)
- Uso generoso de espaço em branco
- Paleta reduzida: fundo claro, preto, branco, cinzas + 1 cor de destaque
- Elementos gráficos simples: linhas, barras, blocos, numeração grande
- Sem decoração excessiva

## Estrutura do relatório

O PDF deve conter, sempre que aplicável, as seguintes seções:

| # | Seção | Conteúdo principal |
|---|-------|--------------------|
| Capa | — | Nome da marca, título, subtítulo, data, elemento gráfico modular |
| Sumário | — | Seções numeradas, alinhamento em grid, visual limpo |
| 01 | Introdução | Contexto da marca, objetivo do projeto, como usar o documento |
| 02 | Diagnóstico Estratégico | Contexto do negócio, problema/oportunidade, objetivos, mercado, concorrência, diferenciais |
| 03 | Núcleo da Marca | Propósito, missão, visão, valores, essência, personalidade, promessa, crenças |
| 04 | Posicionamento | Declaração de posicionamento, território, proposta de valor, diferenciais, percepção desejada |
| 05 | Público e Personas | Público-alvo, segmentos, dores, desejos, barreiras, motivações, personas |
| 06 | Universo Verbal | Tom de voz, linguagem, palavras recomendadas/a evitar, mensagens-chave, exemplos |
| 07 | Universo Visual | Direção visual, estilo gráfico, paleta sugerida, tipografia, fotografia, atmosfera |
| 08 | Diretrizes de Aplicação | Redes sociais, landing pages, apresentações, materiais comerciais, campanhas |
| 09 | Recomendações Estratégicas | Próximos passos, pontos de atenção, oportunidades, sugestões de evolução |
| Encerramento | — | Essência da marca, direção estratégica, valor do sistema, próxima etapa sugerida |

## Tipos de página

O sistema deve usar diferentes tipos de página para criar ritmo editorial:

| Tipo | Uso | Características |
|------|-----|-----------------|
| Abertura de seção | Iniciar uma nova parte | Número grande, título forte, subtítulo curto, muito espaço em branco |
| Conteúdo estratégico | Explicar conceitos e decisões | Título claro, texto em blocos, cards ou colunas, destaques visuais |
| Insight | Destacar uma ideia importante | Frase principal grande, pouco texto, forte contraste, composição limpa |
| Tabela / comparação | Organizar informações comparativas | Tabela simples, linhas finas, poucas cores, boa legibilidade |
| Diretrizes | Apresentar regras de uso da marca | Blocos objetivos, exemplos práticos, organização modular |
| Visual | Referências, moodboards, direções visuais | Imagens no grid, legendas curtas, composição limpa |

## Sistema tipográfico

```txt
Máximo: 2 famílias tipográficas
Preferência: fontes sem serifa, editorial, alto contraste entre pesos

Hierarquia:
  Título de capa:   muito grande
  Título de seção:  grande
  Título de página: médio/grande
  Subtítulo:        médio
  Corpo de texto:   legível
  Legenda:          pequena
  Dados secundários: pequena/média
```

## Sistema de cores

```txt
Fundo:             branco ou off-white
Texto principal:   preto ou grafite
Texto secundário:  cinza
Linhas/divisórias: cinza claro
Cor de destaque:   cor principal da marca (ou definida estrategicamente)
```

Regras:
- Não usar muitas cores ao mesmo tempo
- Não usar gradientes excessivos
- Usar cor para orientar leitura, não apenas decorar
- Manter consistência entre as páginas

## Componentes visuais recorrentes

| Componente | Uso |
|------------|-----|
| Header editorial | Nome da marca, seção, número da página, categoria |
| Numeração de seção | Números grandes para organizar: `01 / Diagnóstico Estratégico` |
| Cards informativos | Insights, valores, características, recomendações, resumos |
| Barras e linhas | Separar blocos, guiar leitura, criar ritmo, reforçar grid |
| Blocos de destaque | Promessa da marca, essência, posicionamento, mensagem central |

## Regras de qualidade visual

Antes de finalizar, revisar:

- [ ] Páginas têm hierarquia clara
- [ ] Grid está consistente
- [ ] Texto está legível
- [ ] Há espaço em branco suficiente
- [ ] Seções estão bem separadas
- [ ] Títulos estão fortes
- [ ] Paleta está consistente
- [ ] Relatório parece profissional, não genérico

## Regras de escrita

O conteúdo deve ser:
- Claro, estratégico, profissional, didático, organizado
- Adequado ao nível do usuário (adaptar se for iniciante)

Evitar:
- Linguagem genérica ou vaga
- Frases muito longas
- Termos técnicos sem explicação
- Conteúdo que parece preenchimento automático

## O que NÃO gerar

- Texto corrido demais
- Páginas muito cheias
- Layout desalinhado
- Excesso de cores, ícones ou fontes decorativas
- Aparência de template Word genérico
- Falta de hierarquia, respiro ou consistência

## Saída esperada

```txt
brandos-output/02-pdf/brand-report-swiss.md   ← conteúdo editorial do relatório
brandos-output/02-pdf/brand-report.pdf         ← PDF final (ou .html se sem ferramenta de PDF)
```

## Agente responsável

`export-agent` (acionado pelo Output Decision Gate na fase 13)
