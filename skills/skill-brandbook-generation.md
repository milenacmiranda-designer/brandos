# Skill — Brandbook Generation

**Tipo:** Skill reutilizável  
**Usada por:** `export-agent`

---

## O que esta skill faz

Consolida todos os documentos gerados nas fases anteriores em um brand book final organizado, claro e pronto para uso.

---

## Quando usar

- Fase 13 (Export System)
- Após aprovação no Gate 12 (Governance + QA)
- Quando o usuário solicitar o brand book consolidado

---

## Pré-requisito

Esta skill só deve ser executada após:
- Gate 8 (Brand DNA) aprovado
- Gate 12 (Governance + QA) aprovado com score ≥ 70

---

## Processo

```
1. Verificar aprovação dos gates
2. Coletar todos os documentos gerados nas fases
3. Verificar consistência entre documentos
4. Organizar na estrutura padrão do brand book
5. Padronizar linguagem e formatação
6. Adicionar introdução e instruções de uso
7. Adicionar checklist de consistência
8. Gerar brand-system.md final
9. Atualizar arquivos de memória
10. Apresentar resumo executivo
```

---

## Estrutura do brand book

Ver estrutura completa em SPEC_10_BRAND_BOOK.md

---

## Saída

Um arquivo `brand-system.md` completo e organizado em `brandos-output/01-brand-system/`.

---

## Critérios de qualidade

- Todas as seções obrigatórias presentes
- Sem contradições entre seções
- Linguagem consistente ao longo do documento
- Diretrizes práticas (não apenas conceituais)
- Autoexplicativo — qualquer pessoa consegue usar sem orientação adicional

---

## O que evitar

- Gerar brand book sem aprovação dos gates
- Repetir conteúdo sem necessidade
- Seções vazias ou "em construção"
- Brand book longo demais que ninguém lê
- Misturar decisões estratégicas com sugestões não validadas
