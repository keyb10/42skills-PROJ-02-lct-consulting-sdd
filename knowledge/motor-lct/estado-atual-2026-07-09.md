# Estado da conversa — 2026-07-09

> **Status (atualizado):** Virada de chave do Degrau 1 + Enriquecimento Estratégico da Matriz.
> **Princípios aplicados:** VII (sincronia MD↔JSON), IX (POPs nunca deletados), X (versionamento patch).
> **Snapshot anterior arquivado em:** `knowledge/motor-lct/_archive/estado-atual-2026-07-07.md` (regra IX).

---

## 1. Onde a régua está hoje

- **Matriz do Motor:** **v0.0.5** — D1 inteiro resetado (profundidade `.`), D2-D5 inalterados; **Eixo Y enriquecido** com substrato estratégico LUZ HUB (papel_no_funil, gatilho_proximo_degrau, fonte_estrategica_linha).
- **D1 sub-state:** `pops/` está vazio de propósito. Os 3 POPs do Elo 6 (vigentes até 07/jul) foram movidos para `_archive/lo6-2026-07-09/NOTA.md`.
- **Sincronia MD↔JSON:** mantida — diff entre `matriz.md` (v0.0.5) e `matriz.json` (v0.0.5) é simétrico.
- **Constituição (Regra inegociável):** ratificada em 05/jul, v1.0.0, 10 princípios — princípio X (versionamento) acionado.
- **Manifesto:** intocado.
- **Governança:** aplicada no tipo 4 (depreciação) + 1 (preencher) + 3 (adotar compêndio estratégico).

## 2. Por que essa virada

| Antes (07/jul) | Depois (09/jul) |
|---|---|
| POPs do Elo 6 prontos no vácuo — sem alinhamento com catálogo de skills | POPs vazios — aguardando curadoria skills antes de qualquer conteúdo |
| Próximo alvo: `pop-sessao-90m.md` (Elo 5) | Próximo alvo: **Sprint 1 — Curadoria de Skills** (depois Elo 5) |
| Filo D1×C1 com profundidade M e 3 POPs referenciados | Filo D1×C1 com profundidade `.`, sem POPs — aberto a reagrupar capacidades |
| SKills mapeadas em [`skills-curadoria/matriz-skills-por-degrau.md`](../../../skills-curadoria/matriz-skills-por-degrau.md) mas sem conexão com a matriz do Motor | Curadoria skills vai virar **input do Motor**, não só elenco independente |

## 3. POPs e agentes atuais

| Ativo | Status |
|---|---|
| `pops/template-raio-x.md` | ⚪️ **Arquivado** (em `_archive/lo6-2026-07-09/`) — pode ser reusado |
| `pops/pop-diagnostico-final.md` | ⚪️ **Arquivado** — pode ser reusado |
| `pops/README.md` (antigo) | ⚪️ **Arquivado** — substituído por novo índice vazio |
| `pops/README.md` (novo) | 🟢 Em vigor (vazio, aguardando Sprint 1) |
| Agentes do Motor | ⏸️ Sem agentes criados ainda nesta rodada |

## 4. Decisões consolidadas (permanecem válidas do 07/jul)

- **Nome do motor:** `motor-lct`
- **Granularidade:** matriz única primeiro; expansão por Degrau sob demanda
- **Conteúdo da matriz:** só "para cliente"
- **Rejeição de capítulos do The Revenue Codex:** caso a caso, com arbitragem de Leandro
- **Cadeia de Espetacularidade:** mantida (princípio III do motor)
- **Marketing é uso interno**
- **Compêndio (The Revenue Codex):** insumo de mercado, sem menção a autor
- **Working tree versionado, commits humanos em PT-BR**

## 5. Próxima operação (Sprint 1)

Sequência acordada: **Estudo profundo de D1×C1** (Camada 1 — Sequência Inversa) usando **3 fontes**:
1. **LUZ HUB** (`strategy/lct-transformation-90d.md`) — substrato estratégico do D1
2. **Motor LCT** (`matriz.md`/`.json`, `governance.md`) — D1×C1 conceitual
3. **The Revenue Codex** (cap. 02, 03, 04, 06, 07 — os identificados no cruzamento v1)

**Skills do catálogo aplicadas (kit completo):**
1. `search` ou `search-strategy` (KB/enterprise-search/) — define escopo do estudo
2. `digest` (KB/enterprise-search/) — lê e digere caps do The Revenue Codex
3. `knowledge-synthesis` (KB/enterprise-search/) — sintetiza entre Motor + The Revenue Codex + Estratégia
4. `write-spec` (KB/product-management/) ou `competitive-brief` — produz documento final

**Entregável da Sprint:** `knowledge/motor-lct/estudos/celula-D1-C1.md` com:
- Resumo das 3 fontes para a célula
- Encontrados (POP/entregável sugerido)
- Choques com Manifesto (Cap. 20, C2, C5, C7)
- Próxima célula-alvo (C2 ou C3 ou C4 do D1)

## 6. Ações decorrentes da virada (atualizado)

**Matriz: v0.0.6 (D1 inteiro estudado — 4/4 células)**

- 🟢 `matriz.json` → **v0.0.6** (D1 inteiro estudado: C1=M, C2=B/M, C3=B, C4=B)
- 🟢 `matriz.md` → **v0.0.6** (Eixo Y enriquecido + D1 inteiro detalhado)
- 🟢 `estudos/celula-D1-C1.md` → estudo inaugural publicado (cap. 02, 03, 04, 06, 07)
- 🟢 `estudos/celula-D1-C2.md` → estudo publicado (cap. 06, 10, 24)
- 🟢 `estudos/celula-D1-C3.md` → estudo publicado (cap. 08, 25-28)
- 🟢 `estudos/celula-D1-C4.md` → estudo publicado (cap. 11, 12-15, 18, 21 — Cap. 20 censurado)
- 🟢 `pops/_archive/lo6-2026-07-09/` (3 POPs arquivados)
- 🟢 `pops/README.md` reescrito (vazio, aguardando produção)
- 🟢 `skills-curadoria/matriz-skills-por-degrau.md` permanece como material de partida
- 🟢 `cruzamento-motor-x-codex.md` (v1, validação 5×4×Cap.)
- 🟢 `d1-por-camada.md` (planejamento macro do D1)
- 🟢 `memory.md` do PROJ-02 alinhado com a virada + D1 fechado

**Próxima fase (plano de produção por célula):**
1. Criar 4 POPs novos: pop-diagnostico-ceo-90m, pop-auditoria-maquina-cliente, pop-pulse-clientes-atuais, pop-5-angulos-posicionamento-cliente
2. Reativar 2 POPs do archive: template-raio-x, pop-diagnostico-final
3. Construir skill  (gap do PROJ-03) — protocolo das 5 perguntas-chave do Cap. 07
4. Construir skill  (gap do PROJ-03) — coerência de voz nas peças D1×C4
5. Aplicar marcadores  /  no The Revenue Codex original (Regra III da governance)
6. (futuro) Estudos de D2-D5 seguindo o mesmo kit completo

## 6. Ações decorrentes da virada (BUMP 09/jul)

- 🟢 `matriz.json` → v0.0.5 (D1 todo `.`, Eixo Y enriquecido)
- 🟢 `matriz.md` → v0.0.5 (Eixo Y enriquecido com tabela de Estratégia LUZ HUB)
- 🟢 `pops/_archive/lo6-2026-07-09/` criado
- 🟢 `pops/README.md` reescrito (vazio, aguardando Sprint 1)
- 🟢 `skills-curadoria/matriz-skills-por-degrau.md` permanece como material de partida da Sprint 1
- 🟢 `knowledge/motor-lct/cruzamento-motor-x-codex.md` criado (v1, validação de 5×4×Cap. Codexo)
- 🟢 `knowledge/motor-lct/d1-por-camada.md` criado (planejamento macro do D1)
- 🟢 `memory.md`, `plan.md`, `tasks.md` do PROJ-02 alinhados com a virada

## 7. Convenções ativas

- MD↔JSON sincronizados — diff antes de commitar
- POPs arquivados (Regra IX) — recuperáveis mas não operacionais
- Cada sprint começa com curadoria — não com produção
- C1 do D1 tem prioridade — Sequência Inversa do método

## 7. Skill brand-lct instalada (2026-07-09, Sprint 1 do PROJ-03 fechada)

- ✅ Skill **brand-lct v0.1.0** instalada em 
- 218 linhas, 11.9KB, 10 regras + cross-ref com skills do catálogo + decision tree
- TDD fechado: RED (1 baseline) + GREEN (3 cenários) + REFACTOR

**Revisão retroativa sob a skill (todos os artefatos do PROJ-02):**
- 4 estudos (celula-D1-C1.md, C2.md, C3.md, C4.md) → ✅ passam
- cruzamento-motor-x-codex.md → ✅ passa
- d1-por-camada.md → ✅ passa
- estado-atual-2026-07-09.md → ✅ passa

**Próxima sprint (PROJ-03 Sprint 2):** construir **ceo-interview** — protocolo 5 perguntas-chave do Cap. 07 (Re-check PMF). Bloqueio de D1×C1 entrar em produção.

---

**Atualização 2026-07-10 (v0.0.8):** D1 PRODUZIDO. 6 POPs prontos em pops/. Marcadores [adotado:] / [rejeitado:] aplicados no The Revenue Codex original (20 caps). Commit + push no GitHub finalizados.

**Próximo:** D2 produção (10 POPs).

**Snapshot anterior arquivado em:** knowledge/motor-lct/_archive/estado-atual-2026-07-07.md
