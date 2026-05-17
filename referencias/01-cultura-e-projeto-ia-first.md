# Referências: Cultura IA-First

## Referências Principais

### [From Memo to Movement: Shopify's Cultural Adoption of AI](https://www.firstround.com/ai/shopify)
**Fonte:** First Round Capital (entrevista com Farhan Thawar, VP & Head of Engineering) | **Ano:** 2025
**Contexto de aplicabilidade:** Documenta como a Shopify transformou a adoção de IA em movimento cultural genuíno — dando acesso a todos, exibindo o raciocínio da IA em vez de escondê-lo, e escalando o programa de estágios de 100 para mais de 1.000. Equipes podem extrair princípios concretos: democratização de acesso, liderança pelo exemplo e ênfase na prototipagem intensa. É um caso de referência para times que querem ir além de licenciar ferramentas e construir uma identidade coletiva em torno da IA.

---

### [Inside Shopify's AI-First Engineering Playbook](https://www.bvp.com/atlas/inside-shopifys-ai-first-engineering-playbook)
**Fonte:** Bessemer Venture Partners | **Ano:** 2026
**Contexto de aplicabilidade:** Detalha o manual operacional da Shopify: proxy de LLM centralizado para controle de custo, ganhos de 20% de produtividade medidos por demos semanais (não por linhas de código), e o conceito de "comprehension debt" — engenheiros precisam manter entendimento dois ou três níveis abaixo do código que geram com IA. Útil para times que estão estruturando governança, métricas e salvaguardas de qualidade em um ambiente IA-first.

---

### [How AI is Changing Software Engineering at Shopify – The Pragmatic Engineer](https://newsletter.pragmaticengineer.com/p/how-ai-is-changing-software-engineering)
**Fonte:** Gergely Orosz, The Pragmatic Engineer | **Ano:** 2025
**Contexto de aplicabilidade:** Gergely Orosz entrevista Farhan Thawar e revela como a Shopify espera que engenheiros usem IA de forma reflexiva, com budget ilimitado de tokens, entrevistas técnicas para diretores e o princípio de que candidatos sem IA em entrevistas tendem a ter pior desempenho. Mostra como uma cultura IA-first se manifesta em processos de contratação, onboarding e expectativas diárias de trabalho.

---

### [AI-First Software Engineering – ThoughtWorks Perspectives](https://www.thoughtworks.com/perspectives/edition36-ai-first-software-engineering/article)
**Fonte:** Birgitta Boeckeler, Alessio Ferri, Martin Fowler — ThoughtWorks | **Ano:** 2025
**Contexto de aplicabilidade:** Artigo de referência da ThoughtWorks que posiciona a entrega de software assistida por IA (AIFSD) como uma mudança que atravessa todo o ciclo de desenvolvimento — da definição de produto à manutenção. Reforça que boas práticas de engenharia (TDD, arquitetura modular, agile) se tornam ainda mais essenciais no contexto IA-first, não menos. Essencial para equipes que precisam alinhar liderança técnica e de produto sobre o que muda e o que permanece.

---

### [Coding Assistants Do Not Replace Pair Programming](https://martinfowler.com/articles/exploring-gen-ai/05-not-your-pair-programmer.html)
**Fonte:** Birgitta Böckeler — martinfowler.com | **Ano:** 2023
**Contexto de aplicabilidade:** Böckeler argumenta com clareza que assistentes de IA e pair programming atendem propósitos fundamentalmente distintos: a IA acelera tarefas táticas, enquanto o pair programming constrói propriedade coletiva do código, conhecimento histórico e habilidades de colaboração que a IA não consegue replicar. Para times adotando IA, o artigo orienta a não sacrificar rituais de programação em par em nome da velocidade — e sim combiná-los.

---

### [Patterns for Reducing Friction in AI-Assisted Development](https://martinfowler.com/articles/reduce-friction-ai/)
**Fonte:** Rahul Garg (Principal Engineer) — martinfowler.com / ThoughtWorks | **Ano:** 2026
**Contexto de aplicabilidade:** Apresenta cinco padrões colaborativos para eliminar o ciclo frustrante de "gerar → revisar → corrigir → regenerar": Knowledge Priming, Design-First Collaboration, Encoding Team Standards, Context Anchoring e Feedback Flywheel. Cada padrão trata a IA como um colaborador que precisa de onboarding — exatamente como um desenvolvedor humano. Altamente aplicável para rituais de times que querem sistematizar o aprendizado coletivo com IA.

---

### [Building an Elite AI Engineering Culture in 2026](https://cjroth.com/blog/2026-02-18-building-an-elite-engineering-culture)
**Fonte:** Chris Roth | **Ano:** 2026
**Contexto de aplicabilidade:** Analisa o DNA de times de alta performance (Linear, Cursor, Vercel, Stripe) no contexto IA-first: equipes pequenas e seniores, cultura de escrita, zero tolerância a dívida de qualidade e dissolução da fronteira design-engenharia. O artigo traz o dado de que engenheiros seniores obtêm ganhos de produtividade quase 5x maiores que juniores com IA — reforçando que cultura e senioridade técnica são alavancas decisivas, não apenas a ferramenta.

---

### [How AI is Transforming Work at Anthropic](https://www.anthropic.com/research/how-ai-is-transforming-work-at-anthropic)
**Fonte:** Saffron Huang et al. — Anthropic | **Ano:** 2025
**Contexto de aplicabilidade:** Estudo baseado em 132 engenheiros, 53 entrevistas e 200.000 transcrições do Claude Code. Revela que colaboradores reportam 50% de aumento de produtividade, estão se tornando mais "full-stack" e usando IA como primeiro ponto de contato para dúvidas antes direcionadas a colegas. Também documenta preocupações legítimas — atrofia de habilidades e redução de mentoria — que times IA-first precisam endereçar ativamente em sua cultura.

---

# Referências: Projeto IA-First E2E

## Referências Principais

### [Best Practices for Claude Code](https://code.claude.com/docs/en/best-practices)
**Fonte:** Anthropic — Claude Code Docs | **Ano:** 2025
**Contexto de aplicabilidade:** Documentação oficial e altamente detalhada que cobre o fluxo E2E de trabalho com um agente de código autônomo: explorar → planejar → implementar → commitar. Inclui diretrizes para escrever CLAUDE.md eficaz, gerenciar janela de contexto, usar subagentes para investigação paralela, e configurar permissões e hooks. Referência primária obrigatória para qualquer time estruturando um projeto IA-first com Claude Code.

---

### [CLAUDE.md: Best Practices Learned from Optimizing Claude Code with Prompt Learning](https://www.humanlayer.dev/blog/writing-a-good-claude-md)
**Fonte:** HumanLayer Blog | **Ano:** 2025
**Contexto de aplicabilidade:** Guia prático focado em como escrever um CLAUDE.md eficaz: incluir apenas instruções universalmente aplicáveis, manter o arquivo curto e testável, tratar cada linha como código (remover o que Claude já faz corretamente). Complementa a documentação oficial com perspectiva de time que otimizou Claude Code em projetos reais. Diretamente aplicável ao setup inicial de qualquer projeto IA-first.

---

### [My LLM Coding Workflow Going Into 2026](https://addyosmani.com/blog/ai-coding-workflow/)
**Fonte:** Addy Osmani (Engineering Manager, Google Chrome) | **Ano:** 2026
**Contexto de aplicabilidade:** Addy Osmani, engenheiro de referência do Google, descreve seu fluxo pessoal com LLMs: planejar antes de codificar, quebrar tarefas em partes pequenas, usar múltiplos modelos em paralelo para cross-checking, revisar todo código gerado como se fosse de um desenvolvedor júnior, e commitar frequentemente como checkpoints seguros. Altamente credível por vir de um praticante experiente com visibilidade da indústria.

---

### [The Prompt Engineering Playbook for Programmers](https://addyo.substack.com/p/the-prompt-engineering-playbook-for)
**Fonte:** Addy Osmani — Substack | **Ano:** 2025
**Contexto de aplicabilidade:** Playbook direto e aplicável sobre como escrever prompts eficazes para código: contexto explícito (frameworks, versões, constraints), especificidade na definição de "done", quebra de tarefas complexas em passos iterativos, e como conduzir um diálogo iterativo em vez de esperar respostas perfeitas na primeira tentativa. Ideal para onboarding de novos membros do time no uso produtivo de assistentes de IA.

---

### [A Field Guide to AI-First Development](https://www.makingdatamistakes.com/ai-first-development/)
**Fonte:** Greg Detre — Making Data Mistakes | **Ano:** 2025
**Contexto de aplicabilidade:** Guia de campo prático que cobre mudança de mentalidade ("você não está mais aqui para escrever código"), estrutura de documentação como infraestrutura (CLAUDE.md, docs evergreen, research docs), escolha de stack simples e bem documentada, e uso de modelos diferentes para tarefas diferentes (Claude para conversação, o3 para debugging e crítica). Especialmente útil para arquitetos e tech leads estruturando o ambiente de um projeto IA-first do zero.

---

### [State of AI-Assisted Software Development 2025 – DORA Report](https://dora.dev/dora-report-2025/)
**Fonte:** Google Cloud / DORA (com GitHub, GitLab, IT Revolution) | **Ano:** 2025
**Contexto de aplicabilidade:** Pesquisa com quase 5.000 profissionais de tecnologia que estabelece que IA é um amplificador — times fortes ficam ainda melhores, times com problemas têm os problemas amplificados. O relatório identifica sete capacidades organizacionais que maximizam o retorno da IA, com ênfase em plataformas internas de qualidade, clareza de workflows e alinhamento de times. Fornece base empírica sólida para decisões de investimento e priorização em projetos IA-first.

---

### [Exploring Generative AI – Martin Fowler (tag collection)](https://martinfowler.com/tags/generative%20AI.html)
**Fonte:** Martin Fowler — martinfowler.com | **Ano:** 2023–2026
**Contexto de aplicabilidade:** Coleção de artigos de Martin Fowler e colaboradores da ThoughtWorks explorando IA generativa na engenharia de software: desde fundamentos de pair programming com IA até nondeterminismo, revisão de código e padrões de entrega. Serve como base de leitura progressiva para equipes que querem construir um vocabulário técnico compartilhado sobre IA no desenvolvimento de software, com a autoridade e rigor metodológico característicos de Fowler.

---

### [How Engineering Teams Can Thrive in 2025 – Stack Overflow Blog](https://stackoverflow.blog/2025/01/28/how-engineering-teams-can-thrive-in-2025/)
**Fonte:** Stack Overflow Blog | **Ano:** 2025
**Contexto de aplicabilidade:** Artigo baseado em dados da comunidade Stack Overflow que mapeia as principais transformações para times de engenharia: adoção de agentes autônomos além de assistentes, dissolução de silos em equipes full-stack, e necessidade de aprendizado contínuo embutido nas operações diárias. Útil como panorama do mercado para apresentações de alinhamento com stakeholders e definição de roadmap de adoção de IA no time.

---

### [Driving GitHub Copilot Adoption in Your Company](https://docs.github.com/en/copilot/tutorials/rolling-out-github-copilot-at-scale/enabling-developers/driving-copilot-adoption-in-your-company)
**Fonte:** GitHub — Documentação Oficial | **Ano:** 2024–2025
**Contexto de aplicabilidade:** Guia oficial do GitHub para rollout de Copilot em escala: cronograma de 45 dias com champions internos, modelo self-service para reduzir atrito de adoção, metas de engenharia claras antes do lançamento, e revisão contínua de métricas de uso. Diretamente aplicável como checklist para times conduzindo onboarding de ferramentas IA — os princípios se generalizam além do Copilot para qualquer assistente de código.
