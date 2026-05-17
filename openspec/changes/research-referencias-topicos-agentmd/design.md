## Context

O AGENT.md define 12 tópicos de formação para times de engenharia na era da IA. Cada tópico cobre uma área com subtópicos específicos, mas ainda sem materiais de referência mapeados. O trabalho de research precisa ser feito de forma sistemática — usando o agente RPI (Research, Plan, Implement) para buscar artigos, papers, posts canônicos, estudos de caso e boas práticas na internet para cada tópico.

O projeto já tem estrutura de `.agents/` com skills, rules e agentes configurados para suportar esse fluxo. O output de cada spec deve ser um documento estruturado com referências verificáveis e contexto de aplicabilidade para times de engenharia.

## Goals / Non-Goals

**Goals:**
- Mapear 5–10 referências de alta qualidade por tópico (artigos, posts, papers, estudos de caso)
- Priorizar fontes primárias e autores reconhecidos (Martin Fowler, ThoughtWorks, Google, Netflix, Stripe, etc.)
- Incluir contexto de como cada referência se aplica ao day-to-day de times de engenharia
- Cobrir todos os 12 tópicos do AGENT.md com profundidade proporcional à sua complexidade
- Identificar materiais em EN e/ou PT-BR quando de alta qualidade
- Estruturar o output de forma que sirva de insumo para criação de conteúdo de formação

**Non-Goals:**
- Criar o conteúdo de formação final (slides, vídeos, workshops) — esse é o próximo passo
- Implementar código ou ferramentas
- Avaliar ou recomendar ferramentas específicas de IA (Cursor, Copilot, etc.) — apenas referenciar quando relevante
- Produzir material exaustivo — curadoria com qualidade é mais importante que volume

## Decisions

**Decisão 1: Uma spec por tópico do AGENT.md**
Cada um dos 12 tópicos vira uma spec separada em `openspec/specs/<capability>/spec.md`. Isso permite trabalho paralelo, rastreabilidade por tópico e revisão independente.
*Alternativa considerada*: um único documento consolidado — rejeitado porque dificulta manutenção e paralelismo.

**Decisão 2: Estrutura padrão de referência em cada spec**
Cada referência segue o formato: título, link, autor/fonte, ano, e 2–3 linhas de contexto de aplicabilidade. Isso garante consistência e facilita a transformação em material de formação.
*Alternativa*: formato livre — rejeitado porque dificulta automação e revisão.

**Decisão 3: Uso do agente RPI para pesquisa via WebSearch**
O agente realiza buscas direcionadas por tópico, filtrando por qualidade e relevância para times de engenharia de produto. Não se limita a resultados recentes — artigos clássicos e fundacionais são prioritários quando ainda relevantes.

**Decisão 4: Prioridade de fontes**
Ordem de prioridade: (1) autores reconhecidos com track record (Martin Fowler, Kent Beck, Sam Newman, etc.), (2) empresas de referência (ThoughtWorks, Netflix, Stripe, Google, Basecamp), (3) comunidades técnicas (martinfowler.com, highscalability.com, infoq.com), (4) artigos acadêmicos quando aplicáveis. Posts de blog genéricos sem autor identificado são evitados.

## Risks / Trade-offs

- **Links podem sair do ar** → Registrar título, autor e data para permitir busca futura; priorizar fontes estáveis (livros, sites institucionais).
- **Viés de língua inglesa** → Busca ativa por material PT-BR de qualidade, mas sem comprometer a relevância — melhor uma referência em EN do que uma em PT-BR de baixa qualidade.
- **Tópicos em evolução rápida (agentes, workflows avançados)** → Marcar referências com data e sinalizar quando o campo está mudando rapidamente; priorizar princípios sobre ferramentas específicas.
- **Volume vs. qualidade** → Cap de 10 referências por tópico força curadoria real; mais referências podem ser adicionadas em iterações futuras.
- **Sobreposição entre tópicos** → Referências podem ser relevantes para múltiplos tópicos — permitido com nota de cross-reference, mas cada spec deve ter pelo menos 5 referências únicas.
