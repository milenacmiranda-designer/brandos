# Skill — Visual Direction

**Tipo:** Skill reutilizável  
**Usada por:** `visual-identity-agent`

---

## O que esta skill faz

Cria a direção visual conceitual da marca: conceito, paleta, tipografia, estilo e referências.

---

## Quando usar

- Fase 10 (Visual Identity)
- Após Brand DNA aprovado no Gate 8
- Quando a marca precisar de direção para designer ou ferramenta de criação

---

## O que esta skill cobre

| Elemento | O que define |
|----------|-------------|
| Conceito visual | A ideia central que orienta as escolhas |
| Atmosfera | Como a marca deve se sentir visualmente |
| Paleta de cores | Primária, secundária, acento, neutros |
| Tipografia | Famílias, uso, hierarquia |
| Estilo gráfico | Linguagem visual (minimalista, orgânico...) |
| Estilo fotográfico | Abordagem de imagem |
| Elementos visuais | Formas, texturas, padrões característicos |
| Referências | Moodboard conceitual descritivo |
| Prompts visuais | Para geração de imagem |

---

## Processo

```
1. Ler Brand DNA aprovado (personalidade, posicionamento, público)
2. Analisar pesquisa de concorrentes (o que evitar visualmente)
3. Definir conceito visual em uma frase
4. Definir atmosfera estética
5. Sugerir paleta (via color-palette-subagent)
6. Sugerir tipografia (via typography-subagent)
7. Definir estilo gráfico
8. Definir estilo fotográfico
9. Criar moodboard conceitual (via visual-references-subagent)
10. Gerar prompts visuais
```

---

## Saída

Ver template completo em SPEC_09_VISUAL_IDENTITY.md

---

## Critérios de qualidade

- Toda escolha visual deve ter justificativa estratégica
- Paleta deve ser diferenciada no segmento
- Tipografia deve ser legível nos canais principais
- Conceito deve ser específico (não "moderno e clean")
- Prompts visuais devem ser detalhados o suficiente para gerar imagens coerentes

---

## O que evitar

- Escolher estética por tendência sem conexão com a estratégia
- Visual bonito mas genérico para a categoria
- Paleta de 6+ cores sem hierarquia clara
- Direção visual que não se traduz em aplicações práticas
