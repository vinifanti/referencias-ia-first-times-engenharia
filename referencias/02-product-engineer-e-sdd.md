# Referências: Product Engineer & Discovery Técnico

## Referências Principais

### [The Product-Minded Software Engineer](https://blog.pragmaticengineer.com/the-product-minded-engineer/)
**Fonte:** Gergely Orosz — The Pragmatic Engineer | **Ano:** 2019 (atualizado 2022)
**Contexto de aplicabilidade:** Artigo fundacional que define as 9 características do engenheiro orientado a produto: curiosidade sobre o "porquê" das decisões, compreensão do modelo de negócio, capacidade de equilibrar trade-offs técnicos e de produto, e ownership do ciclo completo (da ideia à métrica de uso real). Referência essencial para equipes que querem reduzir a dependência de PMs como "tradutores" e aproximar engenheiros do contexto de negócio. Gergely publicou posteriormente um livro homônimo pela O'Reilly expandindo o tema.

---

### [Inside Stripe's Engineering Culture — Part 2](https://newsletter.pragmaticengineer.com/p/stripe-part-2)
**Fonte:** Gergely Orosz — The Pragmatic Engineer | **Ano:** 2022
**Contexto de aplicabilidade:** Descreve como a Stripe operou por anos sem PMs dedicados, exigindo que engenheiros participassem de toda a jornada: escopo de negócio, pesquisa com usuários, colaboração com designers, jurídico e financeiro. Documenta também práticas como "friction logs" (registro estruturado de pontos de atrito na jornada do usuário) e a cultura de escrita que multiplica o alcance de decisões técnicas. Modelo concreto para equipes que querem ampliar a ownership dos engenheiros além do código.

---

### [Inside Figma's Engineering Culture](https://newsletter.pragmaticengineer.com/p/inside-figmas-engineering-culture)
**Fonte:** Gergely Orosz — The Pragmatic Engineer | **Ano:** 2022
**Contexto de aplicabilidade:** Revela como a Figma estrutura engenharia em "produto vertical + features compartilhadas + fundação", promovendo ownership end-to-end por área de produto. Engenheiros participam ativamente de design critiques, são envolvidos nas fases de exploração antes do planejamento formal, e mantêm contato direto com clientes (inclusive o CTO entra em chamadas de debugging). Referência para equipes que querem implementar descoberta colaborativa entre engenharia e design sem processos pesados.

---

### [How Linear Builds Product](https://www.lennysnewsletter.com/p/how-linear-builds-product)
**Fonte:** Lenny Rachitsky — Lenny's Newsletter (entrevista com Karri Saarinen, co-fundador da Linear) | **Ano:** 2023
**Contexto de aplicabilidade:** Documenta como a Linear opera sem PMs tradicionais — engenheiros e designers fazem o papel de PM nos projetos, formam times pequenos (1 designer + 2 engenheiros), escrevem specs detalhadas antes de implementar, e usam "taste and opinions" em vez de A/B testing para decisões de produto. A prática de escrever especificações de projeto como artefato central antes da implementação é diretamente aplicável a equipes adotando desenvolvimento orientado a spec.

---

### [Linear: Move Fast with Little Process](https://newsletter.pragmaticengineer.com/p/linear-move-fast-with-little-process)
**Fonte:** Gergely Orosz — The Pragmatic Engineer | **Ano:** 2024
**Contexto de aplicabilidade:** Análise do modelo de engenharia da Linear com foco em como manter alta velocidade e qualidade com processo mínimo: zero-bug policy, comunicação por princípios (não por manuais), e engenheiros com forte intuição de produto. Mostra que a viabilidade do modelo depende de contratar engenheiros com senso de produto e manter times pequenos — contexto importante para equipes avaliando até onde podem ir sem estrutura formal de PM.

---

### [A Practical Guide to Writing Technical Specs](https://stackoverflow.blog/2020/04/06/a-practical-guide-to-writing-technical-specs/)
**Fonte:** Zara Cooper — Stack Overflow Blog | **Ano:** 2020
**Contexto de aplicabilidade:** Guia prático com estrutura em 8 seções para escrever especificações técnicas eficazes: front matter, introdução, soluções (atual e proposta), considerações adicionais (segurança, custos, riscos), avaliação de sucesso, breakdown de trabalho, deliberação (questões em aberto) e encerramento. Útil para equipes que precisam padronizar Technical Design Docs (TDDs) sem over-engineering — serve como template imediato para engenheiros que nunca escreveram TDDs formais.

---

### [How to Write PRDs for AI Coding Agents](https://medium.com/@haberlah/how-to-write-prds-for-ai-coding-agents-d60d72efb797)
**Fonte:** David Haberlah — Medium | **Ano:** 2026
**Contexto de aplicabilidade:** Articula a mudança de paradigma: PRDs para agentes de IA não são documentos de alinhamento humano, mas interfaces de programação — especificações que funcionam como contrato entre intenção e execução. Propõe arquitetura sequencial Especificar → Planejar → Tarefas → Implementar, com critérios de aceite verificáveis por máquina (quantitativos, sem linguagem qualitativa vaga como "fácil de usar"), seções explícitas de "NÃO ALTERAR" para prevenir escopo creep, e fases de pesquisa obrigatórias para evitar que agentes implementem APIs depreciadas.

---

### [Vertical Slicing: User Stories and Acceptance Criteria](https://dev.to/jan/user-stories-and-vertical-slicing-1dpo)
**Fonte:** Jan — DEV Community | **Ano:** 2021
**Contexto de aplicabilidade:** Explica a diferença entre fatias verticais (funcionalidade end-to-end com valor para o usuário, testável e demonstrável) e fatias horizontais (separação por camada técnica). Fatias verticais são o método recomendado para backlog de times ágeis porque permitem feedback rápido, deployment incremental, e identificação precoce de dependências. Diretamente aplicável ao processo de escrita de acceptance criteria e quebra de user stories em tarefas implementáveis por agentes de IA.

---

---

# Referências: Harness, Spec-Driven Development & Code Review com IA

## Referências Principais

### [Harness Engineering for Coding Agent Users](https://martinfowler.com/articles/harness-engineering.html)
**Fonte:** Birgitta Böckeler (Distinguished Engineer, Thoughtworks) — martinfowler.com | **Ano:** 2026
**Contexto de aplicabilidade:** Artigo seminal que define "harness engineering" — tudo no agente de IA exceto o modelo em si. Categoriza controles em "guias" (feedforward, previnem problemas) e "sensores" (feedback, detectam desvios), e organiza o harness em três camadas: manutenibilidade do código, fitness arquitetural e corretude funcional. Essencial para equipes estruturando pipelines de CI/CD, linters, e revisão de código como parte do harness de qualidade para código gerado por IA.

---

### [Spec-Driven Development with AI: Get Started with a New Open Source Toolkit](https://github.blog/ai-and-ml/generative-ai/spec-driven-development-with-ai-get-started-with-a-new-open-source-toolkit/)
**Fonte:** Den Delimarsky — GitHub Blog | **Ano:** 2025
**Contexto de aplicabilidade:** Introduz o processo de quatro fases do Spec Kit (Especificar → Planejar → Tarefas → Implementar) como forma de eliminar o "vibe coding" e tornar agentes de IA previsíveis em projetos reais. Cada tarefa deve ser pequena o suficiente para ser implementada e testada em isolamento, e a especificação atua como contrato central verificável. Compatível com GitHub Copilot, Claude Code e Gemini CLI — referência prática para equipes que querem adotar SDD com ferramentas open source.

---

### [Spec-Driven Development: Unpacking One of 2025's Key New Practices](https://thoughtworks.medium.com/spec-driven-development-d85995a81387)
**Fonte:** Liu Shangqi (Technology Director APAC, Thoughtworks) — Medium | **Ano:** 2025
**Contexto de aplicabilidade:** Perspectiva crítica e balanceada sobre SDD da Thoughtworks: especificações devem incluir mapeamentos de input/output, pré/pós-condições, invariantes, contratos de integração e lógica de máquina de estados. O autor alerta que SDD não é waterfall acelerado — exige loops de feedback curtos e práticas determinísticas de CI/CD para compensar a não-determinismo da geração de código. Boa referência para equipes que querem implementar SDD de forma responsável, com consciência dos desafios de "spec drift" e alucinação.

---

### [How Spec-Driven Development Improves AI Coding Quality](https://developers.redhat.com/articles/2025/10/22/how-spec-driven-development-improves-ai-coding-quality)
**Fonte:** Rich Naszcyniec — Red Hat Developer | **Ano:** 2025
**Contexto de aplicabilidade:** Contrasta "vibe coding" (interações improvisadas com IA) com "spec coding" (especificação em camadas antes de gerar código), relatando 95%+ de acurácia na implementação na primeira tentativa com código unit-testado. A prática de manter um arquivo "LessonsLearned.md" com erros e correções cria um loop de melhoria contínua das specs ao longo do projeto. Útil para equipes que precisam de um framework pragmático de adoção imediata de SDD, com estrutura de pastas e prompts concretos.

---

### [TDD, AI Agents and Coding with Kent Beck](https://newsletter.pragmaticengineer.com/p/tdd-ai-agents-and-coding-with-kent)
**Fonte:** Gergely Orosz entrevistando Kent Beck — The Pragmatic Engineer Podcast | **Ano:** 2025
**Contexto de aplicabilidade:** Kent Beck, criador do TDD, afirma que testes se tornam um "superpoder" quando se trabalha com agentes de IA — a única forma confiável de evitar regressões silenciosas. Descreve agentes como "genies imprevisíveis" que concebem desejos de formas inesperadas, e relata o paradoxo de ter que impedir agentes de deletar testes para fazê-los "passar". Referência de autoridade máxima para justificar investimento em suítes de teste como mecanismo de controle de qualidade em pipelines com IA.

---

### [Harness Engineering: Structured Workflows for AI-Assisted Development](https://developers.redhat.com/articles/2026/04/07/harness-engineering-structured-workflows-ai-assisted-development)
**Fonte:** Marco Rizzi — Red Hat Developer | **Ano:** 2026
**Contexto de aplicabilidade:** Caso prático de transição de "prompt engineering" para "harness engineering" com dois problemas reais: a IA alucinava caminhos de arquivo e inventava APIs inexistentes quando o contexto era vago. A solução foi um workflow de duas fases — mapa de impacto no repositório (validado por humanos) seguido de template estruturado de tarefa com caminhos de arquivo reais, símbolos de código concretos e critérios de aceite explícitos. Diretamente aplicável a equipes construindo seu próprio harness de desenvolvimento com Claude Code ou Copilot.

---

### [To Vibe or Not to Vibe](https://martinfowler.com/articles/exploring-gen-ai/to-vibe-or-not-vibe.html)
**Fonte:** Birgitta Böckeler — martinfowler.com | **Ano:** 2025
**Contexto de aplicabilidade:** Framework de avaliação de risco em três dimensões para decidir quanta revisão aplicar a código gerado por IA: Probabilidade de erro (qualidade do contexto fornecido), Impacto (criticidade em produção), e Detectabilidade (cobertura de testes, sistema de tipos, familiaridade com o código). Permite que equipes calibrem rigor de revisão de PR por contexto em vez de aplicar o mesmo processo a todo código gerado — evita tanto paranoia paralisante quanto complacência perigosa.

---

### [Research, Review, Rebuild](https://martinfowler.com/articles/research-review-rebuild.html)
**Fonte:** Rahul Ramesh (Consultant Developer, Thoughtworks India) — martinfowler.com | **Ano:** 2025
**Contexto de aplicabilidade:** Metodologia de modernização de legado com IA em três fases: Research (análise do código existente via MCP para entender comportamentos sem suposições), Review (validação por especialistas humanos antes de implementar), e Rebuild (geração de código no stack-alvo com prompts estruturados e intenção clara). O caso Bahmni demonstra migração de AngularJS para React/TypeScript em menos de uma hora por ~$2, versus 3-6 dias manualmente — com revisão humana como gargalo real. Modelo replicável para times com dívida técnica expressiva.

---

### [5 Best Practices for Reviewing and Approving AI-Generated Code](https://brightsec.com/blog/5-best-practices-for-reviewing-and-approving-ai-generated-code/)
**Fonte:** Loris Gutić — Bright Security | **Ano:** 2026
**Contexto de aplicabilidade:** Define o modelo mental correto para revisão de código gerado por IA: tratar o output como "confidententemente incompleto" e de fonte externa não confiável, revisando comportamento e não apenas sintaxe. Atenção especial a auth/autorização (frequentemente atrelada à UI em vez de server-side) e estado. A prática de "exigir evidências, não explicações" — testes rodando em vez de comentários bem escritos — é diretamente aplicável a checklists de PR para times que já usam Copilot ou Claude Code.

---

### [AI Code Review Checklist: What to Check Before Merging AI-Generated Code](https://www.getmrq.com/blog/ai-code-review-checklist)
**Fonte:** mrq team | **Ano:** 2025
**Contexto de aplicabilidade:** Checklist prático e objetivo para revisores de PR organizados em três categorias: Segurança (credenciais hardcoded, SQL injection, XSS, defaults seguros), Lógica & Corretude (edge cases, error handling, off-by-one, async/await), e Manutenibilidade (nomes descritivos, complexidade desnecessária, código morto, alinhamento com padrões do projeto). Serve como template direto para o PR template da equipe, complementado com automação via ESLint e scanners de segurança estáticos.

---

### [Spec-Driven Development: From Code to Contract in the Age of AI Coding Assistants](https://arxiv.org/html/2602.00180v1)
**Fonte:** arXiv (preprint acadêmico) | **Ano:** 2026
**Contexto de aplicabilidade:** Paper acadêmico que formaliza SDD como paradigma onde a especificação é o artefato primário e o código é artefato derivado e verificável. Discute a tensão entre especificações como "guias para geração" versus "fonte de verdade absoluta", e propõe critérios formais para especificações executáveis (mapeamentos I/O, pré/pós-condições, invariantes). Útil para equipes que querem fundamentação teórica sólida ao apresentar SDD internamente ou escrever documentação de arquitetura do processo de desenvolvimento.
