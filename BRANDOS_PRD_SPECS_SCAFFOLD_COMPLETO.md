# BRANDOS — PRD, SPECS E SCAFFOLD COMPLETO

> Arquivo estrutural para integrar ao projeto BrandOS no Claude Code.
>
> Este documento define os fundamentos de produto, especificações, arquitetura de pastas, agentes, subagentes, skills, workflows, templates, outputs e regras de qualidade do BrandOS.

---

# 1. VISÃO GERAL DO BRANDOS

O **BrandOS** é um sistema operacional de branding com IA, criado para conduzir o usuário por um processo completo de construção de marca.

Ele deve transformar uma ideia inicial, marca existente, marca pessoal, negócio local, produto digital ou app em um sistema de marca completo, organizado e aplicável.

O BrandOS não deve funcionar apenas como um gerador de logotipo, slogan ou paleta de cores. Ele deve atuar como uma estrutura estratégica de criação de marca, conectando:

- diagnóstico;
- briefing;
- pesquisa;
- personas;
- posicionamento;
- proposta de valor;
- personalidade da marca;
- identidade verbal;
- identidade visual;
- brand book;
- materiais finais;
- revisão de consistência.

O sistema deve ser didático, organizado e adaptável ao nível de conhecimento do usuário.

Se o usuário for iniciante, o BrandOS deve explicar os conceitos de forma simples antes de executar cada etapa.

Se o usuário demonstrar mais maturidade em branding, marketing, UX, design ou negócios, o BrandOS pode aprofundar análises estratégicas e técnicas.

---

# 2. CONCEITOS FUNDAMENTAIS DO BRANDOS

A arquitetura do BrandOS deve ser baseada em três conceitos centrais:

1. **PRD — Product Requirements Document**
2. **Specs — Especificações funcionais e técnicas**
3. **Scaffold — Estrutura inicial do projeto**

Esses três elementos ajudam a transformar uma ideia solta em um projeto executável dentro do Claude Code.

---

# 3. PRD — PRODUCT REQUIREMENTS DOCUMENT

## 3.1. O que é PRD no BrandOS

O PRD é o documento de requisitos do produto.

No BrandOS, ele funciona como o documento-mãe do sistema. Ele define o que o BrandOS é, para quem ele existe, qual problema resolve, quais funcionalidades precisa ter, quais entregas deve gerar e quais limites precisa respeitar.

O PRD não é um documento técnico de código. Ele é um documento estratégico.

Ele serve para garantir que todos os agentes, subagentes, skills e workflows trabalhem na mesma direção.

---

## 3.2. Objetivo do PRD

O PRD deve responder:

- O que é o BrandOS?
- Para quem ele foi criado?
- Qual problema ele resolve?
- Quais tipos de marca ele consegue desenvolver?
- Quais etapas o sistema deve seguir?
- Quais entregáveis ele deve gerar?
- Quais funcionalidades são obrigatórias?
- Quais funcionalidades são opcionais?
- Quais limites o sistema deve respeitar?
- Como saber se a entrega final está boa?

---

## 3.3. Definição do produto

O BrandOS é um sistema guiado por IA para criação de marcas completas.

Ele conduz o usuário desde uma ideia inicial até a construção de um sistema de marca estruturado, incluindo estratégia, posicionamento, personas, universo verbal, identidade visual, diretrizes de uso e brand book final.

O BrandOS deve ser capaz de operar em diferentes cenários:

- criação de marca nova;
- redesign de marca existente;
- reposicionamento;
- marca pessoal;
- produto digital;
- aplicativo;
- negócio local;
- serviço profissional;
- infoproduto;
- startup;
- projeto experimental;
- projeto de portfólio;
- melhoria de identidade verbal;
- melhoria de identidade visual;
- criação de brand book para marca já existente.

---

## 3.4. Problema que o BrandOS resolve

Criar uma marca completa é um processo complexo.

Muitas pessoas começam apenas com uma ideia, um nome ou uma referência visual, mas não sabem como transformar isso em uma marca coerente.

Problemas comuns que o BrandOS deve resolver:

- falta de clareza estratégica;
- marca criada apenas pela estética;
- ausência de posicionamento;
- público-alvo genérico;
- personas superficiais;
- tom de voz inconsistente;
- identidade visual desconectada da estratégia;
- falta de brand book;
- materiais de marca espalhados;
- dificuldade de explicar a marca;
- dificuldade de aplicar a marca em canais reais;
- dificuldade de conduzir um processo completo de branding.

O BrandOS resolve esses problemas criando um fluxo guiado, estruturado e didático.

---

## 3.5. Público-alvo

O BrandOS pode atender:

- empreendedores;
- designers;
- social medias;
- criadores de conteúdo;
- profissionais autônomos;
- consultores;
- pequenos negócios;
- startups;
- marcas pessoais;
- produtores digitais;
- infoprodutores;
- profissionais de UX/UI;
- estudantes de design;
- pessoas criando um app;
- pessoas criando uma marca do zero;
- pessoas reformulando uma marca existente.

---

## 3.6. Nível de conhecimento do usuário

O BrandOS deve se adaptar ao nível do usuário.

### Usuário iniciante

Se o usuário não entende de branding, o sistema deve:

- explicar conceitos antes de aplicar;
- usar linguagem simples;
- dar exemplos;
- evitar jargões;
- fazer perguntas guiadas;
- oferecer caminhos prontos;
- mostrar o motivo de cada etapa.

### Usuário intermediário

Se o usuário demonstra algum conhecimento, o sistema deve:

- usar linguagem profissional, mas clara;
- aprofundar análises;
- permitir decisões mais estratégicas;
- oferecer alternativas;
- comparar caminhos possíveis.

### Usuário avançado

Se o usuário demonstra domínio de branding, design, marketing ou estratégia, o sistema deve:

- trabalhar com mais profundidade;
- usar frameworks;
- conectar decisões com mercado;
- questionar premissas;
- sugerir refinamentos;
- atuar como parceiro estratégico.

---

## 3.7. Objetivo principal

O objetivo principal do BrandOS é transformar uma ideia, marca ou projeto em um sistema completo de marca.

A entrega final deve conter:

- diagnóstico;
- briefing estruturado;
- análise de contexto;
- personas;
- posicionamento;
- proposta de valor;
- diferenciais;
- personalidade de marca;
- tom de voz;
- universo verbal;
- mensagens principais;
- direção visual;
- paleta de cores;
- tipografias sugeridas;
- estilo gráfico;
- estilo fotográfico;
- diretrizes de uso;
- brand book final;
- materiais opcionais de aplicação.

---

## 3.8. Funcionalidades obrigatórias

O BrandOS deve obrigatoriamente:

1. Identificar o tipo de projeto.
2. Conduzir um briefing inicial.
3. Explicar as etapas de forma didática.
4. Diagnosticar o contexto da marca.
5. Mapear público e personas.
6. Definir posicionamento.
7. Criar proposta de valor.
8. Definir personalidade de marca.
9. Criar identidade verbal.
10. Criar direção visual.
11. Organizar um brand book.
12. Revisar coerência entre estratégia, verbal e visual.
13. Gerar outputs finais em Markdown.
14. Manter consistência entre todas as entregas.

---

## 3.9. Funcionalidades opcionais

O BrandOS também pode gerar, quando solicitado:

- naming;
- tagline;
- slogan;
- manifesto;
- bio para Instagram;
- bio para LinkedIn;
- roteiro de apresentação da marca;
- pitch comercial;
- landing page conceitual;
- posts para redes sociais;
- calendário de conteúdo;
- guia de Instagram;
- guia de LinkedIn;
- apresentação institucional;
- roteiro de vídeo;
- prompts para geração de imagens;
- moodboard conceitual;
- moodboard visual;
- checklist de lançamento;
- plano de campanha;
- guia de aplicação em materiais físicos;
- guia de aplicação em produto digital.

---

## 3.10. Limites do BrandOS

O BrandOS não deve:

- prometer registro jurídico de marca;
- substituir pesquisa no INPI;
- garantir exclusividade de nome;
- afirmar dados de mercado sem fonte ou sem sinalizar hipótese;
- criar apenas logotipo sem estratégia;
- pular etapas fundamentais;
- entregar respostas genéricas;
- usar jargões sem explicar;
- criar personas clichês;
- gerar posicionamentos vagos;
- criar identidade visual desconectada do público;
- tratar branding apenas como estética;
- fingir que executou pesquisa real quando não pesquisou;
- gerar materiais finais sem revisão de consistência.

---

## 3.11. Critérios de sucesso

O BrandOS será considerado bem-sucedido quando entregar uma marca com:

- clareza estratégica;
- público bem definido;
- personas úteis;
- posicionamento consistente;
- proposta de valor clara;
- diferenciais reais ou plausíveis;
- personalidade reconhecível;
- tom de voz aplicável;
- universo verbal coerente;
- direção visual alinhada à estratégia;
- brand book organizado;
- diretrizes fáceis de usar;
- outputs finais claros;
- revisão de consistência.

---

# 4. SPECS — ESPECIFICAÇÕES DO BRANDOS

## 4.1. O que são Specs no BrandOS

Specs são documentos de especificação.

No BrandOS, cada Spec define como uma parte específica do sistema deve funcionar.

Enquanto o PRD define o produto como um todo, as Specs detalham módulos, etapas, agentes, subagentes, skills e entregáveis.

As Specs evitam que a IA trabalhe de forma vaga ou improvisada.

---

## 4.2. Estrutura padrão de uma Spec

Toda Spec do BrandOS deve conter:

```md
# SPEC — Nome da Etapa

## Objetivo
Explicar o objetivo da etapa.

## Entrada necessária
Listar quais informações essa etapa precisa receber.

## Processo
Explicar o passo a passo que o agente deve seguir.

## Saída esperada
Definir exatamente o que deve ser entregue.

## Critérios de qualidade
Definir como avaliar se a entrega ficou boa.

## O que evitar
Listar erros, excessos e comportamentos proibidos.

## Template de saída
Fornecer uma estrutura de resposta padronizada.
```

---

## 4.3. Lista de Specs recomendadas

```txt
specs/
├── SPEC_00_OVERVIEW.md
├── SPEC_01_BRIEFING.md
├── SPEC_02_BRAND_AUDIT.md
├── SPEC_03_RESEARCH.md
├── SPEC_04_PERSONAS.md
├── SPEC_05_POSITIONING.md
├── SPEC_06_VALUE_PROPOSITION.md
├── SPEC_07_BRAND_PERSONALITY.md
├── SPEC_08_VERBAL_IDENTITY.md
├── SPEC_09_VISUAL_IDENTITY.md
├── SPEC_10_BRAND_BOOK.md
├── SPEC_11_OUTPUTS.md
├── SPEC_12_REVIEW.md
└── SPEC_13_EXPORT.md
```

---

# SPEC_00_OVERVIEW — Visão Geral do Sistema

## Objetivo

Explicar a lógica geral do BrandOS e como todas as partes se conectam.

## Entrada necessária

- PRD do BrandOS;
- lista de workflows;
- lista de agentes;
- lista de skills;
- estrutura de outputs.

## Processo

Esta Spec deve organizar:

1. a visão geral do sistema;
2. a relação entre PRD, Specs e Scaffold;
3. a relação entre agentes e workflows;
4. a relação entre skills e entregas;
5. as regras globais de funcionamento;
6. o padrão de qualidade esperado.

## Saída esperada

Uma visão geral clara da arquitetura do BrandOS.

## Critérios de qualidade

A visão geral deve ser:

- fácil de entender;
- organizada;
- completa;
- compatível com o uso no Claude Code;
- útil para orientar futuras alterações.

---

# SPEC_01_BRIEFING — Briefing Guiado

## Objetivo

Definir como o BrandOS deve coletar informações iniciais do usuário.

## Entrada necessária

O sistema deve coletar:

- nome da marca;
- tipo de projeto;
- segmento;
- objetivo principal;
- produto ou serviço;
- público desejado;
- região ou mercado de atuação;
- concorrentes conhecidos;
- referências visuais;
- referências verbais;
- restrições;
- expectativas de entrega;
- nível de maturidade do usuário.

## Processo

O agente responsável deve:

1. Receber a ideia inicial do usuário.
2. Identificar se é marca nova, redesign, marca pessoal, produto digital ou outro tipo.
3. Fazer perguntas essenciais.
4. Evitar excesso de perguntas de uma vez.
5. Explicar o motivo das perguntas quando necessário.
6. Organizar as respostas em um briefing estruturado.
7. Sinalizar lacunas importantes.
8. Preparar o material para as próximas etapas.

## Saída esperada

Um briefing contendo:

- resumo do projeto;
- tipo de marca;
- segmento;
- objetivo;
- público inicial;
- produto ou serviço;
- diferenciais percebidos;
- referências;
- restrições;
- dúvidas pendentes;
- próximos passos recomendados.

## Critérios de qualidade

O briefing deve ser:

- claro;
- organizado;
- suficiente para iniciar a estratégia;
- sem excesso de complexidade;
- adaptado ao nível do usuário.

## O que evitar

- Fazer perguntas demais de uma vez.
- Usar linguagem técnica sem explicação.
- Bloquear o usuário por falta de informação.
- Inventar respostas que o usuário não deu.

---

# SPEC_02_BRAND_AUDIT — Auditoria de Marca

## Objetivo

Analisar uma marca existente quando o projeto for redesign, reposicionamento ou melhoria.

## Entrada necessária

- nome da marca;
- materiais atuais;
- site;
- redes sociais;
- identidade visual atual;
- tom de voz atual;
- percepção desejada;
- problemas percebidos;
- objetivos de mudança.

## Processo

O agente deve avaliar:

1. clareza da proposta;
2. consistência visual;
3. consistência verbal;
4. adequação ao público;
5. força do posicionamento;
6. diferenciação;
7. percepção de valor;
8. oportunidades de melhoria.

## Saída esperada

Um diagnóstico com:

- pontos fortes;
- pontos fracos;
- inconsistências;
- riscos;
- oportunidades;
- recomendações iniciais;
- prioridades de ajuste.

## Critérios de qualidade

A auditoria deve ser:

- objetiva;
- útil;
- estratégica;
- respeitosa;
- acionável.

## O que evitar

- Criticar sem explicar.
- Fazer julgamento puramente estético.
- Ignorar o objetivo do negócio.
- Sugerir mudanças sem justificativa.

---

# SPEC_03_RESEARCH — Pesquisa e Contexto

## Objetivo

Orientar a análise de mercado, categoria, concorrência e referências.

## Entrada necessária

- segmento;
- categoria;
- localização;
- público-alvo;
- concorrentes conhecidos;
- referências desejadas;
- proposta do negócio.

## Processo

O agente deve mapear:

1. contexto da categoria;
2. padrões visuais do mercado;
3. padrões verbais do mercado;
4. concorrentes diretos;
5. concorrentes indiretos;
6. oportunidades de diferenciação;
7. riscos de parecer genérico;
8. tendências relevantes, quando aplicável.

## Saída esperada

Uma síntese estratégica contendo:

- panorama do mercado;
- códigos da categoria;
- oportunidades;
- ameaças;
- lacunas de posicionamento;
- referências úteis;
- implicações para a marca.

## Critérios de qualidade

A pesquisa deve ser:

- contextual;
- objetiva;
- conectada à estratégia;
- útil para orientar posicionamento e identidade.

## O que evitar

- Inventar dados como se fossem fatos.
- Fazer pesquisa superficial.
- Copiar concorrentes.
- Recomendar tendências sem relação com a marca.

---

# SPEC_04_PERSONAS — Personas

## Objetivo

Criar personas estratégicas para orientar comunicação, posicionamento e identidade visual.

## Entrada necessária

- segmento;
- produto ou serviço;
- público desejado;
- faixa de preço;
- região;
- objetivo da marca;
- estilo de comunicação pretendido;
- contexto de mercado.

## Processo

O agente deve:

1. Analisar o briefing.
2. Identificar perfis relevantes de público.
3. Separar público primário e secundário.
4. Criar de 2 a 4 personas.
5. Diferenciar claramente cada persona.
6. Conectar personas às decisões de marca.
7. Gerar implicações para comunicação e visual.

## Saída esperada

Cada persona deve conter:

- nome fictício;
- idade aproximada;
- profissão ou contexto;
- estilo de vida;
- dores;
- desejos;
- medos;
- objeções;
- motivações;
- comportamento de compra;
- canais de comunicação;
- linguagem que utiliza;
- o que espera da marca;
- como a marca deve se comunicar com ela.

## Critérios de qualidade

As personas devem ser:

- realistas;
- úteis;
- coerentes com o segmento;
- não genéricas;
- diferentes entre si;
- conectadas ao posicionamento.

## O que evitar

- Personas clichês.
- Personas sem utilidade prática.
- Personas desconectadas do produto.
- Excesso de detalhes irrelevantes.

---

# SPEC_05_POSITIONING — Posicionamento

## Objetivo

Definir o posicionamento estratégico da marca.

## Entrada necessária

- briefing;
- personas;
- contexto de mercado;
- diferenciais;
- objetivo do negócio;
- percepção desejada;
- proposta de valor inicial.

## Processo

O agente deve definir:

1. categoria da marca;
2. público prioritário;
3. principal promessa;
4. benefício central;
5. diferenciais;
6. razão para acreditar;
7. território de marca;
8. inimigo conceitual;
9. posicionamento central.

## Saída esperada

A entrega deve conter:

- declaração de posicionamento;
- território de marca;
- diferencial competitivo;
- promessa central;
- razão para acreditar;
- frase de posicionamento;
- explicação estratégica;
- implicações para comunicação;
- implicações para identidade visual.

## Template de posicionamento

```md
A marca se posiciona como [categoria] para [público], oferecendo [benefício principal], por meio de [diferencial], para gerar [resultado desejado].
```

## Critérios de qualidade

O posicionamento deve ser:

- claro;
- específico;
- defensável;
- relevante para o público;
- coerente com o mercado;
- aplicável na comunicação.

## O que evitar

- Frases genéricas.
- Promessas vazias.
- Diferenciais que qualquer concorrente poderia usar.
- Posicionamento baseado apenas em estética.

---

# SPEC_06_VALUE_PROPOSITION — Proposta de Valor

## Objetivo

Criar uma proposta de valor clara, diferenciada e aplicável.

## Entrada necessária

- dor principal do público;
- solução oferecida;
- benefícios funcionais;
- benefícios emocionais;
- diferenciais;
- provas de valor;
- objeções.

## Processo

O agente deve identificar:

1. problema principal;
2. transformação prometida;
3. benefício central;
4. valor percebido;
5. diferenciais;
6. argumentos de confiança;
7. mensagens de apoio.

## Saída esperada

A entrega deve conter:

- proposta de valor principal;
- versão curta;
- versão expandida;
- benefícios funcionais;
- benefícios emocionais;
- provas de valor;
- mensagens de apoio;
- variações para canais diferentes.

## Critérios de qualidade

A proposta de valor deve ser:

- simples;
- clara;
- desejável;
- confiável;
- conectada ao público;
- conectada ao produto ou serviço.

## O que evitar

- Prometer demais.
- Usar frases abstratas.
- Criar uma proposta que não se diferencia.
- Ignorar objeções do público.

---

# SPEC_07_BRAND_PERSONALITY — Personalidade da Marca

## Objetivo

Definir a personalidade da marca, seus atributos, energia e comportamento.

## Entrada necessária

- posicionamento;
- personas;
- segmento;
- tipo de marca;
- percepção desejada;
- referências;
- tom desejado.

## Processo

O agente deve definir:

1. arquétipo dominante;
2. arquétipo secundário, se necessário;
3. atributos principais;
4. energia da marca;
5. postura comunicacional;
6. características humanas;
7. limites de comportamento.

## Saída esperada

A entrega deve conter:

- personalidade central;
- 3 a 5 atributos principais;
- arquétipo dominante;
- arquétipo secundário, se fizer sentido;
- como a marca se comporta;
- como a marca não deve se comportar;
- exemplos práticos de atitude da marca.

## Critérios de qualidade

A personalidade deve ser:

- coerente;
- memorável;
- aplicável;
- conectada ao posicionamento;
- útil para orientar linguagem e visual.

## O que evitar

- Atributos demais.
- Atributos contraditórios.
- Arquétipos escolhidos sem justificativa.
- Personalidade sem aplicação prática.

---

# SPEC_08_VERBAL_IDENTITY — Identidade Verbal

## Objetivo

Criar o universo verbal da marca.

## Entrada necessária

- posicionamento;
- proposta de valor;
- personas;
- personalidade;
- segmento;
- canais de comunicação;
- referências verbais.

## Processo

O agente deve criar:

1. tom de voz;
2. vocabulário da marca;
3. palavras que a marca usa;
4. palavras que a marca evita;
5. mensagens principais;
6. slogan, tagline ou assinatura verbal, se necessário;
7. manifesto;
8. bio curta;
9. bio longa;
10. exemplos de comunicação.

## Saída esperada

A entrega deve conter:

- tom de voz;
- guia de linguagem;
- vocabulário recomendado;
- vocabulário proibido ou evitado;
- frases exemplo;
- mensagens-chave;
- narrativa da marca;
- manifesto;
- assinatura verbal;
- aplicações por canal.

## Critérios de qualidade

A identidade verbal deve ser:

- coerente com a estratégia;
- natural;
- diferenciada;
- aplicável;
- fácil de replicar;
- alinhada ao público.

## O que evitar

- Tom artificial.
- Frases genéricas.
- Linguagem desconectada das personas.
- Manifesto exagerado sem relação com a marca.

---

# SPEC_09_VISUAL_IDENTITY — Identidade Visual Conceitual

## Objetivo

Criar a direção visual conceitual da marca.

## Entrada necessária

- posicionamento;
- personalidade;
- personas;
- segmento;
- referências;
- restrições visuais;
- percepção desejada;
- canais de aplicação.

## Processo

O agente deve definir:

1. conceito visual;
2. atmosfera estética;
3. paleta de cores;
4. tipografias sugeridas;
5. estilo gráfico;
6. estilo fotográfico;
7. elementos visuais;
8. grid ou composição;
9. aplicações principais.

## Saída esperada

A entrega deve conter:

- direção visual;
- justificativa estratégica;
- paleta sugerida;
- tipografias sugeridas;
- estilo de imagem;
- elementos gráficos;
- referências conceituais;
- recomendações de aplicação.

## Critérios de qualidade

A direção visual deve:

- traduzir a estratégia;
- conversar com o público;
- diferenciar a marca;
- ser aplicável em canais reais;
- evitar escolhas aleatórias;
- explicar o motivo de cada decisão.

## O que evitar

- Escolher cores apenas por gosto pessoal.
- Sugerir fontes sem justificativa.
- Criar uma estética desconectada da marca.
- Copiar referências diretamente.

---

# SPEC_10_BRAND_BOOK — Brand Book

## Objetivo

Organizar todos os elementos da marca em um documento final.

## Entrada necessária

- briefing final;
- diagnóstico;
- personas;
- posicionamento;
- proposta de valor;
- personalidade;
- identidade verbal;
- identidade visual;
- diretrizes;
- aplicações.

## Estrutura recomendada

O brand book deve conter:

1. Introdução
2. Sobre a marca
3. Essência da marca
4. Público-alvo
5. Personas
6. Posicionamento
7. Proposta de valor
8. Personalidade
9. Identidade verbal
10. Identidade visual
11. Paleta de cores
12. Tipografia
13. Elementos gráficos
14. Estilo fotográfico
15. Aplicações
16. Regras de uso
17. Checklist de consistência

## Saída esperada

Um documento final em Markdown, claro, organizado e pronto para ser usado como guia de marca.

## Critérios de qualidade

O brand book deve ser:

- completo;
- claro;
- bem organizado;
- coerente;
- aplicável;
- fácil de consultar.

## O que evitar

- Repetir informações sem necessidade.
- Misturar estratégia com sugestões soltas.
- Criar um documento bonito, mas pouco útil.
- Ignorar diretrizes práticas de uso.

---

# SPEC_11_OUTPUTS — Entregáveis

## Objetivo

Definir quais entregáveis o BrandOS pode gerar ao final do processo.

## Entregáveis principais

- Brand Book
- Estratégia da marca
- Guia verbal
- Guia visual
- Personas
- Posicionamento
- Proposta de valor
- Mensagens principais
- Diretrizes de aplicação

## Entregáveis opcionais

- calendário de conteúdo;
- posts para Instagram;
- posts para LinkedIn;
- pitch comercial;
- landing page conceitual;
- apresentação institucional;
- roteiro de vídeo;
- prompts para imagens;
- guia de campanha;
- plano de lançamento;
- naming;
- tagline;
- manifesto;
- guia de tom de voz;
- manual de aplicação.

## Critérios de qualidade

Os outputs devem ser:

- claros;
- organizados;
- úteis;
- compatíveis entre si;
- prontos para consulta;
- nomeados corretamente.

---

# SPEC_12_REVIEW — Revisão de Qualidade

## Objetivo

Definir como o BrandOS deve revisar a qualidade das entregas.

## Processo

O agente deve verificar:

1. coerência entre briefing e estratégia;
2. coerência entre personas e posicionamento;
3. clareza da proposta de valor;
4. coerência entre personalidade e tom de voz;
5. coerência entre verbal e visual;
6. ausência de contradições;
7. profundidade estratégica;
8. aplicabilidade prática;
9. qualidade da linguagem;
10. utilidade dos entregáveis.

## Saída esperada

Uma revisão contendo:

- pontos fortes;
- pontos a melhorar;
- inconsistências encontradas;
- sugestões de refinamento;
- checklist final;
- recomendação de aprovação ou ajuste.

## Critérios de qualidade

A revisão deve ser:

- honesta;
- objetiva;
- construtiva;
- acionável;
- conectada ao objetivo da marca.

---

# SPEC_13_EXPORT — Exportação

## Objetivo

Definir como o BrandOS deve organizar os arquivos finais.

## Saída esperada

O sistema deve gerar ou organizar:

```txt
outputs/
├── 01-briefing.md
├── 02-audit.md
├── 03-research.md
├── 04-personas.md
├── 05-positioning.md
├── 06-value-proposition.md
├── 07-brand-personality.md
├── 08-verbal-identity.md
├── 09-visual-identity.md
├── 10-brand-book.md
├── 11-content-guide.md
└── 12-final-summary.md
```

## Regras

Os arquivos finais devem:

- ter nomes claros;
- seguir ordem lógica;
- evitar duplicidade;
- manter linguagem consistente;
- respeitar o PRD;
- respeitar as Specs;
- ser fáceis de localizar.

---

# 5. SCAFFOLD DO PROJETO BRANDOS

## 5.1. O que é Scaffold no BrandOS

Scaffold é a estrutura inicial de pastas e arquivos do projeto.

Ele funciona como o esqueleto do BrandOS.

Enquanto o PRD define a visão e as Specs detalham o funcionamento, o Scaffold define onde cada coisa fica organizada.

Sem Scaffold, o projeto pode virar um conjunto de arquivos soltos.

Com Scaffold, o projeto fica modular, escalável e pronto para uso no Claude Code.

---

## 5.2. Estrutura recomendada

```txt
brandos/
├── README.md
├── PRD.md
├── BRANDOS_HARNESS.md
├── CHANGELOG.md
├── docs/
│   ├── overview.md
│   ├── glossary.md
│   ├── usage-guide.md
│   └── concepts.md
├── specs/
│   ├── SPEC_00_OVERVIEW.md
│   ├── SPEC_01_BRIEFING.md
│   ├── SPEC_02_BRAND_AUDIT.md
│   ├── SPEC_03_RESEARCH.md
│   ├── SPEC_04_PERSONAS.md
│   ├── SPEC_05_POSITIONING.md
│   ├── SPEC_06_VALUE_PROPOSITION.md
│   ├── SPEC_07_BRAND_PERSONALITY.md
│   ├── SPEC_08_VERBAL_IDENTITY.md
│   ├── SPEC_09_VISUAL_IDENTITY.md
│   ├── SPEC_10_BRAND_BOOK.md
│   ├── SPEC_11_OUTPUTS.md
│   ├── SPEC_12_REVIEW.md
│   └── SPEC_13_EXPORT.md
├── agents/
│   ├── 01-discovery-agent.md
│   ├── 02-audit-agent.md
│   ├── 03-research-agent.md
│   ├── 04-persona-agent.md
│   ├── 05-positioning-agent.md
│   ├── 06-value-proposition-agent.md
│   ├── 07-brand-personality-agent.md
│   ├── 08-verbal-identity-agent.md
│   ├── 09-visual-identity-agent.md
│   ├── 10-brandbook-agent.md
│   └── 11-review-agent.md
├── subagents/
│   ├── naming-subagent.md
│   ├── tagline-subagent.md
│   ├── competitor-analysis-subagent.md
│   ├── audience-insight-subagent.md
│   ├── tone-of-voice-subagent.md
│   ├── manifesto-subagent.md
│   ├── color-palette-subagent.md
│   ├── typography-subagent.md
│   └── visual-references-subagent.md
├── skills/
│   ├── skill-briefing-analysis.md
│   ├── skill-brand-audit.md
│   ├── skill-market-research.md
│   ├── skill-persona-generation.md
│   ├── skill-positioning.md
│   ├── skill-value-proposition.md
│   ├── skill-brand-personality.md
│   ├── skill-verbal-identity.md
│   ├── skill-visual-direction.md
│   ├── skill-brandbook-generation.md
│   └── skill-quality-review.md
├── workflows/
│   ├── brandos-main-workflow.md
│   ├── brandos-new-brand-workflow.md
│   ├── brandos-rebrand-workflow.md
│   ├── brandos-personal-brand-workflow.md
│   ├── brandos-digital-product-workflow.md
│   └── brandos-review-workflow.md
├── prompts/
│   ├── system-prompt.md
│   ├── onboarding-prompt.md
│   ├── briefing-prompt.md
│   ├── audit-prompt.md
│   ├── research-prompt.md
│   ├── strategy-prompt.md
│   ├── verbal-prompt.md
│   ├── visual-prompt.md
│   ├── review-prompt.md
│   └── export-prompt.md
├── templates/
│   ├── briefing-template.md
│   ├── audit-template.md
│   ├── research-template.md
│   ├── persona-template.md
│   ├── positioning-template.md
│   ├── value-proposition-template.md
│   ├── verbal-identity-template.md
│   ├── visual-identity-template.md
│   ├── brand-book-template.md
│   └── final-summary-template.md
├── examples/
│   ├── example-new-brand.md
│   ├── example-rebrand.md
│   ├── example-personal-brand.md
│   ├── example-digital-product.md
│   └── example-track-running.md
├── tests/
│   ├── test-new-brand.md
│   ├── test-rebrand.md
│   ├── test-personal-brand.md
│   ├── test-digital-product.md
│   └── test-quality-review.md
└── outputs/
    ├── .gitkeep
    └── README.md
```

---

# 6. FUNÇÃO DE CADA PASTA

## 6.1. Raiz do projeto

A raiz contém os arquivos centrais:

```txt
README.md
PRD.md
BRANDOS_HARNESS.md
CHANGELOG.md
```

### README.md

Explica o que é o BrandOS, como usar, quais comandos existem e como o projeto está organizado.

### PRD.md

Define a visão geral do produto, público, problema, objetivos, funcionalidades, limites e critérios de sucesso.

### BRANDOS_HARNESS.md

Arquivo central de orquestração.

Ele define:

- comportamento geral do sistema;
- regras globais;
- como agentes devem operar;
- como workflows devem ser executados;
- como outputs devem ser gerados;
- como revisar qualidade.

### CHANGELOG.md

Registra mudanças, melhorias e versões do projeto.

---

## 6.2. docs/

Contém documentação complementar:

- visão geral;
- glossário;
- guia de uso;
- conceitos importantes;
- instruções para manutenção.

---

## 6.3. specs/

Contém as especificações.

Cada arquivo explica como uma etapa deve funcionar.

---

## 6.4. agents/

Contém os agentes principais.

Cada agente executa uma fase importante do processo.

---

## 6.5. subagents/

Contém agentes menores e especializados.

Eles ajudam os agentes principais em tarefas pontuais.

---

## 6.6. skills/

Contém habilidades reutilizáveis.

Uma skill pode ser usada por vários agentes.

---

## 6.7. workflows/

Contém a ordem de execução do sistema.

Cada workflow define uma jornada específica.

---

## 6.8. prompts/

Contém prompts-base para orientar o comportamento da IA.

---

## 6.9. templates/

Contém modelos de saída para padronizar entregáveis.

---

## 6.10. examples/

Contém exemplos de uso do BrandOS.

---

## 6.11. tests/

Contém casos de teste para validar o funcionamento do sistema.

---

## 6.12. outputs/

Contém os arquivos finais gerados pelo BrandOS.

---

# 7. AGENTES PRINCIPAIS DO BRANDOS

## 7.1. Discovery Agent

Responsável por entender a ideia inicial do usuário e transformar informações soltas em briefing organizado.

### Responsabilidades

- identificar tipo de projeto;
- fazer perguntas essenciais;
- organizar briefing;
- detectar lacunas;
- preparar entrada para as próximas etapas.

---

## 7.2. Audit Agent

Responsável por auditar marcas existentes.

### Responsabilidades

- avaliar identidade atual;
- identificar inconsistências;
- mapear pontos fortes e fracos;
- sugerir prioridades de melhoria.

---

## 7.3. Research Agent

Responsável por analisar mercado, categoria, concorrentes e referências.

### Responsabilidades

- mapear contexto;
- identificar códigos da categoria;
- analisar concorrentes;
- encontrar oportunidades de diferenciação.

---

## 7.4. Persona Agent

Responsável por criar personas estratégicas.

### Responsabilidades

- analisar público;
- criar personas;
- definir dores, desejos e objeções;
- conectar personas à estratégia.

---

## 7.5. Positioning Agent

Responsável por definir o posicionamento da marca.

### Responsabilidades

- definir território;
- criar declaração de posicionamento;
- identificar diferenciais;
- conectar posicionamento ao público.

---

## 7.6. Value Proposition Agent

Responsável por criar a proposta de valor.

### Responsabilidades

- identificar dor principal;
- definir benefício central;
- criar versões da proposta;
- conectar valor percebido e diferenciação.

---

## 7.7. Brand Personality Agent

Responsável por definir personalidade, arquétipos e atributos.

### Responsabilidades

- definir arquétipo dominante;
- selecionar atributos principais;
- definir comportamento da marca;
- orientar verbal e visual.

---

## 7.8. Verbal Identity Agent

Responsável por criar o universo verbal.

### Responsabilidades

- definir tom de voz;
- criar vocabulário;
- criar mensagens-chave;
- criar manifesto;
- criar bios e frases de aplicação.

---

## 7.9. Visual Identity Agent

Responsável por criar direção visual conceitual.

### Responsabilidades

- definir conceito visual;
- sugerir paleta;
- sugerir tipografia;
- definir estilo gráfico;
- orientar aplicações.

---

## 7.10. Brandbook Agent

Responsável por montar o brand book final.

### Responsabilidades

- consolidar entregas;
- organizar documento final;
- garantir clareza;
- estruturar diretrizes.

---

## 7.11. Review Agent

Responsável por revisar a qualidade e consistência do sistema.

### Responsabilidades

- verificar coerência;
- encontrar contradições;
- sugerir ajustes;
- validar qualidade final.

---

# 8. SUBAGENTES DO BRANDOS

Subagentes são especialistas menores que ajudam em tarefas específicas.

## Naming Subagent

Ajuda a criar nomes de marca.

## Tagline Subagent

Ajuda a criar slogans, taglines e assinaturas verbais.

## Competitor Analysis Subagent

Ajuda a analisar concorrentes diretos e indiretos.

## Audience Insight Subagent

Ajuda a encontrar insights de público.

## Tone of Voice Subagent

Ajuda a refinar o tom de voz.

## Manifesto Subagent

Ajuda a criar manifestos de marca.

## Color Palette Subagent

Ajuda a sugerir paletas coerentes.

## Typography Subagent

Ajuda a sugerir direções tipográficas.

## Visual References Subagent

Ajuda a organizar referências visuais e moodboard conceitual.

---

# 9. SKILLS DO BRANDOS

Skills são capacidades reutilizáveis.

Uma skill não é necessariamente uma etapa inteira. Ela é uma habilidade que pode ser usada por diferentes agentes.

## Skill Briefing Analysis

Analisa briefing e identifica informações importantes.

## Skill Brand Audit

Avalia marcas existentes.

## Skill Market Research

Mapeia contexto, mercado e concorrentes.

## Skill Persona Generation

Cria personas úteis para decisões de marca.

## Skill Positioning

Ajuda a criar posicionamento estratégico.

## Skill Value Proposition

Ajuda a formular proposta de valor.

## Skill Brand Personality

Define personalidade, atributos e arquétipos.

## Skill Verbal Identity

Cria tom de voz, mensagens e universo verbal.

## Skill Visual Direction

Cria direção visual conceitual.

## Skill Brandbook Generation

Organiza o brand book final.

## Skill Quality Review

Revisa coerência e qualidade das entregas.

---

# 10. WORKFLOWS DO BRANDOS

## 10.1. Main Workflow

Fluxo principal do BrandOS.

```txt
entrada do usuário
↓
identificação do tipo de projeto
↓
briefing
↓
diagnóstico ou pesquisa
↓
personas
↓
posicionamento
↓
proposta de valor
↓
personalidade
↓
identidade verbal
↓
identidade visual
↓
brand book
↓
revisão
↓
exportação
```

---

## 10.2. New Brand Workflow

Usado para criação de marca nova.

```txt
briefing inicial
↓
pesquisa de contexto
↓
personas
↓
posicionamento
↓
proposta de valor
↓
personalidade
↓
identidade verbal
↓
identidade visual
↓
brand book
↓
outputs finais
```

---

## 10.3. Rebrand Workflow

Usado para redesign ou reposicionamento.

```txt
briefing
↓
auditoria da marca atual
↓
diagnóstico
↓
pesquisa de mercado
↓
reposicionamento
↓
identidade verbal revisada
↓
identidade visual revisada
↓
brand book atualizado
↓
plano de transição
```

---

## 10.4. Personal Brand Workflow

Usado para marca pessoal.

```txt
história da pessoa
↓
objetivo profissional
↓
público de interesse
↓
posicionamento pessoal
↓
autoridade e diferenciais
↓
tom de voz
↓
identidade visual pessoal
↓
guia de conteúdo
↓
brand book pessoal
```

---

## 10.5. Digital Product Workflow

Usado para app, SaaS, infoproduto ou produto digital.

```txt
problema do usuário
↓
proposta do produto
↓
público-alvo
↓
mercado e concorrentes
↓
posicionamento
↓
proposta de valor
↓
identidade verbal
↓
identidade visual
↓
experiência de marca
↓
brand book do produto
```

---

## 10.6. Review Workflow

Usado para revisão final.

```txt
ler entregas
↓
verificar coerência
↓
identificar contradições
↓
avaliar clareza
↓
avaliar aplicabilidade
↓
sugerir melhorias
↓
gerar checklist final
```

---

# 11. TEMPLATES DE SAÍDA

## 11.1. Template de Briefing

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

---

## 11.2. Template de Persona

```md
# Persona

## Nome fictício

## Idade aproximada

## Contexto

## Objetivos

## Dores

## Desejos

## Medos

## Objeções

## Comportamento de compra

## Canais de comunicação

## Linguagem que utiliza

## Como a marca deve se comunicar com ela
```

---

## 11.3. Template de Posicionamento

```md
# Posicionamento da Marca

## Categoria

## Público prioritário

## Promessa central

## Diferencial

## Razão para acreditar

## Território de marca

## Declaração de posicionamento

## Implicações para comunicação

## Implicações para visual
```

---

## 11.4. Template de Identidade Verbal

```md
# Identidade Verbal

## Tom de voz

## Personalidade verbal

## Palavras que a marca usa

## Palavras que a marca evita

## Mensagens principais

## Tagline ou assinatura verbal

## Manifesto

## Bio curta

## Bio longa

## Exemplos de comunicação
```

---

## 11.5. Template de Identidade Visual

```md
# Identidade Visual Conceitual

## Conceito visual

## Atmosfera estética

## Paleta de cores sugerida

## Tipografias sugeridas

## Estilo gráfico

## Estilo fotográfico

## Elementos visuais

## Aplicações recomendadas

## Justificativa estratégica
```

---

## 11.6. Template de Brand Book

```md
# Brand Book

## 1. Introdução

## 2. Sobre a marca

## 3. Essência da marca

## 4. Público-alvo

## 5. Personas

## 6. Posicionamento

## 7. Proposta de valor

## 8. Personalidade

## 9. Identidade verbal

## 10. Identidade visual

## 11. Paleta de cores

## 12. Tipografia

## 13. Elementos gráficos

## 14. Estilo fotográfico

## 15. Aplicações

## 16. Regras de uso

## 17. Checklist de consistência
```

---

# 12. REGRAS GLOBAIS DO BRANDOS

## 12.1. Regra de clareza

O BrandOS deve sempre explicar o que está fazendo e por que aquela etapa importa.

## 12.2. Regra de adaptação

O sistema deve adaptar a profundidade conforme o nível do usuário.

## 12.3. Regra de consistência

Todas as entregas devem conversar entre si.

## 12.4. Regra de não genericidade

O BrandOS deve evitar respostas genéricas e clichês.

## 12.5. Regra de justificativa

Toda decisão importante deve ser justificada.

## 12.6. Regra de aplicabilidade

Toda entrega deve poder ser usada na prática.

## 12.7. Regra de revisão

Antes de finalizar, o sistema deve revisar coerência e qualidade.

## 12.8. Regra de organização

Os outputs devem ser organizados em arquivos claros e nomeados corretamente.

---

# 13. RELAÇÃO ENTRE PRD, SPECS, SCAFFOLD, AGENTES E OUTPUTS

O BrandOS deve seguir esta lógica:

```txt
PRD
↓
Specs
↓
Scaffold
↓
Agents
↓
Subagents
↓
Skills
↓
Workflows
↓
Templates
↓
Outputs
↓
Review
```

## PRD

Define o que o BrandOS é.

## Specs

Definem como cada parte funciona.

## Scaffold

Define onde cada arquivo fica.

## Agents

Executam as etapas principais.

## Subagents

Ajudam em tarefas específicas.

## Skills

Fornecem habilidades reutilizáveis.

## Workflows

Organizam a ordem de execução.

## Templates

Padronizam as entregas.

## Outputs

Armazenam os resultados finais.

## Review

Garante qualidade, coerência e aplicabilidade.

---

# 14. REGRA CENTRAL DE ARQUITETURA

Nenhum agente deve trabalhar de forma isolada ou improvisada.

Todo agente deve consultar:

1. O PRD, para entender a visão geral.
2. A Spec correspondente, para entender sua tarefa.
3. O Workflow ativo, para entender a ordem de execução.
4. Os Templates, para formatar a entrega.
5. O Harness, para respeitar as regras globais.
6. O Review Agent, para validar a qualidade final.

---

# 15. EXEMPLO PRÁTICO — TRACK RUNNING

## Entrada do usuário

```txt
Marca: Track Running
Segmento: esporte, corrida e fitness
Objetivo: criar uma marca para depois criar um aplicativo que faz treinos de corrida por IA.
```

## Como o BrandOS deve processar

1. Identificar que é uma marca nova e produto digital futuro.
2. Acionar o New Brand Workflow ou Digital Product Workflow.
3. Criar briefing guiado.
4. Analisar mercado de corrida, fitness e apps de treino.
5. Criar personas de corredores iniciantes e intermediários.
6. Definir posicionamento.
7. Criar proposta de valor.
8. Criar personalidade da marca.
9. Criar identidade verbal.
10. Criar direção visual.
11. Montar brand book.
12. Revisar consistência.
13. Gerar outputs finais.

## Exemplo de posicionamento

```md
A Track Running se posiciona como uma marca de tecnologia fitness para pessoas que querem começar ou evoluir na corrida com mais segurança, consistência e personalização, oferecendo treinos inteligentes guiados por IA para transformar a corrida em um hábito acessível e motivador.
```

## Outputs esperados

```txt
outputs/
├── 01-briefing-track-running.md
├── 02-research-track-running.md
├── 03-personas-track-running.md
├── 04-positioning-track-running.md
├── 05-value-proposition-track-running.md
├── 06-verbal-identity-track-running.md
├── 07-visual-identity-track-running.md
└── 08-brand-book-track-running.md
```

---

# 16. COMO USAR ESTE ARQUIVO NO CLAUDE CODE

Este arquivo pode ser usado como referência estrutural para o Claude Code.

## Prompt recomendado

```txt
Leia o arquivo BRANDOS_PRD_SPECS_SCAFFOLD_COMPLETO.md.
Com base nele, revise e melhore a estrutura atual do projeto BrandOS.
Crie ou atualize os arquivos necessários seguindo o PRD, as Specs, o Scaffold, os Agents, os Workflows, as Skills e os Templates definidos.
Mantenha a arquitetura modular e gere arquivos Markdown organizados.
Não remova conteúdo existente sem justificar.
Ao final, apresente um resumo das alterações feitas e uma lista de próximos passos.
```

---

# 17. CHECKLIST FINAL DO BRANDOS

Antes de finalizar qualquer entrega, verificar:

```txt
[ ] O projeto tem PRD claro?
[ ] As Specs estão definidas?
[ ] O Scaffold está organizado?
[ ] Os agentes têm responsabilidades claras?
[ ] Os subagentes têm funções específicas?
[ ] As skills são reutilizáveis?
[ ] Os workflows estão definidos?
[ ] Os templates padronizam as entregas?
[ ] Os outputs estão nomeados corretamente?
[ ] A linguagem está clara?
[ ] O sistema explica conceitos quando necessário?
[ ] As entregas não são genéricas?
[ ] A estratégia, o verbal e o visual estão conectados?
[ ] O brand book está completo?
[ ] A revisão final foi feita?
```

---

# 18. RESUMO FINAL

O BrandOS deve ser tratado como um sistema completo de construção de marca.

Para isso, ele precisa de:

- um PRD para definir a visão;
- Specs para detalhar o funcionamento;
- Scaffold para organizar o projeto;
- agentes para executar etapas;
- subagentes para tarefas específicas;
- skills para capacidades reutilizáveis;
- workflows para organizar a jornada;
- templates para padronizar entregas;
- outputs para armazenar resultados;
- review para garantir qualidade.

O objetivo final do BrandOS é permitir que qualquer pessoa transforme uma ideia em uma marca estruturada, estratégica, coerente, aplicável e documentada.

