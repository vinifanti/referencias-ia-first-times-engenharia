## ADDED Requirements

### Requirement: Referências sobre RAG aplicado a codebases e documentação técnica
O research SHALL produzir referências que cubram como aplicar RAG (Retrieval-Augmented Generation) a codebases — indexando documentação, ADRs e padrões para que a IA use automaticamente como contexto de domínio.

#### Scenario: Referências sobre RAG aplicado a codebases
- **WHEN** o agente pesquisa RAG para desenvolvimento de software
- **THEN** o output MUST incluir pelo menos 3 referências sobre como implementar e usar RAG em contextos de engenharia de software — indexação de código, docs e ADRs

#### Scenario: Referências sobre ADRs: escrita, manutenção e uso com IA
- **WHEN** o agente busca por Architecture Decision Records
- **THEN** o output MUST incluir pelo menos 2 referências sobre como escrever ADRs eficazes e como a IA pode ajudar a manter e consultar ADRs como memória organizacional

### Requirement: Referências sobre governança mínima e padrões compartilhados ensináveis
O research SHALL identificar materiais sobre como criar padrões técnicos que tanto o time quanto a IA sigam — incluindo exemplos, rubricas, checklists e playbooks de qualidade — com governança leve para evoluí-los sem burocracia.

#### Scenario: Referências sobre padrões compartilhados que a IA pode seguir
- **WHEN** o agente pesquisa padrões de código e IA
- **THEN** o output MUST incluir pelo menos 2 referências sobre como criar padrões, exemplos e checklists que a IA possa usar como referência para gerar código consistente com o estilo do time

#### Scenario: Referências sobre playbooks de qualidade e code review guidelines
- **WHEN** o agente busca por playbooks de engenharia
- **THEN** o output MUST incluir pelo menos 2 referências com exemplos de playbooks de qualidade, guidelines de code review e critérios de merge usados por times de engenharia de referência
