# BrandOS — Product Requirements Document

> Este arquivo é o PRD oficial do BrandOS. Para a versão completa com specs e scaffold integrados, consulte `BRANDOS_PRD_SPECS_SCAFFOLD_COMPLETO.md`.

---

## Visão geral

O **BrandOS** é um sistema operacional de branding com IA, criado para conduzir o usuário por um processo completo de construção de marca.

Ele transforma uma ideia inicial, marca existente, marca pessoal, negócio local, produto digital ou app em um sistema de marca completo, organizado e aplicável.

---

## Problema que resolve

- falta de clareza estratégica
- marca criada apenas pela estética
- ausência de posicionamento
- público-alvo genérico
- personas superficiais
- tom de voz inconsistente
- identidade visual desconectada da estratégia
- falta de brand book
- dificuldade de conduzir um processo completo de branding

---

## Público-alvo

- empreendedores e donos de negócio
- designers e social medias
- criadores de conteúdo e marcas pessoais
- startups e produtos digitais
- pessoas criando uma marca do zero
- pessoas reformulando uma marca existente

---

## Funcionalidades obrigatórias

1. Identificar o tipo de projeto
2. Conduzir briefing guiado
3. Pesquisar mercado e concorrentes
4. Mapear público e personas
5. Definir posicionamento e proposta de valor
6. Criar personalidade de marca (Brand DNA)
7. Criar identidade verbal
8. Criar direção visual
9. Revisar coerência e qualidade (Gate QA)
10. Exportar brand book completo
11. Manter memória persistente entre fases
12. Adaptar ao nível do usuário (básico / intermediário / avançado)

---

## Funcionalidades opcionais

- Auditoria de marca existente
- Naming
- Tagline e manifesto
- UX + Product Experience (para produtos digitais)
- Production System (posts, copy, campanhas, prompts visuais)

---

## Feature: Key Visual & Direção de Aplicações

### Objetivo

Permitir que o BrandOS gere uma direção visual aplicada antes da criação de layouts finais, garantindo consistência entre estratégia, identidade visual e aplicações práticas.

### Problema que resolve

Evita que os layouts sejam gerados sem uma referência visual central, reduzindo inconsistência estética entre peças. Preenche a lacuna entre "cores e fontes definidas" e "layouts prontos" com uma imagem-mãe da marca.

### Posição no pipeline

Fase 10.5 — após Visual Identity (10) e antes de UX + Product Experience (11) e Propostas de Layout.

### Agente responsável

`key-visual-agent` com 6 subagentes especializados: composition, typography-application, color-application, image-direction, graphic-assets, application-system.

### Usuário beneficiado

Designers, empreendedores, criadores de marca, equipes de marketing e usuários não especialistas que precisam visualizar como a marca se comporta na prática.

### Resultado esperado

Arquivo `09-key-visual-direcao-aplicacoes.md` com conceito visual central, composição, tipografia aplicada, cor aplicada, imagem, grafismos, aplicações derivadas e checklist de consistência.

### Comando

`/gerar-key-visual`

### Comportamento quando pulado

Se o usuário pular esta fase, o sistema registra `key_visual.status = "skipped"` em `creative-memory.json` e avisa que os layouts serão gerados sem referência visual central.

### Integração

- **Propostas de Layout:** usa o Key Visual como referência base quando aprovado.
- **Swiss Editorial PDF (SPEC_15):** inclui seção "Key Visual & Direção de Aplicações".
- **Memória:** campo `key_visual` em `creative-memory.json`.

---

## Limites

O BrandOS não deve:

- prometer registro jurídico de marca
- substituir pesquisa no INPI
- afirmar dados de mercado sem sinalizar hipótese
- criar apenas logotipo sem estratégia
- gerar outputs genéricos
- avançar sem gates de qualidade

---

## Critérios de sucesso

O BrandOS é bem-sucedido quando entrega uma marca com:

- clareza estratégica
- público bem definido
- posicionamento consistente
- proposta de valor clara
- personalidade reconhecível
- tom de voz aplicável
- direção visual alinhada à estratégia
- brand book organizado e pronto para uso

---

## Arquitetura do sistema

Ver `docs/overview.md` para a visão geral da arquitetura.

Ver `specs/` para as especificações de cada fase.

Ver `BRANDOS_HARNESS.md` para regras, gates e critérios de qualidade.
