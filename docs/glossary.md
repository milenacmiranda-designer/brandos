# Glossário do BrandOS

Definições dos principais termos usados no sistema.

---

## Termos de branding

**Brand DNA**
A fonte única da verdade da marca. Arquivo consolidado (`brand-dna.json`) que contém essência, propósito, valores, personalidade, posicionamento e princípios verbais e visuais. Tudo deriva dele.

**Brand System**
O conjunto completo de elementos que formam a identidade de uma marca: estratégia, verbal e visual, com diretrizes de aplicação. O BrandOS entrega o brand system em `brand-system.md`.

**Brand Book**
Documento que organiza e documenta todos os elementos do brand system. É o entregável final da fase 13.

**Posicionamento**
O espaço que a marca ocupa na mente do público. Define como a marca se diferencia dos concorrentes e por que o público deveria escolhê-la.

**Proposta de Valor**
O benefício central que a marca oferece ao público. Responde: por que comprar de você e não do concorrente?

**Persona**
Representação semi-fictícia do cliente ideal. Não é um dado demográfico — é um perfil com dores, desejos, medos, comportamentos e linguagem.

**Arquétipo**
Modelo de personalidade baseado nos 12 arquétipos de Jung, adaptados para branding. Orienta comportamento comunicacional e tom de voz.

**Tom de Voz**
Como a marca fala — não o que ela diz, mas o estilo, a atitude e o ritmo da comunicação.

**Território de Marca**
O espaço conceitual que a marca ocupa — a ideia central que diferencia e orienta todas as decisões de comunicação.

**Manifesto**
Texto que declara o propósito e a visão da marca. Captura o porquê de existir e convoca o público para essa visão.

**Identidade Verbal**
O conjunto de elementos que define como a marca se comunica: tom de voz, vocabulário, mensagens, tagline, manifesto, bios.

**Identidade Visual Conceitual**
A direção que orienta as escolhas visuais: conceito, paleta, tipografia, estilo gráfico, estilo fotográfico. Não é execução — é direção.

---

## Termos do sistema

**Agent**
Componente que executa uma fase específica do pipeline. Cada agente tem função clara, entrada definida, saída esperada e limites de atuação.

**Subagent**
Especialista menor que ajuda agentes principais em tarefas pontuais (naming, tagline, paleta, tipografia...).

**Skill**
Habilidade reutilizável que pode ser usada por diferentes agentes. Encapsula um processo específico.

**Gate**
Ponto de controle obrigatório que bloqueia o avanço até ser aprovado. O BrandOS tem dois gates: Brand DNA (fase 8) e Governance + QA (fase 12).

**Scaffold**
Estrutura inicial de pastas e arquivos do projeto.

**Harness**
Documento de controle, teste e auditoria do sistema (`BRANDOS_HARNESS.md`).

**Score**
Pontuação de qualidade de 0 a 100. Score mínimo para exportação: 70. Score recomendado: 80+.

**Pipeline**
A sequência de 14 fases que o BrandOS executa para criar um brand system completo.

**Memória Persistente**
Sistema de 8 arquivos JSON que armazena decisões, progresso e contexto da marca para garantir consistência entre fases e permitir retomada.
