# SPEC_01_BRIEFING — Briefing Guiado

## Objetivo

Definir como o BrandOS deve coletar informações iniciais do usuário.

## Entrada necessária

O sistema deve coletar:

- nome da marca
- tipo de projeto
- segmento
- objetivo principal
- produto ou serviço
- público desejado
- região ou mercado de atuação
- concorrentes conhecidos
- referências visuais
- referências verbais
- restrições
- expectativas de entrega
- nível de maturidade do usuário

## Processo

O agente responsável deve:

1. Receber a ideia inicial do usuário
2. Identificar se é marca nova, redesign, marca pessoal, produto digital ou outro tipo
3. Fazer perguntas essenciais
4. Evitar excesso de perguntas de uma vez (máximo 3 a 5 por bloco)
5. Explicar o motivo das perguntas quando necessário
6. Organizar as respostas em um briefing estruturado
7. Sinalizar lacunas importantes
8. Preparar o material para as próximas etapas

## Saída esperada

Um briefing contendo:

- resumo do projeto
- tipo de marca
- segmento
- objetivo
- público inicial
- produto ou serviço
- diferenciais percebidos
- referências
- restrições
- dúvidas pendentes
- próximos passos recomendados

## Critérios de qualidade

O briefing deve ser:

- claro
- organizado
- suficiente para iniciar a estratégia
- sem excesso de complexidade
- adaptado ao nível do usuário

## O que evitar

- Fazer perguntas demais de uma vez
- Usar linguagem técnica sem explicação
- Bloquear o usuário por falta de informação
- Inventar respostas que o usuário não deu

## Template de saída

```md
# Briefing da Marca

## Nome da marca

## Tipo de projeto

## Segmento

## Objetivo principal

## Produto ou serviço

## Público inicial

## Diferenciais percebidos

## Referências

## Restrições

## Dúvidas pendentes

## Próximos passos
```

## Agente responsável

`discovery-agent` + `onboarding-agent`
