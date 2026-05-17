# BRANDOS_HARNESS.md

**Projeto:** BrandOS — Branding System com agentes, subagentes, tasks e skills  
**Tipo de arquivo:** Harness de teste, validação, auditoria, QA e documentação  
**Versão do Harness:** v1.0.0  
**Versão sugerida do BrandOS:** v1.0.0  
**Status:** pronto para uso inicial no Claude Code, Claude Cloud / Cloud Coach, ChatGPT, Cursor, Antigravity e GitHub

---

## 0. Como usar este arquivo

Este arquivo deve ser colocado na raiz do projeto BrandOS, ao lado do `README.md`.

Estrutura recomendada:

```txt
brandos/
├── BRANDOS_HARNESS.md
├── README.md
├── LICENSE
├── .claude-plugin/
├── agents/
├── commands/
├── workflows/
└── templates/
```

O objetivo deste harness é testar se o BrandOS está funcionando como um sistema completo, guiado, intuitivo e profissional para criação de Branding Systems.

Este arquivo pode ser usado de três formas:

1. **Como documentação oficial do projeto.**
2. **Como checklist de auditoria no Claude Code.**
3. **Como prompt de validação para testar agentes, prompts, workflow, memória, entregáveis e qualidade final.**

---

# 1. Objetivo principal do BrandOS

O BrandOS tem como objetivo criar um workflow inteligente, fácil e intuitivo, baseado em agentes, subagentes, tasks e skills, capaz de transformar um briefing simples em um Branding System completo.

O sistema deve guiar o usuário passo a passo, reduzindo a complexidade do processo de branding e permitindo que ele crie sua própria marca de forma estratégica, organizada e profissional, mesmo sem dominar conceitos técnicos de branding.

A partir das informações fornecidas pelo usuário, o BrandOS deve gerar uma estrutura completa de marca, incluindo:

- estratégia de marca;
- posicionamento;
- proposta de valor;
- público-alvo;
- diferenciação;
- Brand DNA;
- personalidade de marca;
- identidade verbal;
- tom de voz;
- direção visual;
- sistema visual;
- brand book;
- assets;
- materiais de apoio;
- sistema de governança e QA.

Além de gerar entregáveis, o BrandOS deve validar a coerência entre as etapas, garantir consistência estratégica, verbal e visual, e facilitar a transformação do resultado em um brand book pronto para uso.

---

# 2. Objetivo do Harness

O BrandOS Harness é uma camada de controle, teste, auditoria, validação e documentação do sistema.

Ele deve verificar se o BrandOS:

- possui estrutura completa de plugin/projeto;
- contém todos os agentes esperados;
- possui comandos funcionais;
- segue o pipeline correto;
- executa as fases na ordem certa;
- usa memória persistente corretamente;
- faz perguntas adequadas ao usuário;
- adapta a experiência ao nível de conhecimento do usuário;
- valida gates estratégicos;
- detecta falhas;
- corrige inconsistências;
- gera logs;
- entrega um Brand System completo, coerente e profissional.

O harness não substitui o BrandOS. Ele testa se o BrandOS está funcionando com qualidade.

---

# 3. Uso previsto do projeto

O BrandOS será usado principalmente para:

- uso pessoal da criadora;
- criação de Branding Systems de forma fácil e intuitiva;
- venda como produto;
- plugin para Claude Code;
- automação para geração de brand books;
- criação de entregáveis estruturados de marca;
- documentação e evolução versionável no GitHub.

Neste momento, o projeto não tem como foco principal o atendimento direto a clientes, mas sim a criação de um sistema/produto que permita ao usuário gerar seu próprio Branding System com autonomia.

---

# 4. Plataformas compatíveis

O BrandOS deve funcionar como um sistema modular e multiplataforma.

Plataformas principais:

- Claude Code;
- Claude Cloud / Cloud Coach;
- ChatGPT;
- Cursor;
- Antigravity;
- GitHub;
- outras plataformas compatíveis com Markdown, workflows de agentes, automações por prompt ou documentação versionável.

## 4.1 Regra de portabilidade

O harness não deve depender exclusivamente de uma plataforma específica.

Sempre que possível, as instruções devem ser escritas de forma universal, para que possam ser copiadas, adaptadas ou executadas em diferentes ambientes.

Quando houver instruções específicas para uma plataforma, elas devem ficar em blocos próprios.

---

# 5. Usuário final do BrandOS

## 5.1 Quem vai usar

O BrandOS deve atender diferentes perfis de usuários:

- designers;
- empreendedores;
- social media;
- donos de pequenos negócios;
- criadores de conteúdo;
- agências;
- profissionais criativos;
- pessoas que estão começando uma marca do zero;
- pessoas sem experiência em branding;
- usuários que possuem apenas uma ideia inicial;
- usuários que já possuem uma marca e querem organizar ou melhorar o sistema de marca.

## 5.2 Nível de conhecimento em branding

O BrandOS deve atender usuários com diferentes níveis:

- pessoas que não entendem nada de branding;
- pessoas que entendem pouco;
- usuários intermediários;
- designers;
- agências;
- profissionais criativos;
- usuários avançados que desejam acelerar processos.

O sistema não deve presumir conhecimento técnico avançado.

## 5.3 Linguagem desejada

A linguagem do BrandOS deve ser:

- amigável;
- simplificada;
- didática;
- profissional;
- consultiva;
- acolhedora;
- estratégica;
- clara;
- objetiva;
- sem excesso de termos técnicos.

A experiência deve parecer uma conversa com uma consultora estratégica de marca: profissional, mas fácil de entender.

## 5.4 Explicação de conceitos

O BrandOS deve explicar conceitos sempre que necessário, de forma curta, simples, prática e conectada à etapa atual.

Conceitos que devem ser explicados quando aparecerem:

- branding;
- Brand System;
- posicionamento;
- proposta de valor;
- público-alvo;
- diferenciação;
- personalidade de marca;
- tom de voz;
- identidade verbal;
- direção visual;
- Brand DNA;
- brand book;
- assets;
- guidelines;
- governança de marca;
- QA de marca.

## 5.5 Regra de acessibilidade

O BrandOS deve ser fácil o suficiente para uma pessoa sem experiência em branding conseguir usar, mas estruturado o bastante para entregar valor a designers, social medias, empreendedores, agências e profissionais criativos.

---

# 6. Experiência ideal

## 6.1 Comportamento esperado

O BrandOS deve parecer uma consultora estratégica de marca:

- amigável;
- clara;
- didática;
- profissional;
- acolhedora;
- estratégica;
- organizada;
- segura;
- orientada a resultado.

## 6.2 Quantidade de perguntas

O sistema deve fazer perguntas em blocos pequenos, preferencialmente de 3 a 5 perguntas por etapa.

Ele deve evitar blocos longos demais, principalmente para usuários iniciantes.

## 6.3 Uso de exemplos

O BrandOS deve mostrar exemplos simples para ajudar o usuário a responder melhor, principalmente quando:

- o usuário demonstrar dúvida;
- o usuário responder de forma muito vaga;
- o usuário tiver pouco conhecimento;
- o conceito for técnico;
- a etapa exigir decisões estratégicas importantes.

## 6.4 Modos adaptativos

O BrandOS deve ter modo básico, intermediário e avançado, mas a seleção deve ser adaptativa.

O sistema deve identificar o nível do usuário pela forma como ele responde.

| Modo | Quando usar | Comportamento esperado |
|---|---|---|
| Básico | Usuário responde pouco, demonstra insegurança ou não domina branding | Explicar mais, fazer perguntas simples, trazer exemplos e evitar termos técnicos |
| Intermediário | Usuário traz informações razoáveis, mas ainda precisa de orientação | Fazer perguntas mais estratégicas e organizar as respostas em blocos claros |
| Avançado | Usuário traz contexto profundo, referências, objetivos e decisões claras | Aprofundar estratégia, validar nuances e acelerar etapas operacionais |

## 6.5 Salvar progresso

O BrandOS deve salvar progresso por fase, registrar decisões importantes e permitir que o usuário continue de onde parou.

O sistema deve manter registro de:

- fase atual;
- agente responsável;
- decisões aprovadas;
- respostas do usuário;
- pendências;
- próximos passos;
- score parcial;
- status dos gates.

---

# 7. Caminhos de entrada

O BrandOS deve aceitar diferentes tipos de entrada.

| Caminho de entrada | Deve aceitar? | Comportamento esperado |
|---|---:|---|
| Apenas uma ideia inicial | Sim | Ativar Discovery e conduzir com perguntas simples |
| Marca existente | Sim | Organizar, melhorar ou completar o Brand System existente |
| Redesign | Sim | Avaliar o que existe, o que precisa permanecer e o que deve mudar |
| Marca pessoal | Sim | Trabalhar narrativa, autoridade, personalidade e presença digital |
| Produto digital | Sim | Ativar ou recomendar UX + Product Experience |
| Loja física | Sim | Adaptar perguntas para operação local, experiência e comunicação |
| Loja online | Sim | Considerar canais digitais, conversão e experiência de compra |
| Agência ou serviço | Sim | Considerar portfólio, autoridade e diferenciação |
| Briefing completo | Sim | Avançar com validação e aprofundamento |
| Briefing incompleto | Sim | Não gerar marca final; ativar Discovery |

## 7.1 Regra principal

O sistema deve adaptar o fluxo de perguntas conforme o tipo de entrada.

Uma marca pessoal, uma loja física, uma agência, um SaaS e um aplicativo não devem receber exatamente o mesmo Discovery.

---

# 8. Estrutura atual esperada do projeto

O harness deve validar se a estrutura principal do BrandOS está presente.

```txt
brandos/
├── .claude-plugin/
│   ├── plugin.json
│   └── marketplace.json
├── agents/
│   ├── brandos-core.md
│   ├── onboarding-agent.md
│   ├── discovery-agent.md
│   ├── brand-context-agent.md
│   ├── competitive-research-agent.md
│   ├── audience-intelligence-agent.md
│   ├── strategy-agent.md
│   ├── brand-dna-agent.md
│   ├── verbal-identity-agent.md
│   ├── visual-identity-agent.md
│   ├── ux-product-experience-agent.md
│   ├── governance-qa-agent.md
│   ├── export-agent.md
│   └── production-agent.md
├── commands/
│   ├── brandos.md
│   ├── brandos-status.md
│   ├── brandos-resume.md
│   └── brandos-produce.md
├── workflows/
│   └── brandos-pipeline.md
├── templates/
│   └── memory/
│       ├── brand-dna.json
│       ├── strategic-memory.json
│       ├── creative-memory.json
│       ├── audience-memory.json
│       ├── decision-memory.json
│       ├── conversation-memory.json
│       ├── production-memory.json
│       └── campaign-memory.json
├── README.md
├── LICENSE
└── BRANDOS_HARNESS.md
```

---

# 9. Teste de integridade do plugin

## 9.1 Objetivo

Verificar se o projeto possui os arquivos mínimos para funcionar como plugin, workflow e documentação versionável.

## 9.2 Checklist

- [ ] Existe `.claude-plugin/plugin.json`
- [ ] Existe `.claude-plugin/marketplace.json`
- [ ] Existe `README.md`
- [ ] Existe `LICENSE`
- [ ] Existe pasta `agents/`
- [ ] Existe pasta `commands/`
- [ ] Existe pasta `workflows/`
- [ ] Existe pasta `templates/memory/`
- [ ] Existe `workflows/brandos-pipeline.md`
- [ ] Existe este arquivo `BRANDOS_HARNESS.md`

## 9.3 Critério de aprovação

O teste de integridade é aprovado se todos os arquivos essenciais estiverem presentes.

Se algum item essencial estiver ausente, o status deve ser:

```txt
STATUS: REPROVADO — ESTRUTURA INCOMPLETA
```

---

# 10. Agentes esperados

O BrandOS deve conter 14 agentes principais.

| Nº | Agente | Função principal | Status esperado |
|---:|---|---|---|
| 01 | `brandos-core.md` | Coordenação central do sistema | Obrigatório |
| 02 | `onboarding-agent.md` | Boas-vindas, orientação inicial e modo adaptativo | Obrigatório |
| 03 | `discovery-agent.md` | Coleta de briefing e aprofundamento inicial | Obrigatório |
| 04 | `brand-context-agent.md` | Análise de materiais/contexto da marca | Condicional |
| 05 | `competitive-research-agent.md` | Pesquisa e análise competitiva | Obrigatório |
| 06 | `audience-intelligence-agent.md` | Público-alvo, personas e audiência | Obrigatório |
| 07 | `strategy-agent.md` | Estratégia, posicionamento e diferenciação | Obrigatório |
| 08 | `brand-dna-agent.md` | Consolidação do DNA da marca e gate estratégico | Obrigatório |
| 09 | `verbal-identity-agent.md` | Tom de voz, mensagens e identidade verbal | Obrigatório |
| 10 | `visual-identity-agent.md` | Direção visual e sistema visual | Obrigatório |
| 11 | `ux-product-experience-agent.md` | Experiência de produto, app, SaaS, jornada e UX | Condicional |
| 12 | `governance-qa-agent.md` | QA, consistência e governança | Obrigatório |
| 13 | `export-agent.md` | Exportação dos documentos finais | Obrigatório |
| 14 | `production-agent.md` | Materiais de produção, campanhas e assets | Condicional |

---

# 11. Teste dos agentes

## 11.1 Objetivo

Validar se cada agente possui papel claro, entrada definida, saída esperada e limites de atuação.

## 11.2 Checklist geral por agente

Cada agente deve conter, de forma explícita ou inferível:

- [ ] nome do agente;
- [ ] descrição da função;
- [ ] fase correspondente;
- [ ] quando deve ser acionado;
- [ ] entrada esperada;
- [ ] tarefas principais;
- [ ] saída esperada;
- [ ] critérios de qualidade;
- [ ] dependências com agentes anteriores;
- [ ] limites do que não deve fazer;
- [ ] falhas que deve evitar.

## 11.3 Regras de comportamento por agente

### brandos-core

Deve coordenar o sistema como orquestrador principal.

Não deve executar tudo sozinho quando houver agentes especializados.

Deve garantir que:

- as fases sejam respeitadas;
- a memória seja consultada;
- o progresso seja salvo;
- os gates sejam respeitados;
- o usuário não fique perdido.

### onboarding-agent

Deve receber o usuário, explicar o processo de forma simples e identificar o nível de maturidade.

Deve:

- explicar como o BrandOS funciona;
- identificar o caminho de entrada;
- detectar modo básico, intermediário ou avançado;
- evitar excesso de perguntas no começo;
- orientar o usuário com clareza.

### discovery-agent

Deve coletar contexto e aprofundar o briefing.

Não deve gerar o Branding System final.

Deve fazer perguntas claras sobre:

- nome da marca;
- segmento;
- produto ou serviço;
- público;
- objetivo;
- problema que resolve;
- diferenciais;
- personalidade desejada;
- referências;
- canais de uso;
- estágio da marca.

### brand-context-agent

Deve analisar materiais existentes quando houver.

Deve considerar:

- logo atual;
- paleta atual;
- redes sociais;
- site;
- materiais antigos;
- brand book anterior;
- percepção atual da marca.

Se não houver materiais existentes, deve ser pulado ou marcado como não aplicável.

### competitive-research-agent

Deve mapear concorrentes, referências e oportunidades de diferenciação.

Deve evitar copiar concorrentes.

Deve buscar padrões, lacunas e oportunidades.

### audience-intelligence-agent

Deve transformar informações de público em perfis claros e úteis.

Deve entregar:

- público-alvo;
- dores;
- desejos;
- objeções;
- motivações;
- linguagem do público;
- possíveis personas.

### strategy-agent

Deve criar a estratégia de marca antes de qualquer decisão verbal ou visual.

Deve entregar:

- posicionamento;
- proposta de valor;
- promessa central;
- diferenciais;
- pilares estratégicos;
- território de marca.

### brand-dna-agent

Deve consolidar a essência da marca.

É um gate obrigatório.

Deve entregar:

- essência;
- propósito;
- valores;
- personalidade;
- promessa;
- diferenciação;
- posicionamento consolidado;
- princípios verbais e visuais.

### verbal-identity-agent

Deve criar identidade verbal a partir do Brand DNA aprovado.

Não deve criar tom de voz desalinhado com a estratégia.

Deve entregar:

- tom de voz;
- guia de linguagem;
- palavras que usa;
- palavras que evita;
- mensagens-chave;
- slogans, se aplicável;
- manifesto, se aplicável.

### visual-identity-agent

Deve criar direção visual a partir da estratégia e do Brand DNA aprovado.

Não deve criar visual apenas bonito sem conceito.

Deve entregar:

- direção criativa;
- paleta sugerida;
- tipografia sugerida;
- estilo fotográfico;
- elementos gráficos;
- aplicações visuais;
- prompts visuais, se aplicável.

### ux-product-experience-agent

Deve ser acionado quando houver produto digital, aplicativo, SaaS, site, plataforma ou experiência de serviço.

Deve entregar:

- princípios de experiência;
- jornada inicial;
- pilares de UX;
- recomendações de interface;
- coerência entre marca e produto.

### governance-qa-agent

Deve validar consistência geral.

É um gate obrigatório.

Deve verificar:

- coerência estratégica;
- consistência verbal;
- consistência visual;
- ausência de contradições;
- profundidade;
- aplicabilidade;
- prontidão para exportação.

### export-agent

Deve organizar a entrega final.

Deve gerar ou orientar a geração de:

- Brand System em Markdown;
- Brand Book;
- arquivos de memória;
- scorecard;
- logs;
- estrutura final de pastas.

### production-agent

Deve gerar materiais de produção quando solicitado.

Pode criar:

- posts;
- bio de Instagram;
- copy de landing page;
- prompts visuais;
- apresentação comercial;
- campanhas;
- assets derivados.

---

# 12. Comandos esperados

O BrandOS deve conter comandos principais para iniciar, acompanhar, retomar e produzir materiais.

| Comando | Arquivo esperado | Função |
|---|---|---|
| `/brandos` | `commands/brandos.md` | Iniciar ou executar fluxo principal |
| `/brandos-status` | `commands/brandos-status.md` | Verificar fase atual, progresso e pendências |
| `/brandos-resume` | `commands/brandos-resume.md` | Retomar projeto de onde parou |
| `/brandos-produce` | `commands/brandos-produce.md` | Gerar materiais de produção e assets |

## 12.1 Checklist de comandos

- [ ] Existe comando para iniciar o BrandOS.
- [ ] Existe comando para verificar status.
- [ ] Existe comando para retomar progresso.
- [ ] Existe comando para produzir materiais finais.
- [ ] Os comandos explicam quando devem ser usados.
- [ ] Os comandos respeitam memória e fase atual.
- [ ] Os comandos não pulam gates obrigatórios.

---

# 13. Pipeline de 14 fases

O BrandOS deve seguir 14 fases principais.

| Nº | Fase | Status | Agente principal |
|---:|---|---|---|
| 01 | Welcome / Onboarding | Obrigatória | onboarding-agent |
| 02 | Discovery Inicial | Obrigatória | discovery-agent |
| 03 | Materiais da Marca | Condicional | brand-context-agent |
| 04 | Competitive Discovery | Obrigatória | competitive-research-agent |
| 05 | Research Flow | Obrigatória | competitive-research-agent / strategy-agent |
| 06 | Audience Discovery | Obrigatória | audience-intelligence-agent |
| 07 | Strategy Flow | Obrigatória | strategy-agent |
| 08 | Brand DNA | Obrigatória / Gate | brand-dna-agent |
| 09 | Verbal Identity | Obrigatória | verbal-identity-agent |
| 10 | Visual Identity | Obrigatória | visual-identity-agent |
| 11 | UX + Product Experience | Condicional | ux-product-experience-agent |
| 12 | Governance + QA | Obrigatória / Gate | governance-qa-agent |
| 13 | Export System | Obrigatória | export-agent |
| 14 | Production System | Condicional | production-agent |

## 13.1 Fases obrigatórias

As fases obrigatórias são:

1. Welcome / Onboarding
2. Discovery Inicial
3. Competitive Discovery
4. Research Flow
5. Audience Discovery
6. Strategy Flow
7. Brand DNA
8. Verbal Identity
9. Visual Identity
10. Governance + QA
11. Export System

## 13.2 Fases condicionais

As fases condicionais são:

- **Materiais da Marca:** usada quando o usuário possui marca, arquivos, referências, redes sociais, logo, site ou materiais anteriores.
- **UX + Product Experience:** usada quando o projeto envolve produto digital, app, SaaS, site, plataforma, comunidade, jornada de usuário ou experiência de serviço.
- **Production System:** usada quando o usuário deseja gerar materiais de produção, campanhas, posts, landing pages, apresentações ou assets.

## 13.3 Fases adicionadas como subfases

O harness recomenda adicionar duas subfases:

### Seleção de Modo

Deve acontecer durante o Onboarding.

Objetivo:

- identificar se o usuário está no modo básico, intermediário ou avançado;
- adaptar linguagem e profundidade;
- ajustar quantidade de perguntas;
- definir se o sistema deve explicar mais ou acelerar.

### Resumo e Aprovação

Deve acontecer antes dos gates principais.

Objetivo:

- resumir decisões;
- confirmar entendimento;
- permitir ajustes;
- evitar que o sistema avance com premissas erradas.

---

# 14. Gates obrigatórios

O BrandOS deve ter pelo menos dois gates obrigatórios:

1. Gate 8 — Brand DNA
2. Gate 12 — Governance + QA

---

## 14.1 Gate 8 — Brand DNA

### Objetivo

Garantir que a base estratégica esteja clara antes de avançar para identidade verbal e visual.

### Checklist de aprovação

- [ ] Nome da marca preenchido ou definido como pendente.
- [ ] Segmento claro.
- [ ] Público-alvo definido.
- [ ] Problema que a marca resolve definido.
- [ ] Proposta de valor definida.
- [ ] Diferenciais definidos.
- [ ] Posicionamento claro.
- [ ] Personalidade da marca definida.
- [ ] Promessa central definida.
- [ ] Território de marca definido.
- [ ] Tom inicial sugerido.
- [ ] Direção estratégica aprovada.
- [ ] Decisões registradas na memória.

### Reprovação automática

O gate deve reprovar se:

- o posicionamento estiver genérico;
- o público estiver indefinido;
- a proposta de valor estiver vaga;
- não houver diferencial claro;
- houver contradição com o briefing;
- o sistema tiver inventado informações críticas;
- o usuário não tiver validado decisões essenciais.

---

## 14.2 Gate 12 — Governance + QA

### Objetivo

Garantir que o Brand System final esteja coerente, completo e pronto para exportação.

### Checklist de aprovação

- [ ] Estratégia coerente com o briefing.
- [ ] Público-alvo coerente com a proposta.
- [ ] Posicionamento claro.
- [ ] Identidade verbal alinhada ao Brand DNA.
- [ ] Tom de voz aplicável.
- [ ] Direção visual alinhada à estratégia.
- [ ] Entregáveis obrigatórios completos.
- [ ] Não há contradições graves.
- [ ] Memória atualizada.
- [ ] Score mínimo atingido.
- [ ] Próximos passos claros.

### Reprovação automática

O gate deve reprovar se:

- o score geral for menor que 70;
- houver contradição grave entre estratégia, verbal e visual;
- a marca estiver genérica demais;
- o brand book estiver superficial;
- o sistema tiver pulado etapas obrigatórias;
- o Brand DNA tiver sido ignorado;
- a exportação for solicitada antes do QA.

---

# 15. Sistema de memória

O BrandOS deve usar memória persistente para evitar perda de contexto e garantir consistência.

## 15.1 Arquivos esperados

| Arquivo | Função |
|---|---|
| `brand-dna.json` | Fonte única da verdade da marca |
| `strategic-memory.json` | Decisões estratégicas |
| `creative-memory.json` | Direção criativa, verbal e visual |
| `audience-memory.json` | Público, personas e insights de audiência |
| `decision-memory.json` | Decisões aprovadas e recusadas |
| `conversation-memory.json` | Histórico resumido da conversa |
| `production-memory.json` | Materiais produzidos e pendentes |
| `campaign-memory.json` | Campanhas e desdobramentos |

## 15.2 Regras de memória

- O Brand DNA deve ser a fonte única da verdade.
- Agentes devem ler a memória antes de produzir novas decisões.
- Ao final de cada fase, a memória deve ser atualizada.
- Decisões aprovadas não devem ser contraditas sem justificativa.
- O sistema deve registrar pendências.
- O sistema deve permitir retomada de projeto.
- O sistema deve evitar repetição de perguntas já respondidas.

## 15.3 Checklist de memória

- [ ] Todos os templates de memória existem.
- [ ] A memória é lida antes de gerar outputs importantes.
- [ ] A memória é atualizada após cada fase.
- [ ] O Brand DNA está consolidado.
- [ ] Decisões estratégicas estão registradas.
- [ ] O sistema consegue retomar de onde parou.
- [ ] Não há contradições entre arquivos de memória.

---

# 16. Entregáveis finais

## 16.1 Entregáveis obrigatórios

O BrandOS deve gerar, no mínimo:

- Discovery organizado;
- diagnóstico inicial da marca;
- análise de contexto;
- análise de concorrentes;
- público-alvo;
- personas ou perfis de audiência;
- estratégia de marca;
- posicionamento;
- proposta de valor;
- diferenciais;
- Brand DNA;
- personalidade da marca;
- tom de voz;
- identidade verbal;
- mensagens-chave;
- direção visual;
- recomendações de paleta de cores;
- recomendações de tipografia;
- estilo visual;
- aplicações iniciais da marca;
- Governance + QA;
- Brand System final em Markdown;
- estrutura para Brand Book.

## 16.2 Entregáveis opcionais

O BrandOS pode gerar:

- análise de materiais existentes;
- naming;
- slogans;
- manifesto;
- arquétipo de marca;
- missão, visão e valores;
- guia de linguagem completo;
- estilo fotográfico;
- elementos gráficos;
- prompts para criação visual;
- bio para Instagram;
- posts para redes sociais;
- copy para landing page;
- apresentação comercial;
- campanhas;
- assets adicionais.

## 16.3 Entregáveis do modo avançado

No modo avançado, o BrandOS pode gerar:

- brand book completo;
- brand guidelines em PDF;
- sistema de governança da marca;
- guia de aplicação visual;
- guia de consistência verbal;
- matriz de decisão estratégica;
- scorecard de qualidade;
- logs completos da execução;
- documentação versionável no GitHub;
- materiais de produção;
- prompts finais para execução visual.

---

# 17. Estrutura de exportação esperada

O output final recomendado deve seguir esta estrutura:

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
│   ├── 03-brand-context.md
│   ├── 04-competitive-research.md
│   ├── 05-audience.md
│   ├── 06-strategy.md
│   ├── 07-brand-dna.md
│   ├── 08-verbal-identity.md
│   ├── 09-visual-identity.md
│   ├── 10-ux-product-experience.md
│   ├── 11-governance-qa.md
│   └── brand-system.md
├── 02-pdf/
│   └── brand-guidelines.pdf
├── 03-production/
│   ├── social-posts.md
│   ├── landing-page-copy.md
│   ├── prompt-visual.md
│   └── campaign-ideas.md
└── 04-assets/
    └── README.md
```

## 17.1 Checklist de exportação

- [ ] Existe pasta `brandos-output/`.
- [ ] Existe pasta `memory/`.
- [ ] Existe pasta `01-brand-system/`.
- [ ] Existe `brand-system.md`.
- [ ] Existe documento de QA.
- [ ] Existe scorecard.
- [ ] Existem arquivos de memória atualizados.
- [ ] Entregáveis obrigatórios foram exportados.
- [ ] Entregáveis opcionais foram exportados somente quando aplicáveis.

---

# 18. Qualidade mínima

## 18.1 Nota mínima

A nota mínima recomendada para aprovação geral é **80/100**.

## 18.2 Classificação

| Nota | Status | Significado |
|---:|---|---|
| 0 a 69 | Reprovado | O sistema precisa revisar antes de exportar |
| 70 a 79 | Aprovado com ajustes obrigatórios | Pode avançar somente após correções |
| 80 a 89 | Aprovado | Entrega consistente e utilizável |
| 90 a 100 | Excelente | Entrega forte, profunda e profissional |

## 18.3 Critérios mais importantes

- clareza estratégica;
- coerência com o briefing;
- profundidade da análise;
- diferenciação da marca;
- consistência entre estratégia, verbal e visual;
- aplicabilidade prática;
- facilidade de entendimento pelo usuário;
- qualidade profissional dos entregáveis;
- capacidade de virar brand book;
- ausência de contradições.

## 18.4 Reprovação automática

O BrandOS deve reprovar automaticamente se:

- gerar branding genérico demais;
- pular Discovery;
- criar direção visual antes da estratégia;
- ignorar o público-alvo;
- contradizer o Brand DNA;
- inventar informações críticas;
- entregar brand book superficial;
- finalizar sem passar pelo QA;
- criar tom de voz desalinhado com o posicionamento;
- gerar visual bonito, mas sem conceito estratégico;
- exportar sem score mínimo.

---

# 19. Rubrica de pontuação

Cada critério deve receber nota de 0 a 10.

| Critério | Peso | Descrição |
|---|---:|---|
| Clareza estratégica | 10 | A estratégia é clara, compreensível e bem organizada |
| Coerência com briefing | 10 | As decisões respeitam o que o usuário informou |
| Público-alvo | 10 | O público está bem definido e utilizável |
| Posicionamento | 10 | A marca tem espaço claro e diferencial |
| Diferenciação | 10 | A marca não parece genérica ou igual aos concorrentes |
| Brand DNA | 10 | A essência está forte e orienta o sistema |
| Identidade verbal | 10 | Tom, mensagens e linguagem estão coerentes |
| Identidade visual | 10 | Direção visual tem conceito e aplicabilidade |
| Aplicabilidade | 10 | A entrega pode ser usada na prática |
| Consistência geral | 10 | Estratégia, verbal e visual funcionam juntos |

Pontuação máxima: 100.

## 19.1 Regra de pesos críticos

Mesmo que a média geral seja alta, a entrega deve ser reprovada ou marcada para revisão se algum destes critérios receber menos de 7:

- posicionamento;
- diferenciação;
- Brand DNA;
- consistência geral;
- coerência com briefing.

---

# 20. Falhas que o sistema deve evitar

O BrandOS não pode:

- gerar branding genérico;
- pular etapas essenciais;
- fazer perguntas confusas;
- usar linguagem técnica demais com iniciantes;
- deixar de explicar conceitos;
- criar estratégia sem entender o público;
- criar posicionamento sem diferencial;
- criar identidade verbal desalinhada;
- criar direção visual sem estratégia;
- contradizer decisões anteriores;
- ignorar o briefing;
- esquecer progresso salvo;
- misturar públicos diferentes sem justificar;
- entregar brand book incompleto;
- aprovar score baixo;
- dar respostas bonitas, mas pouco aplicáveis;
- avançar para exportação sem validação;
- transformar o processo em algo pesado demais para usuários iniciantes.

## 20.1 Regra principal

O BrandOS deve priorizar coerência, clareza e aplicabilidade acima de respostas bonitas.

---

# 21. Modos do harness

O harness deve funcionar em diferentes modos.

| Modo | Comando sugerido | Função |
|---|---|---|
| audit | `/brandos-harness audit` | Verifica estrutura do projeto e arquivos essenciais |
| agent-check | `/brandos-harness agent-check` | Testa se os agentes existem e possuem função clara |
| prompt-check | `/brandos-harness prompt-check` | Valida clareza e consistência dos prompts |
| run | `/brandos-harness run` | Executa um caso de teste completo |
| qa | `/brandos-harness qa` | Avalia um Brand System já criado |
| repair | `/brandos-harness repair` | Identifica falhas e propõe correções |
| export-check | `/brandos-harness export-check` | Valida se os arquivos finais foram gerados |
| score | `/brandos-harness score` | Gera pontuação geral do projeto |

---

# 22. Testes de prompt

## 22.1 Objetivo

Validar se os prompts dos agentes são claros, completos e coerentes com o objetivo do BrandOS.

## 22.2 Checklist

- [ ] O prompt explica a função do agente.
- [ ] O prompt define entrada e saída esperadas.
- [ ] O prompt evita respostas genéricas.
- [ ] O prompt respeita o nível do usuário.
- [ ] O prompt explica conceitos quando necessário.
- [ ] O prompt segue a fase correta do pipeline.
- [ ] O prompt não invade responsabilidades de outros agentes.
- [ ] O prompt consulta a memória quando necessário.
- [ ] O prompt registra decisões importantes.
- [ ] O prompt possui critérios de qualidade.

## 22.3 Falhas comuns em prompts

- agente tenta fazer tudo sozinho;
- agente pula etapas;
- agente gera output final antes do gate;
- prompt não orienta linguagem amigável;
- prompt não define formato de saída;
- prompt não menciona memória;
- prompt não explica o que fazer quando faltar informação.

---

# 23. Testes de UX conversacional

## 23.1 Objetivo

Validar se o BrandOS é fácil e intuitivo para o usuário.

## 23.2 Checklist

- [ ] O sistema explica o processo de forma simples.
- [ ] O sistema não começa com perguntas demais.
- [ ] O sistema mostra exemplos quando necessário.
- [ ] O sistema adapta a linguagem ao nível do usuário.
- [ ] O sistema evita jargões sem explicação.
- [ ] O sistema confirma decisões antes de avançar.
- [ ] O sistema permite continuar de onde parou.
- [ ] O sistema informa a fase atual.
- [ ] O sistema deixa claro o próximo passo.
- [ ] O sistema não faz o usuário se sentir perdido.

---

# 24. Casos de teste

Os casos de teste simulam marcas e cenários para validar se o BrandOS funciona corretamente.

---

## Caso 1 — Track Running

### Tipo

Marca nova com potencial futuro de produto digital.

### Nome

Track Running

### Segmento

Esporte, corrida e fitness.

### Objetivo

Criar uma marca para, futuramente, evoluir para um aplicativo que faz treinos de corrida personalizados por inteligência artificial.

### Contexto

A Track Running nasce como uma marca voltada para pessoas que querem melhorar sua performance na corrida com orientação inteligente, acessível e personalizada.

A marca deve preparar a base estratégica, verbal e visual para futuramente evoluir para um aplicativo de treinos por IA.

### Público inicial

Pessoas que correm ou querem começar a correr, incluindo:

- iniciantes;
- corredores amadores;
- pessoas interessadas em saúde;
- pessoas interessadas em performance;
- pessoas que querem emagrecer;
- pessoas que buscam condicionamento físico;
- pessoas que precisam de rotina de treinos.

### Personalidade desejada

- energética;
- inteligente;
- motivadora;
- moderna;
- confiável;
- acessível;
- tecnológica.

### Resultado esperado

O BrandOS deve criar uma marca esportiva moderna, com estratégia clara, posicionamento voltado para corrida e tecnologia, tom de voz motivador sem ser exagerado, identidade verbal acessível e direção visual com energia, movimento, performance e inovação.

### Critérios específicos de validação

- [ ] A marca comunica corrida, progresso e evolução.
- [ ] A marca parece confiável para iniciantes.
- [ ] A marca também parece útil para corredores mais experientes.
- [ ] A identidade não parece genérica de academia.
- [ ] A direção visual transmite movimento, ritmo, performance e tecnologia.
- [ ] O sistema identifica potencial de produto digital futuro.
- [ ] A fase UX + Product Experience é acionada ou recomendada.
- [ ] O tom de voz motiva sem soar forçado.

---

## Caso 2 — Casa Toyos

### Tipo

Pequeno negócio local.

### Nome

Casa Toyos

### Segmento

Móveis planejados.

### Objetivo

Organizar a marca para comunicar confiança, qualidade, personalização e facilidade de pagamento.

### Público inicial

Famílias, casais e pessoas que desejam mobiliar a casa com móveis personalizados.

### Personalidade desejada

- acolhedora;
- confiável;
- prática;
- familiar;
- acessível;
- profissional.

### Resultado esperado

O BrandOS deve gerar uma estratégia clara para um negócio local, com linguagem acessível, foco em confiança e aplicações para redes sociais, WhatsApp e materiais comerciais.

### Critérios específicos de validação

- [ ] A marca comunica confiança.
- [ ] A linguagem é simples e comercial.
- [ ] A marca não parece fria ou distante.
- [ ] O sistema considera canais como WhatsApp e Instagram.
- [ ] O resultado pode ser usado por vendedoras, social media ou dona do negócio.

---

## Caso 3 — Milena Miranda

### Tipo

Marca pessoal.

### Nome

Milena Miranda

### Segmento

Design, branding e inteligência artificial.

### Objetivo

Construir uma marca pessoal que una criatividade, estratégia, tecnologia e didática.

### Público inicial

Empreendedores, criadores, designers e pessoas interessadas em criar marcas com apoio de IA.

### Personalidade desejada

- criativa;
- estratégica;
- acessível;
- humana;
- inovadora;
- didática.

### Resultado esperado

O BrandOS deve gerar posicionamento de marca pessoal, narrativa, tom de voz, pilares de conteúdo, direção visual e possíveis desdobramentos para LinkedIn, Instagram e produto digital.

### Critérios específicos de validação

- [ ] A marca pessoal não parece genérica.
- [ ] A narrativa conecta design, branding e IA.
- [ ] O tom é humano e estratégico.
- [ ] O sistema propõe pilares de conteúdo.
- [ ] A direção visual apoia autoridade e criatividade.

---

## Caso 4 — NexaFlow

### Tipo

Produto digital / SaaS.

### Nome

NexaFlow

### Segmento

SaaS de produtividade para pequenos negócios.

### Objetivo

Criar uma marca simples, moderna e confiável para um produto digital.

### Público inicial

Microempreendedores e equipes pequenas que precisam organizar tarefas e processos.

### Personalidade desejada

- eficiente;
- moderna;
- clara;
- confiável;
- objetiva;
- tecnológica.

### Resultado esperado

O BrandOS deve acionar a fase UX + Product Experience, criar estratégia, posicionamento, tom de voz funcional e experiência de produto coerente.

### Critérios específicos de validação

- [ ] A fase UX é acionada.
- [ ] A marca parece simples e confiável.
- [ ] O tom de voz é claro e funcional.
- [ ] A direção visual comunica produtividade e organização.
- [ ] O sistema considera produto, interface e jornada.

---

## Caso 5 — Briefing incompleto

### Tipo

Teste de falha.

### Nome

Lume

### Segmento

Não informado.

### Público

Não informado.

### Objetivo informado pelo usuário

“Quero uma marca bonita.”

### Resultado esperado

O BrandOS não deve gerar o Branding System completo imediatamente.

Ele deve:

- explicar que precisa de mais contexto;
- ativar o Discovery;
- fazer perguntas simples;
- mostrar exemplos;
- identificar segmento, público, objetivo, personalidade e referências;
- salvar progresso;
- só avançar depois de obter informações mínimas.

### Critérios específicos de validação

- [ ] O sistema não inventa segmento.
- [ ] O sistema não cria visual final sem estratégia.
- [ ] O sistema faz perguntas de Discovery.
- [ ] O sistema mantém linguagem amigável.
- [ ] O sistema explica por que precisa de mais informações.

---

# 25. Logs

O harness deve gerar logs em Markdown e, quando possível, em JSON.

## 25.1 Logs em Markdown

Uso:

- leitura humana;
- revisão manual;
- documentação;
- acompanhamento de projeto;
- registro de decisões.

Arquivo sugerido:

```txt
brandos-run-log.md
```

## 25.2 Logs em JSON

Uso:

- automação futura;
- integração com ferramentas;
- comparação entre execuções;
- auditoria técnica;
- versionamento estruturado.

Arquivos sugeridos:

```txt
brandos-scorecard.json
brandos-errors.json
brandos-memory-state.json
```

## 25.3 Campos obrigatórios do log

Cada log deve registrar:

- data da execução;
- nome da marca;
- modo utilizado;
- fase executada;
- agente responsável;
- input recebido;
- output gerado;
- decisões tomadas;
- score da fase;
- falhas identificadas;
- correções aplicadas;
- status da fase;
- status geral do projeto;
- próxima etapa recomendada.

---

# 26. Template de log em Markdown

```md
# BrandOS Run Log

## Projeto

Nome da marca:
Tipo de projeto:
Data:
Modo do harness:
Status geral:

---

## Fase executada

Fase:
Agente responsável:
Status:
Score parcial:

### Input recebido


### Output gerado


### Decisões tomadas


### Falhas encontradas


### Correções aplicadas


### Próxima etapa

```

---

# 27. Template de scorecard

```md
# BrandOS Scorecard

## Projeto

Nome da marca:
Data:
Modo:

## Pontuação

| Critério | Nota | Observação |
|---|---:|---|
| Clareza estratégica | 0/10 |  |
| Coerência com briefing | 0/10 |  |
| Público-alvo | 0/10 |  |
| Posicionamento | 0/10 |  |
| Diferenciação | 0/10 |  |
| Brand DNA | 0/10 |  |
| Identidade verbal | 0/10 |  |
| Identidade visual | 0/10 |  |
| Aplicabilidade | 0/10 |  |
| Consistência geral | 0/10 |  |

## Resultado

Score total:
Status:

## Ajustes obrigatórios

- 

## Recomendações

- 
```

---

# 28. Template JSON de score

```json
{
  "project_name": "",
  "date": "",
  "harness_mode": "",
  "overall_score": 0,
  "status": "",
  "criteria": {
    "strategic_clarity": 0,
    "briefing_coherence": 0,
    "audience_quality": 0,
    "positioning": 0,
    "differentiation": 0,
    "brand_dna": 0,
    "verbal_identity": 0,
    "visual_identity": 0,
    "applicability": 0,
    "general_consistency": 0
  },
  "critical_failures": [],
  "required_fixes": [],
  "recommendations": [],
  "next_step": ""
}
```

---

# 29. Prompt master para rodar o harness

Use este prompt no Claude Code, ChatGPT, Cursor, Antigravity ou Cloud Coach para executar o harness.

```md
Você é o BrandOS Harness, responsável por auditar, testar, validar e melhorar o projeto BrandOS.

Sua função é verificar se o BrandOS está funcionando como um sistema completo de criação de Branding Systems, com agentes, subagentes, tasks, skills, memória, gates, QA, exportação e documentação.

Você deve avaliar:

1. estrutura do projeto;
2. arquivos obrigatórios;
3. agentes;
4. comandos;
5. workflow de 14 fases;
6. memória persistente;
7. gates obrigatórios;
8. experiência do usuário;
9. qualidade dos entregáveis;
10. consistência estratégica, verbal e visual;
11. logs;
12. score final;
13. falhas e correções.

Siga as regras deste arquivo BRANDOS_HARNESS.md.

Ao executar, informe:

- modo utilizado;
- itens verificados;
- problemas encontrados;
- score;
- status final;
- correções recomendadas;
- próximos passos.

Nunca aprove uma entrega se houver contradição grave entre estratégia, Brand DNA, identidade verbal e identidade visual.

Nunca avance para exportação se o Governance + QA não tiver sido aprovado.

Priorize clareza, consistência, aplicabilidade e experiência amigável para o usuário.
```

---

# 30. Prompt para auditoria estrutural

```md
Execute o modo `/brandos-harness audit`.

Verifique se o projeto BrandOS possui todos os arquivos e pastas obrigatórios:

- .claude-plugin/plugin.json
- .claude-plugin/marketplace.json
- README.md
- LICENSE
- agents/
- commands/
- workflows/brandos-pipeline.md
- templates/memory/
- BRANDOS_HARNESS.md

Depois, verifique se existem os 14 agentes esperados, os 4 comandos principais e os 8 templates de memória.

Retorne:

1. checklist completo;
2. arquivos encontrados;
3. arquivos ausentes;
4. riscos;
5. score de integridade;
6. status final;
7. recomendações de correção.
```

---

# 31. Prompt para teste de caso real

```md
Execute o modo `/brandos-harness run` usando o Caso 1 — Track Running.

Simule a entrada de um usuário que deseja criar uma marca chamada Track Running, no segmento de esporte, corrida e fitness, com o objetivo futuro de criar um aplicativo de treinos de corrida personalizados por inteligência artificial.

Valide se o BrandOS:

1. entende que é uma marca nova;
2. entende que há potencial de produto digital futuro;
3. ativa Discovery;
4. estrutura público-alvo;
5. cria posicionamento coerente;
6. gera Brand DNA;
7. cria identidade verbal motivadora, mas não exagerada;
8. cria direção visual ligada a movimento, performance e tecnologia;
9. recomenda ou aciona UX + Product Experience;
10. passa pelo Governance + QA.

No final, gere score, falhas, correções e status.
```

---

# 32. Prompt para QA de entrega existente

```md
Execute o modo `/brandos-harness qa`.

Avalie o Brand System gerado abaixo com base nos critérios deste harness.

Você deve verificar:

- clareza estratégica;
- coerência com briefing;
- público-alvo;
- posicionamento;
- diferenciação;
- Brand DNA;
- identidade verbal;
- identidade visual;
- aplicabilidade;
- consistência geral.

Dê uma nota de 0 a 100.

Classifique como:

- Reprovado;
- Aprovado com ajustes obrigatórios;
- Aprovado;
- Excelente.

Aponte:

1. pontos fortes;
2. falhas;
3. contradições;
4. ajustes obrigatórios;
5. recomendações;
6. próximos passos.
```

---

# 33. Prompt para repair

```md
Execute o modo `/brandos-harness repair`.

Analise as falhas encontradas no BrandOS ou em um Brand System gerado.

Para cada falha, retorne:

- tipo da falha;
- fase onde ocorreu;
- agente provável;
- impacto no resultado;
- correção recomendada;
- prioridade;
- exemplo de ajuste.

Prioridades:

- Alta: impede aprovação ou gera contradição grave.
- Média: reduz qualidade, mas não quebra o sistema.
- Baixa: melhoria de clareza, organização ou refinamento.
```

---

# 34. Prompt para export-check

```md
Execute o modo `/brandos-harness export-check`.

Verifique se a exportação final do BrandOS possui todos os arquivos esperados.

Avalie:

- estrutura de pastas;
- arquivos de memória;
- Brand System em Markdown;
- documento de QA;
- scorecard;
- assets;
- materiais opcionais;
- consistência entre arquivos.

Retorne:

1. arquivos encontrados;
2. arquivos ausentes;
3. inconsistências;
4. score de exportação;
5. status final;
6. recomendações.
```

---

# 35. Checklist final de aprovação do BrandOS

O BrandOS só deve ser considerado aprovado se:

- [ ] A estrutura do projeto está completa.
- [ ] Todos os agentes obrigatórios existem.
- [ ] Todos os comandos principais existem.
- [ ] O pipeline de 14 fases está documentado.
- [ ] As fases obrigatórias são respeitadas.
- [ ] As fases condicionais são acionadas corretamente.
- [ ] O Discovery não é pulado.
- [ ] O Brand DNA funciona como gate.
- [ ] O Governance + QA funciona como gate.
- [ ] A memória persistente está estruturada.
- [ ] O sistema salva progresso.
- [ ] O sistema permite retomada.
- [ ] A linguagem é amigável e simplificada.
- [ ] O sistema explica conceitos.
- [ ] O usuário iniciante consegue usar.
- [ ] O usuário avançado não fica limitado.
- [ ] Os entregáveis obrigatórios são gerados.
- [ ] O Brand System final é coerente.
- [ ] O score mínimo é 80/100.
- [ ] Não há contradição grave entre estratégia, verbal e visual.
- [ ] O projeto está pronto para Claude Code, Cloud Coach, ChatGPT, Cursor, Antigravity e GitHub.

---

# 36. Roadmap recomendado

## v1.0.0

- Harness completo em Markdown.
- Testes de estrutura.
- Testes de agentes.
- Testes de workflow.
- Rubrica de qualidade.
- Casos de teste.
- Logs.
- Prompts de execução.

## v1.1.0

- Adicionar comando real `/brandos-harness`.
- Criar arquivo `commands/brandos-harness.md`.
- Criar templates reais de scorecard.
- Criar pasta `tests/` com casos de teste separados.

## v1.2.0

- Automatizar auditoria de arquivos.
- Gerar relatórios em JSON.
- Comparar execuções por versão.
- Criar testes específicos por agente.

## v2.0.0

- Criar sistema automatizado de QA.
- Criar interface ou fluxo guiado.
- Integrar com exportação de PDF.
- Integrar com geração de assets.
- Criar validação de produto para venda.

---

# 37. Changelog

## v1.0.0 — Versão inicial

Inclui:

- objetivo do BrandOS;
- objetivo do harness;
- plataformas compatíveis;
- usuário final;
- experiência ideal;
- caminhos de entrada;
- estrutura esperada do projeto;
- agentes esperados;
- comandos esperados;
- pipeline de 14 fases;
- gates obrigatórios;
- sistema de memória;
- entregáveis finais;
- estrutura de exportação;
- rubrica de pontuação;
- falhas a evitar;
- modos do harness;
- testes de prompt;
- testes de UX conversacional;
- casos de teste;
- logs;
- scorecard;
- prompts master;
- checklist final;
- roadmap.

---

# 38. Decisão final do Harness

O BrandOS Harness deve garantir que o BrandOS não seja apenas um gerador de respostas bonitas.

Ele deve validar se o sistema realmente funciona como um processo profissional, intuitivo e consistente de criação de Branding Systems.

O objetivo final é transformar o BrandOS em um produto confiável, reutilizável, versionável e pronto para evoluir como plugin, workflow, automação e sistema operacional de marca.

