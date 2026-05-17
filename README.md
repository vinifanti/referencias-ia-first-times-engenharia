# Programa IA-First para Times de Engenharia

Repositório de pesquisa, materiais e referências para desenvolver times de engenharia que operam com mentalidade e práticas IA-first — do onboarding à arquitetura, passando por cultura, qualidade e desenvolvimento de agentes.

## Objetivo

Este repositório centraliza o trabalho de **Research, Plan e Implement (RPI)** para os 12 tópicos do programa de formação descrito em [AGENT.md](./AGENT.md). Para cada tópico, foram levantadas referências canônicas, casos reais e boas práticas de fontes reconhecidas na internet, organizadas para servir de insumo direto ao desenvolvimento de conteúdo de formação para times de engenharia.

---

## Tópicos do Programa

### Fase 1 — Fundações

| # | Tópico | Referências |
|---|---|---|
| 1 | Onboarding / Cultura IA-First | [01-cultura-e-projeto-ia-first.md](./referencias/01-cultura-e-projeto-ia-first.md) |
| 2 | Projeto IA-First: Setup e Entrega E2E com IA | [01-cultura-e-projeto-ia-first.md](./referencias/01-cultura-e-projeto-ia-first.md) |
| 3 | Product Engineer: Discovery, PRDs e Backlog | [02-product-engineer-e-sdd.md](./referencias/02-product-engineer-e-sdd.md) |
| 4 | Harness, Spec-Driven Development e Code Review com IA | [02-product-engineer-e-sdd.md](./referencias/02-product-engineer-e-sdd.md) |
| 5 | Construindo uma Empresa IA-First / Team Topologies | [03-team-topologies-e-adocao.md](./referencias/03-team-topologies-e-adocao.md) |
| 6 | Adoção de IA de Forma Segura | [03-team-topologies-e-adocao.md](./referencias/03-team-topologies-e-adocao.md) |

### Fase 2 — Arquitetura e Qualidade

| # | Tópico | Referências |
|---|---|---|
| 7 | Evolução Arquitetural: Monólito Modular e Microsserviços | [04-arquitetura-e-refatoracao.md](./referencias/04-arquitetura-e-refatoracao.md) |
| 8 | Refatoração Assistida por IA: DDD e Padrões | [04-arquitetura-e-refatoracao.md](./referencias/04-arquitetura-e-refatoracao.md) |
| 9 | Workflows Avançados com IA | [05-workflows-e-frontend.md](./referencias/05-workflows-e-frontend.md) |
| 10 | Evolução Arquitetural Frontend na Era da IA | [05-workflows-e-frontend.md](./referencias/05-workflows-e-frontend.md) |

### Fase 3 — Contexto, Governança e Agentes

| # | Tópico | Referências |
|---|---|---|
| 11 | Contexto Compartilhado, RAG, Padrões e Governança | [06-rag-e-agentes.md](./referencias/06-rag-e-agentes.md) |
| 12 | Desenvolvimento de Agentes | [06-rag-e-agentes.md](./referencias/06-rag-e-agentes.md) |

---

## Arquivos de Referência

```
referencias/
├── INDEX.md                        ← Índice completo com cross-references entre tópicos
├── 01-cultura-e-projeto-ia-first.md
├── 02-product-engineer-e-sdd.md
├── 03-team-topologies-e-adocao.md
├── 04-arquitetura-e-refatoracao.md
├── 05-workflows-e-frontend.md
├── 06-rag-e-agentes.md
└── 07-referencias-pt-br.md         ← Hipsters.tech, InfoQ Brasil, Lambda3
```

**133 referências curadas** de fontes primárias: Martin Fowler, Pragmatic Engineer, Anthropic, ThoughtWorks, Shopify Engineering, DORA, McKinsey, Team Topologies, Addy Osmani, Simon Willison, Chip Huyen, Lilian Weng e mais.

Comece pelo [INDEX.md](./referencias/INDEX.md) para ter uma visão completa com cross-references entre tópicos.

---

## Estrutura do Repositório

```
.
├── AGENT.md                        ← Definição dos 12 tópicos do programa
├── README.md                       ← Este arquivo
├── referencias/                    ← Materiais e referências por tópico
└── openspec/                       ← Histórico de planejamento e specs (OpenSpec)
    └── changes/
        └── research-referencias-topicos-agentmd/
            ├── proposal.md         ← Por que este research foi feito
            ├── design.md           ← Como foi conduzido
            ├── tasks.md            ← Todas as 46 tarefas (concluídas)
            └── specs/              ← Specs por capability
```