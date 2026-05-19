# SPEC_07_BRAND_PERSONALITY — Personalidade da Marca

## Objetivo

Definir a personalidade da marca, seus atributos, energia e comportamento.

## Entrada necessária

- posicionamento aprovado
- personas
- segmento
- tipo de marca
- percepção desejada pelo usuário
- referências de marcas admiradas
- tom desejado (inicial)

## Processo

O agente deve definir:

1. arquétipo dominante (usando os 12 arquétipos de Jung adaptados para branding)
2. arquétipo secundário, se necessário para nuance
3. 3 a 5 atributos principais da personalidade
4. energia da marca (dinâmica, serena, ousada, técnica...)
5. postura comunicacional (como a marca "fala")
6. características humanas (se fosse uma pessoa, seria...)
7. limites de comportamento (o que a marca não faz)

## Arquétipos disponíveis

- Inocente — pureza, otimismo, simplicidade
- Explorador — liberdade, descoberta, aventura
- Sábio — conhecimento, expertise, clareza
- Herói — superação, coragem, conquista
- Fora-da-lei — ruptura, provocação, mudança
- Mago — transformação, visão, magia
- Cara Comum — pertencimento, autenticidade, praticidade
- Amante — sensorialidade, conexão, desejo
- Bobo da Corte — leveza, humor, liberdade criativa
- Cuidador — cuidado, proteção, empatia
- Criador — expressão, originalidade, construção
- Governante — autoridade, ordem, liderança

## Saída esperada

A entrega deve conter:

- personalidade central (1 parágrafo descritivo)
- 3 a 5 atributos principais com descrição curta
- arquétipo dominante com justificativa
- arquétipo secundário, se fizer sentido
- como a marca se comporta na comunicação
- como a marca não deve se comportar
- exemplos práticos de atitude da marca
- implicações para tom de voz
- implicações para identidade visual

## Critérios de qualidade

A personalidade deve ser:

- coerente com o posicionamento e as personas
- memorável e distinta
- aplicável na prática (verbal e visual)
- conectada ao que o público valoriza
- útil para orientar qualquer decisão de comunicação

## O que evitar

- Atributos demais (mais de 5 dilui a identidade)
- Atributos contraditórios sem intenção clara
- Arquétipos escolhidos apenas por "soar bem"
- Personalidade genérica ("moderna, inovadora, confiável")
- Personalidade sem aplicação prática nas entregas

## Template de saída

```md
# Personalidade da Marca — [Nome]

## Personalidade central

## Arquétipo dominante

**Arquétipo:** [nome]
**Por quê:** 

## Arquétipo secundário (se aplicável)

## Atributos principais

| Atributo | Como se manifesta |
|----------|-------------------|
|          |                   |

## Como a marca se comporta

## Como a marca NÃO se comporta

## Exemplos de atitude da marca

## Implicações para tom de voz

## Implicações para identidade visual
```

## Agente responsável

`brand-dna-agent`
