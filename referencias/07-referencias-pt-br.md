# Referências em PT-BR

> Materiais de alta qualidade em Português para complementar as referências principais.

---

## Cultura IA-First & Adoção

### [IA Generativa além do hype: da produtividade à resistência nas empresas — Hipsters.Talks #04](https://www.hipsters.tech/ia-generativa-alem-do-hype-da-produtividade-a-resistencia-nas-empresas-ft-patricia-prado-04/)
**Fonte:** Hipsters Ponto Tech (Alura/Caelum) — Paulo Silveira entrevista Patrícia Prado (Líder de IA Generativa na Accenture) | **Ano:** 2025

**Contexto de aplicabilidade:** Episódio denso sobre a diferença entre adoção superficial e transformação real de processos com IA generativa em grandes organizações. Prado distingue casos onde houve ganho de 100x em produção de conteúdo versus iniciativas que emperraram na resistência cultural — o argumento central é que mudança de cultura e treinamento precedem qualquer resultado técnico. Diretamente aplicável a times que estão além do piloto e enfrentam a fase de escala.

---

### [Coding Agents na Prática: Claude Code, Cursor e Cia. — Hipsters Ponto Tech #511](https://www.hipsters.tech/coding-agents-na-pratica-claude-code-cursor-e-cia-hipsters-ponto-tech-511/)
**Fonte:** Hipsters Ponto Tech (Alura) — Paulo Silveira, Mauricio Aniche (CTO Alura), Rafael Ribeiro (CTO StartSe), Vinny Neves, Crisley Marques | **Ano:** 2026

**Contexto de aplicabilidade:** Discussão técnica e honesta entre praticantes sobre como coding agents (Claude Code, Cursor, Windsurf, Copilot, Augment) estão mudando o fluxo real de trabalho de engenheiros sênior — incluindo o fenômeno de profissionais experientes voltando a codar ativamente. Aborda diferenças práticas entre uso via CLI versus IDE, e o que é hype vs. ganho real de velocidade. Referência obrigatória para times calibrando sua adoção de agentes de codificação.

---

## Arquitetura de Software

### [QTrends Arquitetura — A ascensão e queda dos microservices](https://www.infoq.com/br/news/2020/06/qtrends-arquitetura-microservice/)
**Fonte:** InfoQ Brasil — Leandro Guimarães e Daniel Bryant | **Ano:** 2020

**Contexto de aplicabilidade:** Análise crítica do ciclo de hype dos microsserviços a partir de casos reais: o estudo da Segment, que migrou de monólito para microsserviços e depois reverteu a decisão por custo operacional insustentável, é o exemplo mais citado. O artigo cunha o anti-padrão "monólito distribuído" — quando serviços independentes exigem deploys sincronizados, eliminando o principal benefício da arquitetura. Leitura essencial antes de qualquer decisão de decomposição.

### [QTrends Arquitetura — A vez dos monólitos modulares](https://www.infoq.com/br/news/2020/07/qtrends-monolitos-modulares/)
**Fonte:** InfoQ Brasil — Leandro Guimarães e Daniel Bryant | **Ano:** 2020

**Contexto de aplicabilidade:** Artigo complementar ao anterior que apresenta o monólito modular como alternativa arquitetural legítima, não como solução de segunda classe. Traz a citação de Sam Newman — "microsserviços não devem ser sua escolha padrão" — e discute como DDD pode guiar a identificação de fronteiras de módulos antes de qualquer decomposição. Relevante para times que ainda operam monólitos e precisam de vocabulário técnico para justificar a decisão de não migrar.

### [Desafios e soluções: Evolução da arquitetura tecnológica – do monolito para microsserviços](https://www.infoq.com/br/presentations/desafios-solucoes-evolucao-da-arquitetura/)
**Fonte:** InfoQ Brasil / DevCamp — Ulisses Maeda (Solutions Architect, 14 anos em fintechs) | **Ano:** 2019

**Contexto de aplicabilidade:** Apresentação de 40 minutos com foco em como conduzir a migração de monólito para microsserviços sem impactar o negócio em produção — especialmente relevante para contextos financeiros regulados. Maeda detalha as técnicas práticas usadas por seu time, incluindo estratégias de strangler fig e particionamento incremental. Diferencia-se de conteúdo teórico por partir de uma execução real em ambiente de alta criticidade.

---

## Domain-Driven Design

### [Lambda3 Podcast #14 — Domain Driven Design](https://www.lambda3.com.br/2016/10/podcast-14-domain-driven-design/)
**Fonte:** Lambda3 Podcast — Giovanni Bassi, Abner das Dores, Heber Pereira, Thiago Holder, Vinicius Quaiato | **Ano:** 2016

**Contexto de aplicabilidade:** Episódio de 73 minutos conduzido por praticantes experientes de DDD no Brasil, cobrindo Linguagem Ubíqua, Bounded Contexts, Aggregates e os principais erros de implementação que times cometem ao adotar DDD pela primeira vez. Embora de 2016, os conceitos são atemporais e a discussão em PT-BR com exemplos brasileiros o torna mais acessível do que os livros canônicos. Serve como ponto de entrada para equipes que precisam calibrar o vocabulário antes de aplicar DDD em microsserviços ou monólitos modulares.

### [DDD e Microsserviços — Do negócio à arquitetura](https://www.lambda3.com.br/2019/08/ddd-e-microsservicos-do-negocio-a-arquitetura/)
**Fonte:** Lambda3 Blog | **Ano:** 2019

**Contexto de aplicabilidade:** Artigo que conecta diretamente os conceitos estratégicos de DDD (Bounded Contexts, Context Maps) às decisões de decomposição em microsserviços — preenchendo a lacuna entre o aprendizado teórico de DDD e sua aplicação como ferramenta de design arquitetural. Recomendado para times que já conhecem DDD tático e precisam avançar para o design estratégico como base de decisões de serviços.

---

## Team Topologies

### [Review do Livro — Team Topologies](https://diegoeis.com/review-livro-team-topologies/)
**Fonte:** Blog Diego Eis (autor e product manager referência no Brasil) | **Ano:** 2021

**Contexto de aplicabilidade:** Resenha técnica densa que vai além da descrição das quatro topologias e articula o porquê estrutural do framework: como a Lei de Conway, o número de Dunbar e o conceito de carga cognitiva se combinam para produzir (ou destruir) fluxo de entrega. Diego Eis critica e conecta os conceitos com honestidade, apontando onde o livro é prescritivo demais. Útil para engenheiros e tech leads que querem internalizar os fundamentos antes de propor mudanças organizacionais.

### [Construção de times com Team Topologies](https://eduardohattorif.medium.com/constru%C3%A7%C3%A3o-de-times-com-team-topologies-b8b6999e7e7e)
**Fonte:** Medium — Eduardo Hattori | **Ano:** 2022

**Contexto de aplicabilidade:** Artigo prático em PT-BR que explica as quatro topologias e os três modos de interação (colaboração, X-as-a-Service, facilitação) com exemplos aplicados. Destaca a aplicação reversa da Lei de Conway — estruturar times deliberadamente para produzir a arquitetura desejada — e discute como gerenciar carga cognitiva como variável de design organizacional. Bom ponto de partida para times que precisam de um guia de leitura rápida antes de apresentar o framework para liderança.

---

*Nota: A maioria das referências canônicas neste programa está em inglês. Este arquivo reúne o melhor do conteúdo PT-BR disponível — priorize qualidade sobre quantidade.*

*Sobre lacunas: Não foi encontrado conteúdo PT-BR de qualidade técnica suficiente sobre Team Topologies em fontes como Zup, iMasters ou InfoQ Brasil — o tema ainda é predominantemente coberto em inglês no Brasil. Para Agentes de IA em desenvolvimento de software além do episódio Hipsters #511, o conteúdo PT-BR disponível é majoritariamente introdutório; as referências técnicas de profundidade neste tema permanecem em inglês (ver `06-rag-e-agentes.md`).*
