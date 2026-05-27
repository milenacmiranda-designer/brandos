# BRANDOS — Atualização de Workflow: Fase de Key Visual & Direção de Aplicações

> Arquivo de atualização para integrar ao projeto BrandOS / AI Brand Operating System no Claude Code.
>
> Objetivo: adicionar uma fase estruturada de **Key Visual** ao fluxo de criação de marca, conectando estratégia, universo visual, propostas de layout e geração final do brand book/PDF.

---

## 1. Contexto da atualização

O BrandOS já possui um fluxo robusto de construção de marca, com etapas voltadas para:

- onboarding;
- briefing;
- diagnóstico;
- estratégia;
- posicionamento;
- Brand DNA;
- identidade verbal;
- identidade visual;
- universo visual;
- UX / produto;
- propostas de layout;
- geração de relatório final em PDF;
- exportação de arquivos estruturados;
- QA de consistência.

Também já foi definido que, após o usuário responder às perguntas principais, o sistema entra em uma **Fase de Consolidação Pós-Briefing**, onde pode escolher entre:

1. gerar um PDF completo da marca;
2. avançar para propostas visuais/layouts;
3. revisar respostas anteriores;
4. continuar a construção do sistema da marca.

A atualização proposta aqui adiciona uma etapa essencial entre o **Universo Visual** e as **Propostas de Layout**:

# Fase de Key Visual & Direção de Aplicações

Essa fase evita que o sistema pule diretamente de “cores, fontes e referências” para “layouts finais” sem antes consolidar uma imagem-mãe da marca.

---

## 2. O que é Key Visual dentro do BrandOS

No BrandOS, o **Key Visual** deve ser entendido como a composição visual central que traduz a identidade da marca em uma linguagem gráfica aplicável.

Ele não é apenas um post, uma capa, uma tela ou um banner isolado.

Ele é a **peça-mãe visual** que orienta todos os desdobramentos gráficos da marca.

Em termos simples:

> O Key Visual é a primeira materialização visual completa da marca depois da estratégia e da direção visual.

Ele mostra como a marca se comporta quando seus elementos aparecem juntos:

- logo;
- cores;
- tipografia;
- imagens;
- grafismos;
- texturas;
- símbolos;
- grid;
- ritmo visual;
- mensagens principais;
- composição;
- hierarquia de informação;
- estilo editorial ou digital;
- atmosfera visual.

---

## 3. Por que adicionar essa fase

A fase de Key Visual resolve um problema importante do workflow:

Antes, o sistema poderia definir:

- paleta de cores;
- tipografias;
- moodboard;
- referências visuais;
- estilo gráfico;
- tom visual.

Mas ainda faltava uma etapa intermediária para responder:

> Como tudo isso aparece junto em uma peça visual real?

Sem o Key Visual, o sistema corre o risco de gerar layouts muito diferentes entre si, sem unidade estética.

Com o Key Visual, o BrandOS cria uma referência visual central antes de produzir:

- posts;
- landing pages;
- apresentações;
- relatórios;
- campanhas;
- capas;
- banners;
- peças comerciais;
- telas de produto;
- brand book;
- materiais editoriais.

---

## 4. Onde a fase entra no workflow atual

A nova fase deve entrar depois da construção do Universo Visual e antes das Propostas de Layout.

### Fluxo atualizado sugerido

```txt
01. Onboarding
02. Discovery / Briefing
03. Diagnóstico da Marca
04. Estratégia de Marca
05. Posicionamento
06. Brand DNA
07. Identidade Verbal
08. Universo Visual
09. Key Visual & Direção de Aplicações
10. Propostas de Layout
11. UX / Produto / Brand-to-Product Bridge
12. Guidelines / Design System
13. Export System
14. QA / Consistência Final
```

Caso o projeto mantenha a nomenclatura anterior com 14 fases fixas, a fase de Key Visual pode ser incorporada como subfase oficial dentro da etapa de Identidade Visual, mas o ideal é que ela tenha status próprio no fluxo.

### Opção A — Como fase própria

```txt
08. Universo Visual
09. Key Visual & Direção de Aplicações
10. Propostas de Layout
```

### Opção B — Como subfase da Identidade Visual

```txt
08. Identidade Visual
    08.1 Moodboard
    08.2 Paleta de Cores
    08.3 Tipografia
    08.4 Grafismos
    08.5 Estilo de Imagem
    08.6 Key Visual
    08.7 Direção de Aplicações
```

### Recomendação

Usar como fase própria:

# 09. Key Visual & Direção de Aplicações

Porque essa etapa tem importância estratégica e prática. Ela faz a ponte entre conceito e aplicação.

---

## 5. Nome oficial da nova fase

Nome recomendado:

# Key Visual & Direção de Aplicações

Nomes alternativos aceitos:

- Direção Visual Aplicada;
- Consolidação Visual da Marca;
- Sistema Visual em Ação;
- Visual Master Direction;
- Brand Visual Application System.

Nome preferencial para o BrandOS:

```txt
09_KEY_VISUAL_DIRECAO_APLICACOES.md
```

---

## 6. Função estratégica da fase

A fase de Key Visual deve consolidar visualmente:

1. o posicionamento da marca;
2. a personalidade definida no Brand DNA;
3. o território verbal;
4. o universo visual;
5. os elementos gráficos principais;
6. a linguagem estética dominante;
7. a lógica de aplicação da marca em peças reais.

Ela deve transformar decisões abstratas em uma referência visual concreta.

Exemplo:

```txt
Estratégia: marca de corrida com IA, performance e autonomia.
Personalidade: energética, inteligente, próxima e motivadora.
Universo visual: tecnológico, esportivo, limpo, com dados e movimento.
Key Visual: composição com corredor em movimento, linhas de rota, dados de performance, headline forte, paleta vibrante, tipografia sem serifa e grid dinâmico.
```

---

## 7. Entradas necessárias para gerar o Key Visual

A fase de Key Visual deve usar como input as etapas anteriores.

### Inputs obrigatórios

- nome da marca;
- segmento;
- público-alvo;
- objetivo da marca;
- posicionamento;
- proposta de valor;
- Brand DNA;
- personalidade da marca;
- tom de voz;
- mensagens-chave;
- slogan ou tagline, se existir;
- paleta de cores;
- tipografias sugeridas;
- moodboard;
- referências visuais;
- estilo de imagem;
- estilo gráfico;
- território visual;
- restrições de uso;
- canais prioritários.

### Inputs opcionais

- logo já existente;
- símbolo;
- ilustrações;
- fotografia de produto;
- imagens institucionais;
- materiais antigos da marca;
- referências de concorrentes;
- benchmark visual;
- estilos proibidos;
- aplicações desejadas pelo usuário.

---

## 8. Saídas esperadas da fase

A fase deve gerar um documento estruturado com:

### 8.1 Conceito visual central

Descrição do conceito por trás do Key Visual.

Exemplo:

```txt
O Key Visual da marca parte da ideia de movimento inteligente: uma estética que combina energia esportiva, dados de performance e proximidade humana. A composição deve transmitir progresso, tecnologia acessível e evolução contínua.
```

### 8.2 Direção de composição

Definir como os elementos aparecem na peça:

- composição centralizada ou assimétrica;
- uso de grid;
- hierarquia entre imagem, texto e marca;
- respiro visual;
- áreas de destaque;
- proporção entre elementos;
- ritmo gráfico;
- uso de contraste.

### 8.3 Direção tipográfica aplicada

Definir como a tipografia deve aparecer em uso real:

- títulos;
- subtítulos;
- textos de apoio;
- números/dados;
- legendas;
- CTAs;
- hierarquia;
- peso visual;
- alinhamento;
- espaçamento.

### 8.4 Direção cromática aplicada

Definir como as cores devem funcionar na prática:

- cor principal;
- cor de contraste;
- cor de apoio;
- fundos;
- áreas de destaque;
- variações claras e escuras;
- uso emocional da cor;
- proporção recomendada.

### 8.5 Direção de imagem

Definir o tratamento visual de imagens:

- fotografia;
- ilustração;
- 3D;
- colagem;
- mockup;
- textura;
- pessoas;
- produto;
- ambiente;
- movimento;
- enquadramento;
- luz;
- contraste;
- filtros;
- recortes.

### 8.6 Grafismos e elementos de apoio

Definir os elementos gráficos que reforçam a marca:

- linhas;
- formas;
- padrões;
- ícones;
- texturas;
- molduras;
- setas;
- módulos;
- cards;
- grids;
- elementos de dados;
- ilustrações secundárias.

### 8.7 Mensagem principal aplicada

Definir uma frase ou headline que represente a marca visualmente.

Exemplo:

```txt
Headline principal: Corra com inteligência. Evolua com consistência.
Subheadline: Um sistema de treino com IA para transformar dados em progresso real.
```

### 8.8 Aplicações derivadas

A partir do Key Visual, o sistema deve sugerir como ele pode ser desdobrado em:

- post de Instagram;
- capa de apresentação;
- landing page;
- anúncio digital;
- banner;
- tela inicial de app;
- capa de PDF;
- página de brand book;
- material institucional;
- carrossel;
- thumbnail;
- peça comercial.

---

## 9. Estrutura do arquivo gerado pela fase

O BrandOS deve gerar um arquivo chamado:

```txt
09-key-visual-direcao-aplicacoes.md
```

Conteúdo mínimo do arquivo:

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

---

## 10. Prompt interno para geração da fase

Use o prompt abaixo dentro do agente responsável pela fase de Key Visual.

```txt
Você é o agente de Key Visual do BrandOS.

Sua função é transformar a estratégia, o Brand DNA, a identidade verbal e o universo visual da marca em uma direção visual aplicada e coesa.

Você não deve criar apenas uma arte isolada. Você deve construir a imagem-mãe da marca: uma referência visual central capaz de orientar todos os layouts e aplicações futuras.

Use os dados já consolidados nas fases anteriores:

- briefing;
- diagnóstico;
- posicionamento;
- proposta de valor;
- personalidade;
- Brand DNA;
- tom de voz;
- mensagens-chave;
- universo visual;
- paleta de cores;
- tipografia;
- moodboard;
- estilo gráfico;
- referências visuais;
- canais prioritários.

Gere uma documentação completa contendo:

1. conceito visual central;
2. objetivo do Key Visual;
3. descrição da composição principal;
4. orientação de grid;
5. hierarquia visual;
6. direção tipográfica aplicada;
7. direção cromática aplicada;
8. estilo de imagem;
9. grafismos e elementos de apoio;
10. headline principal aplicada;
11. variações possíveis;
12. aplicações recomendadas;
13. regras de consistência;
14. checklist de validação.

A resposta deve ser clara, didática, aplicável e conectada ao projeto da marca.
Explique conceitos quando necessário, mas mantenha a linguagem prática para designers, criadores, empreendedores e usuários não especialistas.
```

---

## 11. Agente responsável

Adicionar um novo agente ao sistema:

```txt
Agent: Key Visual Director
```

### Função

Transformar a identidade visual conceitual em uma direção visual aplicada.

### Responsabilidades

- interpretar estratégia e Brand DNA;
- consolidar o universo visual;
- definir a composição-mãe da marca;
- orientar o uso aplicado de cores e tipografias;
- definir estilo de imagem e grafismos;
- criar lógica de desdobramento visual;
- preparar a marca para layouts finais;
- garantir consistência entre identidade e aplicação.

### Inputs

- outputs do Strategy Agent;
- outputs do Brand DNA Agent;
- outputs do Verbal Identity Agent;
- outputs do Visual Identity Agent;
- moodboard;
- paleta;
- tipografia;
- canais prioritários;
- objetivos de aplicação.

### Outputs

- Key Visual documentado;
- direção visual aplicada;
- regras de composição;
- variações do sistema visual;
- recomendações para layouts;
- checklist de consistência.

---

## 12. Subagentes recomendados

O agente de Key Visual pode acionar subagentes especializados.

### 12.1 Composition Subagent

Responsável por definir:

- grid;
- hierarquia;
- disposição dos elementos;
- ritmo visual;
- proporção;
- áreas de respiro;
- contraste.

### 12.2 Typography Application Subagent

Responsável por definir:

- uso real das fontes;
- títulos;
- subtítulos;
- chamadas;
- CTAs;
- números;
- espaçamentos;
- contraste tipográfico.

### 12.3 Color Application Subagent

Responsável por definir:

- proporção cromática;
- fundos;
- contrastes;
- cores de ação;
- cores emocionais;
- variações de aplicação.

### 12.4 Image Direction Subagent

Responsável por definir:

- fotografia;
- ilustração;
- textura;
- enquadramento;
- luz;
- estilo visual;
- tratamento de imagem.

### 12.5 Graphic Assets Subagent

Responsável por definir:

- grafismos;
- padrões;
- formas;
- ícones;
- linhas;
- elementos modulares;
- sistema de apoio visual.

### 12.6 Application System Subagent

Responsável por sugerir desdobramentos em:

- social media;
- landing page;
- apresentação;
- relatório;
- anúncio;
- app;
- materiais comerciais.

---

## 13. Integração com PRD, Spec e Scaffold

A fase de Key Visual deve ser refletida também nos documentos técnicos do BrandOS.

### 13.1 Atualização no PRD

Adicionar ao PRD:

```md
## Feature: Key Visual & Direção de Aplicações

### Objetivo
Permitir que o BrandOS gere uma direção visual aplicada antes da criação de layouts finais, garantindo consistência entre estratégia, identidade visual e aplicações práticas.

### Problema que resolve
Evita que os layouts sejam gerados sem uma referência visual central, reduzindo inconsistência estética entre peças.

### Usuário beneficiado
Designers, empreendedores, criadores de marca, equipes de marketing, founders e usuários não especialistas que precisam visualizar como a marca se comporta na prática.

### Resultado esperado
Um documento estruturado com o Key Visual da marca, contendo conceito, composição, tipografia aplicada, cor aplicada, imagem, grafismos, aplicações derivadas e checklist de consistência.
```

### 13.2 Atualização na Spec

Adicionar à Spec:

```md
## Spec: Key Visual Generation

### Trigger
Executar após a conclusão da fase de Universo Visual.

### Required Inputs
- brand_name
- segment
- target_audience
- positioning
- brand_dna
- verbal_identity
- color_palette
- typography
- visual_references
- image_style
- application_goals

### Processing Rules
- Não gerar layouts finais antes de consolidar a direção visual aplicada.
- Usar o Brand DNA como filtro de consistência.
- Validar se a direção visual reforça o posicionamento.
- Criar pelo menos uma composição principal e variações de aplicação.
- Gerar checklist final antes de liberar para a fase de Propostas de Layout.

### Output
- 09-key-visual-direcao-aplicacoes.md
- key_visual_summary
- application_guidelines
- consistency_checklist
```

### 13.3 Atualização no Scaffold

Adicionar nova pasta ou arquivo:

```txt
/brandos-project
  /09-key-visual
    09-key-visual-direcao-aplicacoes.md
    key-visual-summary.md
    application-guidelines.md
    consistency-checklist.md
```

Ou, se mantiver dentro de identidade visual:

```txt
/04-identidade-visual
  moodboard.md
  paleta.md
  tipografia.md
  grafismos.md
  key-visual.md
  direcao-aplicacoes.md
```

---

## 14. Integração com a Fase de Consolidação Pós-Briefing

Na Fase de Consolidação Pós-Briefing, adicionar uma nova opção para o usuário.

### Fluxo anterior

Após o briefing, o usuário podia escolher:

1. gerar PDF completo;
2. avançar para propostas de layout;
3. revisar respostas.

### Fluxo atualizado

Após o briefing e a consolidação das bases da marca, o sistema deve perguntar:

```txt
Agora que consolidamos a base da marca, o que você deseja fazer?

1. Gerar o PDF completo da marca.
2. Criar o Key Visual da marca antes dos layouts.
3. Avançar para propostas de layout.
4. Revisar alguma etapa anterior.
5. Exportar arquivos estruturados do projeto.
```

### Regra importante

Se o usuário escolher “propostas de layout” sem ter criado o Key Visual, o sistema deve recomendar:

```txt
Antes de criar os layouts, recomendo gerar o Key Visual da marca. Ele funciona como a imagem-mãe do sistema visual e ajuda a manter consistência em todas as peças. Deseja gerar o Key Visual agora?
```

Se o usuário disser não, o sistema pode avançar, mas deve registrar:

```txt
Key Visual não gerado. Layouts serão criados com base apenas no universo visual existente.
```

---

## 15. Integração com Propostas de Layout

A fase de Propostas de Layout deve usar o Key Visual como referência obrigatória quando ele existir.

### Regra

```txt
Se key_visual existe:
    usar key_visual como base para todos os layouts.
Se key_visual não existe:
    usar universo_visual + brand_dna + posicionamento.
```

### Aplicações possíveis

O sistema pode gerar propostas para:

- landing page;
- post de Instagram;
- carrossel;
- capa de apresentação;
- anúncio;
- banner;
- tela inicial de app;
- capa de relatório;
- página editorial;
- peça institucional;
- material comercial;
- identidade de campanha.

Cada layout deve informar:

- qual elemento do Key Visual foi usado;
- como a paleta foi aplicada;
- como a tipografia foi aplicada;
- qual grafismo foi usado;
- qual lógica de composição foi seguida;
- como a peça mantém consistência com a marca.

---

## 16. Integração com o PDF final Swiss Editorial Layout

O BrandOS já possui uma diretriz para gerar o PDF final com base em **Swiss Editorial Layout / Swiss Style Design**.

A fase de Key Visual deve alimentar esse PDF.

### No PDF final, incluir uma seção chamada:

```txt
Key Visual & Direção de Aplicações
```

### Essa seção deve conter:

- explicação do conceito visual central;
- composição principal;
- uso aplicado de cores;
- uso aplicado de tipografia;
- estilo de imagem;
- grafismos;
- variações;
- exemplos de aplicação;
- regras de consistência.

### Direção editorial Swiss para essa seção

A seção deve seguir:

- grid limpo;
- hierarquia tipográfica forte;
- bastante respiro;
- alinhamento preciso;
- uso racional de colunas;
- contraste entre título, corpo e legendas;
- organização visual clara;
- estética de brand book profissional.

---

## 17. Checklist de validação do Key Visual

Antes de liberar a fase, o sistema deve validar:

```md
# Checklist de Key Visual

- [ ] O Key Visual reflete o posicionamento da marca?
- [ ] O Key Visual traduz o Brand DNA?
- [ ] A composição tem hierarquia clara?
- [ ] A paleta foi aplicada de forma coerente?
- [ ] A tipografia foi aplicada de forma funcional?
- [ ] O estilo de imagem está alinhado ao território visual?
- [ ] Os grafismos reforçam a identidade da marca?
- [ ] O sistema visual pode ser desdobrado em diferentes peças?
- [ ] Existe consistência entre verbal e visual?
- [ ] O Key Visual ajuda a orientar layouts futuros?
- [ ] A direção visual está clara para designers e não designers?
- [ ] O material pode entrar no PDF final da marca?
```

---

## 18. Regras de qualidade

O Key Visual gerado pelo BrandOS deve ser:

- estratégico;
- visualmente coerente;
- aplicável;
- fácil de entender;
- conectado ao Brand DNA;
- conectado ao universo verbal;
- escalável para múltiplas peças;
- útil para designers;
- compreensível para usuários não especialistas;
- pronto para orientar o brand book.

Não deve ser:

- genérico;
- apenas decorativo;
- desconectado da estratégia;
- excessivamente subjetivo;
- limitado a uma única peça;
- incompatível com o público da marca;
- contraditório com o tom de voz;
- difícil de aplicar.

---

## 19. Exemplo aplicado — marca fictícia Track Running

### Contexto

```txt
Marca: Track Running
Segmento: esporte, corrida e fitness
Objetivo: criar uma marca para um aplicativo de treinos de corrida com IA
Personalidade: energética, inteligente, acessível e motivadora
Território visual: performance, tecnologia, movimento e evolução
```

### Key Visual sugerido

```txt
O Key Visual da Track Running deve traduzir a ideia de movimento inteligente. A composição principal pode combinar uma imagem de corredor em movimento com linhas de rota, módulos de dados, marcações de progresso e tipografia forte.

A estética deve parecer esportiva e tecnológica, mas sem ser fria. O sistema visual deve equilibrar performance e proximidade humana.
```

### Elementos visuais

```txt
- Foto ou silhueta de corredor em movimento.
- Linhas que simulam trajeto, rota ou batimento.
- Cards de dados com ritmo, distância, evolução e meta.
- Paleta vibrante com contraste alto.
- Tipografia sem serifa, forte e limpa.
- Grid dinâmico inspirado em movimento.
- Headline curta e motivadora.
```

### Headline possível

```txt
Corra com inteligência. Evolua com consistência.
```

### Aplicações derivadas

```txt
- Capa de app.
- Landing page.
- Post de lançamento.
- Banner de campanha.
- Apresentação para investidores.
- Brand book.
- Tela inicial do produto.
```

---

## 20. Comando sugerido

Adicionar comando específico ao BrandOS:

```txt
/gerar-key-visual
```

Ou em inglês:

```txt
/generate-key-visual
```

### Comportamento do comando

Quando acionado, o sistema deve:

1. verificar se as fases anteriores existem;
2. ler Brand DNA, verbal identity e universo visual;
3. identificar lacunas;
4. gerar a direção de Key Visual;
5. salvar o arquivo `09-key-visual-direcao-aplicacoes.md`;
6. atualizar o resumo do projeto;
7. liberar a etapa de propostas de layout.

---

## 21. Regra para memória persistente

O BrandOS deve salvar o Key Visual como parte da memória da marca.

Adicionar ao Brand Memory:

```json
{
  "key_visual": {
    "concept": "",
    "composition_direction": "",
    "typography_application": "",
    "color_application": "",
    "image_direction": "",
    "graphic_assets": [],
    "main_headline": "",
    "application_rules": [],
    "status": "draft | approved | skipped"
  }
}
```

---

## 22. Critérios de aprovação

A fase só deve ser considerada concluída quando:

1. o conceito visual central estiver claro;
2. os elementos principais estiverem definidos;
3. houver orientação de composição;
4. houver orientação de cor aplicada;
5. houver orientação de tipografia aplicada;
6. houver estilo de imagem definido;
7. houver grafismos definidos;
8. houver aplicações sugeridas;
9. houver checklist de consistência;
10. o usuário aprovar ou solicitar ajustes.

Mensagem final da fase:

```txt
O Key Visual da marca foi estruturado. Ele agora pode servir como base para as propostas de layout, o relatório final em PDF e os desdobramentos visuais da marca.

Está tudo correto por aqui? Quer voltar em alguma etapa? Sim ou não? Finalizar.
```

---

## 23. Atualização resumida para colar no sistema

```md
# Atualização BrandOS — Key Visual & Direção de Aplicações

Adicionar ao BrandOS uma nova fase chamada `Key Visual & Direção de Aplicações`, posicionada após `Universo Visual` e antes de `Propostas de Layout`.

Essa fase deve transformar estratégia, Brand DNA, identidade verbal e universo visual em uma imagem-mãe da marca, documentando conceito visual central, composição, tipografia aplicada, cor aplicada, estilo de imagem, grafismos, headline principal, variações, aplicações recomendadas e checklist de consistência.

A fase deve gerar o arquivo `09-key-visual-direcao-aplicacoes.md` e alimentar as etapas seguintes: propostas de layout, PDF final em Swiss Editorial Layout, guidelines e design system.

Adicionar o agente `Key Visual Director`, responsável por consolidar a direção visual aplicada da marca.

O sistema deve recomendar a geração do Key Visual antes de criar layouts. Caso o usuário pule essa etapa, registrar que os layouts foram gerados sem Key Visual aprovado.
```

---

## 24. Instrução final para o Claude Code

```txt
Atualize o projeto BrandOS incorporando a fase `Key Visual & Direção de Aplicações` ao workflow principal.

A fase deve ser posicionada depois de `Universo Visual` e antes de `Propostas de Layout`.

Crie ou atualize os seguintes pontos:

1. workflow principal;
2. PRD;
3. Spec;
4. Scaffold;
5. agentes;
6. subagentes;
7. memória persistente da marca;
8. fase de consolidação pós-briefing;
9. propostas de layout;
10. exportação do PDF final em Swiss Editorial Layout.

Garanta que o Key Visual funcione como ponte entre estratégia e aplicação visual, evitando que o sistema gere layouts finais sem uma direção visual consolidada.

O output principal da fase deve ser:

`09-key-visual-direcao-aplicacoes.md`

Esse arquivo deve conter:

- conceito visual central;
- objetivo do Key Visual;
- composição principal;
- grid;
- hierarquia visual;
- tipografia aplicada;
- cor aplicada;
- estilo de imagem;
- grafismos;
- headline principal;
- variações;
- aplicações recomendadas;
- regras de consistência;
- checklist final.
```

---

## 25. Resultado esperado da atualização

Com essa atualização, o BrandOS passa a ter uma etapa intermediária mais profissional entre identidade visual e layout final.

O sistema deixa de apenas definir elementos visuais separados e passa a construir uma linguagem visual aplicada, capaz de orientar toda a produção gráfica da marca.

Essa fase fortalece:

- a consistência visual;
- a qualidade dos layouts;
- a geração do brand book;
- a clareza para o usuário;
- a ponte entre marca e produto;
- a aplicação profissional da identidade;
- a experiência final do BrandOS como sistema de branding guiado por IA.

