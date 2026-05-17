# Referências: Contexto Compartilhado, RAG & Governança para Times de Engenharia

## Referências Principais

---

### [Building Effective Agents](https://www.anthropic.com/research/building-effective-agents)
**Fonte:** Anthropic (Erik Schluntz & Barry Zhang) | **Ano:** 2024
**Contexto de aplicabilidade:** Guia definitivo da Anthropic sobre quando e como construir sistemas agênticos. Distingue *workflows* (fluxos predefinidos) de *agentes autônomos* e apresenta os cinco padrões centrais de composição (chaining, routing, parallelization, orchestrator-workers, evaluator-optimizer). Recomenda fortemente começar pela solução mais simples possível e só adicionar complexidade agêntica quando soluções diretas se mostrarem insuficientes.

---

### [Documenting Architecture Decisions](https://www.cognitect.com/blog/2011/11/15/documenting-architecture-decisions)
**Fonte:** Michael Nygard / Cognitect | **Ano:** 2011
**Contexto de aplicabilidade:** Artigo seminal que popularizou os Architecture Decision Records (ADRs) — documentos leves que capturam o contexto, a decisão e as consequências de cada escolha arquitetural significativa. Nygard argumenta que documentos grandes nunca são mantidos atualizados, enquanto ADRs modulares em Markdown versionados junto ao código têm chance real de sobreviver. Referência obrigatória para qualquer time que queira fornecer contexto histórico à IA e a novos membros.

---

### [Architectural Decision Records (ADRs) — adr.github.io](https://adr.github.io/)
**Fonte:** ADR GitHub Organization | **Ano:** Mantido ativamente
**Contexto de aplicabilidade:** Hub central de recursos sobre ADRs: vocabulário padronizado, templates (incluindo o formato Y-statement), ferramentas de captura de decisões e referências à adoção em Azure Well-Architected Framework e AWS Prescriptive Guidance. Ponto de partida prático para times que desejam implementar ou padronizar ADRs e integrá-los a pipelines de RAG sobre documentação técnica.

---

### [LLM Powered Autonomous Agents](https://lilianweng.github.io/posts/2023-06-23-agent/)
**Fonte:** Lilian Weng / Lil'Log | **Ano:** 2023
**Contexto de aplicabilidade:** Visão panorâmica e detalhada da anatomia de agentes baseados em LLMs: planejamento (Chain of Thought, Tree of Thoughts, ReAct, Reflexion), memória (sensorial, curta duração, longa duração via vector stores) e uso de ferramentas. Essencial para times que precisam entender os fundamentos antes de escolher frameworks ou projetar sistemas agênticos para revisão de código, triagem de bugs e geração de documentação.

---

### [Agents — Chip Huyen](https://huyenchip.com/2025/01/07/agents.html)
**Fonte:** Chip Huyen / huyenchip.com | **Ano:** 2025
**Contexto de aplicabilidade:** Análise rigorosa dos componentes de um agente — ferramentas (knowledge augmentation, capability extension, write actions), planejamento e seus modos de falha. Huyen recomenda desacoplar geração de plano da execução, validar planos antes de rodá-los e rastrear métricas específicas como precisão de chamadas de ferramentas e taxa de planos válidos. Leitura estratégica para times que precisam avaliar e monitorar agentes em produção.

---

### [Effective Context Engineering for AI Agents](https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents)
**Fonte:** Anthropic Applied AI Team | **Ano:** 2025
**Contexto de aplicabilidade:** Guia técnico sobre como projetar e manter o conjunto ótimo de tokens que alimenta um agente durante a inferência — sistema de instrução, ferramentas, dados externos e histórico de mensagens. Introduz o conceito de *context rot* (degradação de acurácia à medida que o volume de tokens cresce) e recomenda técnicas como recuperação just-in-time, compaction e multi-agentes para tarefas de longa duração. Diretamente aplicável ao design de contexto compartilhado para times de engenharia.

---

### [RAG for a Codebase with 10k Repos](https://www.qodo.ai/blog/rag-for-large-scale-code-repos/)
**Fonte:** Qodo (anteriormente CodiumAI) | **Ano:** 2024
**Contexto de aplicabilidade:** Estudo de caso detalhado de RAG aplicado a codebases de escala empresarial: chunking com análise estática por linguagem, embeddings enriquecidos com descrições em linguagem natural, recuperação em dois estágios (busca vetorial + filtragem por LLM) e indexação contínua. Demonstra como superar o gap entre "como o desenvolvedor pergunta" e "o que o embedding captura" — padrão diretamente aplicável a sistemas que indexam ADRs, padrões de equipe e documentação técnica.

---

### [Context Engineering Guide — LlamaIndex](https://www.llamaindex.ai/blog/context-engineering-what-it-is-and-techniques-to-consider)
**Fonte:** LlamaIndex | **Ano:** 2025
**Contexto de aplicabilidade:** Distingue context engineering de prompt engineering e apresenta cinco técnicas concretas: seleção de knowledge base e ferramentas, compressão e ordenação de contexto, memória de longa duração (VectorMemoryBlock, FactExtractionMemoryBlock), saídas estruturadas e workflow engineering. Referência prática para times que constroem assistentes de código com consciência de codebase, cobrindo decisões arquiteturais sobre quando engajar o LLM versus lógica determinística.

---

### [ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/abs/2210.03629)
**Fonte:** Yao et al. / Princeton & Google | **Ano:** 2022
**Contexto de aplicabilidade:** Paper original que define o padrão ReAct — ciclo Thought → Action → Observation que intercala raciocínio e uso de ferramentas. Supera baselines em 34% no ALFWorld e 10% no WebShop, reduz alucinações e aumenta interpretabilidade em comparação ao Chain-of-Thought puro. Fundamental para entender o loop de raciocínio que sustenta a maioria dos agentes de engenharia modernos, incluindo agentes de revisão de código e triagem de bugs.

---

### [Agentic Engineering Patterns](https://simonw.substack.com/p/agentic-engineering-patterns)
**Fonte:** Simon Willison | **Ano:** 2026
**Contexto de aplicabilidade:** Coletânea de padrões práticos para construção de software *com* agentes de código (Claude Code, Cursor, GitHub Copilot), não apenas *para* agentes. Inclui Red/Green TDD com agentes, "First Run the Tests" como contrato de qualidade e Linear Walkthroughs para entender codebases desconhecidas. Willison define agentic engineering como a disciplina emergente de desenvolvedores que dirigem agentes que geram e executam código, com implicações diretas para governança de qualidade.

---

### [The Standard of Code Review — Google Engineering Practices](https://google.github.io/eng-practices/review/reviewer/standard.html)
**Fonte:** Google | **Ano:** Mantido ativamente
**Contexto de aplicabilidade:** Define o padrão central de revisão de código do Google: aprovar um PR quando ele melhora a saúde do código, mesmo que imperfeito, equilibrando progresso com qualidade. Fornece critérios objetivos (fatos técnicos superam preferências pessoais, style guides são autoritativos, mentoria via "Nit:") que podem ser codificados como rubrica compartilhada entre time humano e agentes de revisão de código.

---

### [Engineering Fundamentals Checklist — Microsoft CSE Playbook](https://microsoft.github.io/code-with-engineering-playbook/engineering-fundamentals-checklist/)
**Fonte:** Microsoft CSE / code-with-engineering-playbook | **Ano:** Mantido ativamente
**Contexto de aplicabilidade:** Checklist abrangente de fundamentos de engenharia cobrindo source control, testes (>90% cobertura de unidade), CI/CD, segurança, observabilidade, revisão de código (mínimo 2 revisores por política) e design reviews com alternativas documentadas. Serve como governance mínima viável que pode ser ingerida em um sistema RAG para que agentes verifiquem conformidade automaticamente em PRs.

---

### [State of Agent Engineering — LangChain Survey](https://www.langchain.com/state-of-agent-engineering)
**Fonte:** LangChain | **Ano:** 2025
**Contexto de aplicabilidade:** Survey com 1.340 respondentes sobre o estado real de agentes em produção: 57% já têm agentes rodando em produção, qualidade/acurácia é a principal barreira (32%), 94% dos times com agentes em produção implementaram observabilidade. Dados de adoção de multi-model strategies (75%+), preferência por RAG + prompt engineering sobre fine-tuning (57% não fazem fine-tuning) e padrões emergentes como MCP como protocolo universal. Essencial para calibrar expectativas e prioridades de investimento.

---

### [Context Engineering Best Practices for AI-Powered Dev Teams](https://packmind.com/context-engineering-ai-coding/context-engineering-best-practices/)
**Fonte:** Packmind | **Ano:** 2025–2026
**Contexto de aplicabilidade:** Guia operacional de context engineering para times de desenvolvimento: como estruturar arquivos de contexto hierárquicos, estabelecer governança (quem pode modificar, qual processo de revisão), tratar contexto como "código vivo" com atualizações incrementais, e criar rotinas de compartilhamento semanal de aprendizados. Times que combinaram ganhos de produtividade com revisão de IA no loop reportaram 81% de melhora em qualidade de código — mais que o dobro de times sem context engineering sistemático.

---

## Referências Complementares

### [Architecture Decision Record — Martin Fowler bliki](https://martinfowler.com/bliki/ArchitectureDecisionRecord.html)
**Fonte:** Martin Fowler | **Ano:** Atualizado continuamente
**Contexto de aplicabilidade:** Verbete de referência rápida de Martin Fowler sobre ADRs, com links para o artigo original de Nygard e recursos adicionais. Útil para onboarding de times ao conceito e para embasar a decisão de adotar ADRs como artefato de contexto compartilhado com IA.

---

### [CLAUDE.md Best Practices — Anthropic Code Docs](https://code.claude.com/docs/en/best-practices)
**Fonte:** Anthropic | **Ano:** 2025
**Contexto de aplicabilidade:** Documentação oficial sobre como estruturar o arquivo CLAUDE.md — o "contrato de comportamento" que o Claude Code lê automaticamente a cada sessão. Cobre o que incluir (stack tecnológica, padrões arquiteturais, comandos de build/test, restrições de escopo), o que evitar (regras de style que um linter faz melhor) e como manter o arquivo com menos de 300 linhas para não exaurir a atenção do modelo. Padrão aplicável a qualquer assistente de código com suporte a instruções customizadas.

---

### [AI Agent vs. Automation — AWS Executive Insights](https://aws.amazon.com/executive-insights/content/agents-vs-automation-a-strategic-guide-for-business-leaders/)
**Fonte:** AWS | **Ano:** 2024
**Contexto de aplicabilidade:** Framework estratégico para decidir entre automação tradicional e agentes de IA: automação para regras fixas, entradas estruturadas e consistência crítica; agentes para entradas não estruturadas, regras que mudam frequentemente e decisões que exigem julgamento. A combinação dos dois é o padrão recomendado — automação para o previsível, agente para onde julgamento é necessário. Referência direta para times que precisam justificar (ou refutar) a adoção de agentes em workflows de engenharia.
