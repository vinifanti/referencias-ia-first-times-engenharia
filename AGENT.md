## Estrutura de pastas
Verifique se existe a pasta .agents com a folders de skills, rules, agents etc.. se nao existir crie a estrutura.

## Objetivo do Projeto
Fazer Research, Plan e Implement (RPI) para pesquisar os topicos na seção de topicos na internet buscando os ultimos artigos de referencia da internet e criando materiais ajudar a desenvolver e aplicar os topicos no dia-a-dia do time de engenharia.

## Topicos para explorar
Fase 1 - FUNDAÇÕES

-> Onboarding / Cultura IA First
Objetivo: Construção de uma mentalidade IA-first — antes de qualquer ferramenta ou código.
›Critérios de sucesso da formação, uso da comunidade/WhatsApp e rotina semanal
›O que é cultura IA-first na prática: mentalidade, hábitos e comportamentos
›Como criar um ambiente onde experimentar com IA é esperado, não excepcional
›Princípios IA-first: velocidade de aprendizado, tolerância a erro controlado, compartilhamento, elevação coletiva


->Projeto IA-first: setup e entrega E2E com IA
Objetivo: Mostrar na prática como entregar uma feature completa usando IA como copiloto em todas as etapas — do scaffold ao PR.
›Como estruturar um projeto IA-first: pastas, contexto de codebase, rules e skills
›Workflow de entrega: scaffold → testes → implementação → PR
›Como dar instruções precisas para a IA, com restrições e checklists
›Quando confiar e quando revisar o output da IA

-> Product Engineer: Discovery técnico, PRDs, Design Docs e gerenciamento de backlog
Objetivo: Desenvolver a capacidade de usar IA para acelerar o processo de discovery e planejamento técnico sem perder profundidade e qualidade de decisão.
›O que é um Product Engineer: engenheiro que entende o problema, participa do discovery e decide com contexto de negócio (não é PM técnico, nem executor de ticket)
›Como estruturar um Technical Design Doc (TDD) leve e eficaz
›Uso de IA para explorar trade-offs, levantar riscos e gerar alternativas de design
›Escrita de PRDs com IA que realmente guiam a implementação
›Fatiamento vertical, critérios de aceite e sinais de risco no backlog
›Como manter previsibilidade de entrega sem microgestão

-> Harness, Spec-Driven Development e Code Review com IA
Objetivo: Construir uma base sólida de qualidade usando IA para escrever testes, investigar bugs e conduzir code reviews mais eficientes.
›Conceito de Harness: ambiente de testes e contexto para a IA gerar código mais seguro
›Spec-Driven Development: escrever a spec antes do código e deixar a IA implementar contra ela
›Geração de suites de teste com IA (unitários, integração, edge cases)
›Checklist de PR focado em segurança, performance e redução de regressões
›Como revisar código gerado por IA de forma crítica e eficiente

->Construindo uma empresa IA-first / Team Topologies
Objetivo: Entender como times e organizações de engenharia precisam se reorganizar para operar de forma IA-first — do modelo mental à estrutura de times.
›O que significa ser uma empresa IA-first (além de usar ferramentas)
›Team Topologies na era da IA: fronteiras, interações e autonomia com a IA como membro do time
›Casos reais de adoção em empresas de produto (perspectiva da LangWatch)
›Como o papel do tech lead muda quando a IA assume tarefas operacionais
›Onde a IA cria alavancagem e onde ainda precisa de supervisão humana

-> Como adotar IA de forma segura, criação de cultura e aplicação do framework de adoção
Objetivo: Aplicar um framework prático de adoção de IA no time — com foco em segurança, governança mínima e geração de cultura sustentável.
›Framework de adoção de IA: diagnóstico, onboarding gradual e métricas
›Como identificar resistências e criar aliados internos
›Framework de 7 fases: do diagnóstico de maturidade ao piloto, governança e escala corporativa
›Cada fase com critérios de entrada, métricas e conteúdo autossuficiente


-> Evolução Arquitetural na Era da IA: Monólito Modular, Microsserviços
Objetivo:Desenvolver critérios de decisão arquitetural claros para escolher e evoluir entre monólito modular e microsserviços — sem seguir modismos.
›Por que arquitetura importa ainda mais na era da IA
›Como saber se seu time está pronto para microsserviços (spoiler: a maioria não está)
›Monólito modular: módulos com boundaries claros, deploys independentes, baixo acoplamento
›Critérios de decisão: acoplamento de dados, frequência de deploy, autonomia, observabilidade, maturidade operacional
›Riscos comuns na transição e como mitigá-los

-> Refatoração Assistida por IA: Complexidade, DDD e Padrões
Objetivo: Usar IA para conduzir refatorações incrementais com segurança, aplicando DDD tático e design patterns para reduzir complexidade acidental.
›Complexidade acidental vs. essencial no código
›DDD tático na prática: Entities, Value Objects, Aggregates, Domain Services e Repositories
›IA para mapear bounded contexts, sugerir refatorações e gerar testes de cobertura antes de refatorar
›Design patterns na era da IA: quando usar, quando evitar
›Refatoração incremental: strangler fig, feature flags, migração sem big bang
›IA para manter consistência em refatorações grandes

-> Workflows avançados com IA
Objetivo: Dominar workflows de IA para tarefas de engenharia complexas — integrações, migrations, testes de integração e observabilidade — com a perspectiva de quem constrói ferramentas de IA para devs.
›Workflows de IA para tarefas de maior risco (migrations, contratos de API, refatorações em massa)
›Testes de integração gerados e mantidos com IA
›Observabilidade de sistemas que usam IA: traces, logs estruturados, alertas
›Agentes para tarefas repetitivas de engenharia: o que automatizar, o que manter humano
›Como os melhores devs usam o Cursor — o que diferencia os top 1%.


-> Evolução Arquitetural Frontend na Era da IA
Objetivo: Desenvolver critérios de decisão arquitetural claros para o frontend — entre monorepo, microfrontends e frontends modulares — sem seguir modismos.
›Por que arquitetura frontend importa mais quando a IA gera código em escala
›Monorepo vs. multi-repo: critérios baseados em autonomia, CI e acoplamento de componentes
›Microfrontends na prática: boundaries, composição (module federation, iframes, web components) e custos reais
›Frontends modulares sem microfrontends: boundaries e deploys independentes dentro de um único app
›Como a IA muda o custo de migração e refatoração de arquiteturas frontend
›Critérios para evoluir a arquitetura de forma incremental

-> Contexto Compartilhado, RAG, Padrões e Governança
Objetivo: Criar uma base de conhecimento compartilhada que a IA pode usar como memória do time — e estabelecer governança leve para escalar qualidade sem burocracia.
›Por que IA sem contexto de domínio gera código genérico — e como resolver
›RAG aplicado a codebases: indexar documentação, ADRs e padrões para a IA usar automaticamente
›Padrões compartilhados ensináveis: exemplos, rubricas e checklists que time e IA seguem
›ADRs: como escrever, manter e usar com IA
›Playbooks de qualidade: guidelines de code review, critérios de merge, boas práticas de IA
›Governança mínima viável: revisar e evoluir padrões sem criar processo pesado

-> Desenvolvimento de Agentes
Objetivo: Entender quando faz sentido construir agentes, como arquitetá-los de forma robusta e como integrá-los ao workflow de engenharia do time.
›O que é um agente de IA na prática e quando faz mais sentido que uma automação simples
›Anatomia de um agente: loop de raciocínio, ferramentas, memória, contexto
›Padrões de design para agentes confiáveis: falhas, loops, comportamentos inesperados
›Agentes para engenharia: code review, documentação, triagem de bugs
›Como testar e monitorar agentes em produção
›Quando NÃO construir um agente — e usar um workflow mais simples