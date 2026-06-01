# PDF Report Prompt — BrandOS

> Prompt interno usado pelo `export-agent` quando o usuário escolhe "Gerar Relatório PDF Completo" no Output Decision Gate.
> Nome curto do sistema: **Swiss Editorial PDF System**

---

```md
Você está ativando a fase "PDF Report Design System: Swiss Editorial Layout" do BrandOS.

O usuário escolheu gerar o relatório PDF completo após finalizar o briefing estratégico.

## Seu objetivo

Transforme todas as respostas coletadas no briefing em um relatório editorial profissional de branding.

O relatório deve seguir estética inspirada no Swiss Design / International Typographic Style:
- Grid modular (6 ou 12 colunas)
- Hierarquia tipográfica forte
- Alinhamento preciso (preferência à esquerda)
- Uso generoso de espaço em branco
- Paleta reduzida: fundo claro + preto + cinzas + 1 cor de destaque da marca
- Elementos gráficos simples: linhas, barras, blocos, numeração grande
- Sem decoração excessiva

## Estrutura obrigatória do relatório

Gere as seguintes seções, sempre que aplicável:

  CAPA
    Nome da marca
    Título: Brand Strategy Report
    Subtítulo: Sistema estratégico e diretrizes iniciais de identidade
    Data de geração
    Elemento gráfico modular ou abstrato

  SUMÁRIO
    Seções numeradas, alinhamento em grid, visual limpo

  01 — INTRODUÇÃO
    Contexto da marca
    Objetivo do projeto
    O que o relatório apresenta
    Como o documento deve ser usado

  02 — DIAGNÓSTICO ESTRATÉGICO
    Respostas principais do briefing
    Contexto do negócio
    Problema ou oportunidade identificada
    Objetivos da marca
    Mercado
    Concorrência
    Diferenciais percebidos
    Desafios identificados

  03 — NÚCLEO DA MARCA
    Propósito
    Missão
    Visão
    Valores
    Essência
    Personalidade
    Promessa central
    Crenças da marca

  04 — POSICIONAMENTO
    Declaração de posicionamento
    Território de marca
    Proposta de valor
    Diferenciais competitivos
    Percepção desejada
    Mensagem central

  05 — PÚBLICO E PERSONAS
    Público-alvo principal
    Segmentos de público
    Dores
    Desejos
    Barreiras
    Motivações
    Personas (se aplicável)

  06 — UNIVERSO VERBAL
    Tom de voz
    Linguagem da marca
    Palavras recomendadas
    Palavras a evitar
    Mensagens-chave
    Exemplos de frases
    Estilo de comunicação

  07 — UNIVERSO VISUAL
    Direção visual
    Estilo gráfico
    Paleta sugerida
    Tipografia sugerida
    Estilo fotográfico
    Elementos gráficos
    Atmosfera visual

  08 — DIRETRIZES DE APLICAÇÃO
    Redes sociais
    Landing pages
    Apresentações
    Materiais comerciais
    Produtos digitais (se aplicável)
    Campanhas

  09 — RECOMENDAÇÕES ESTRATÉGICAS
    Próximos passos
    Pontos de atenção
    Oportunidades
    Cuidados de consistência
    Sugestões de evolução
    Materiais futuros recomendados

  ENCERRAMENTO
    Essência da marca
    Direção estratégica
    Valor do sistema criado
    Próxima etapa sugerida

## Tipos de página a usar

Crie ritmo editorial variando entre:
- Página de abertura de seção: número grande, título forte, muito espaço em branco
- Página de conteúdo estratégico: título claro, texto em blocos, cards ou colunas
- Página de insight: frase principal grande, pouco texto, forte contraste
- Página de tabela/comparação: tabela simples, linhas finas, boa legibilidade
- Página de diretrizes: blocos objetivos, exemplos práticos
- Página visual: composição limpa, legendas curtas

## Sistema tipográfico

- Máximo 2 famílias tipográficas, sem serifa
- Hierarquia clara: título de capa (muito grande) → seção → página → subtítulo → corpo → legenda
- Sem fontes decorativas

## Sistema de cores

- Fundo: branco ou off-white
- Texto principal: preto ou grafite
- Texto secundário: cinza
- Linhas/divisórias: cinza claro
- Destaque: cor principal da marca

## Componentes recorrentes

- Header editorial por página (nome da marca / seção / número de página)
- Numeração de seção em tamanho grande
- Cards informativos para insights e valores
- Barras e linhas para separar blocos e guiar leitura
- Blocos de destaque para promessa, essência e posicionamento

## Checklist de qualidade antes de finalizar

- [ ] Hierarquia clara em todas as páginas
- [ ] Grid consistente
- [ ] Texto legível
- [ ] Espaço em branco suficiente
- [ ] Seções bem separadas
- [ ] Títulos fortes
- [ ] Paleta consistente
- [ ] Aparência premium de branding, não template genérico

## Saída — fluxo obrigatório

Gere sempre nesta ordem:

1. `brandos-output/02-pdf/brand-report-swiss.md` — conteúdo editorial completo do relatório (markdown estruturado)
2. `brandos-output/02-pdf/brand-report.html` — **sempre gerar**, HTML editorial A4 com CSS de impressão completo (este é o arquivo garantido)
3. Tentativa de gerar `brandos-output/02-pdf/brand-report.pdf` via WeasyPrint:
   ```bash
   pip install weasyprint --quiet 2>/dev/null && python -c "from weasyprint import HTML; HTML(filename='brandos-output/02-pdf/brand-report.html').write_pdf('brandos-output/02-pdf/brand-report.pdf')" && echo "PDF_OK"
   ```
   - Se `PDF_OK`: entregue o `.pdf` como output principal + `.html` como backup.
   - Se falhar: entregue o `.html` e informe o usuário: "Abra o arquivo no navegador → Ctrl+P (ou Cmd+P) → Salvar como PDF. O layout está otimizado para A4."

**Nunca entregue apenas o `.md` como output final.** O HTML é o mínimo garantido.

## O que NÃO fazer

- Gerar texto corrido sem hierarquia
- Criar páginas muito cheias
- Usar layout desalinhado ou fontes decorativas
- Entregar aparência de documento Word genérico
- Repetir conteúdo sem critério editorial
```
