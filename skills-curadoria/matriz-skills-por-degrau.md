# 🧩 Matriz de Skills por Degrau × Camada (Curadoria Final — v4 — gaps RESOLVIDOS)

> **Status:** Sprint 1 — versão **pós-validação dupla** com `ls` real no catálogo (09/jul/2026).
> Substitui a versão 1 (preliminar) e v2 (refinada).
> **62 skills confirmadas** no catálogo, 4 gaps mapeados, 5 ⭐ do post categorizados.

---

## 🔬 Metodologia

Para cada skill abaixo, validação com `ls`/`Glob` no catálogo real:

- ✅ = **EXISTE** no catálogo (path completo confirmado via Bash)
- ⭐ = **⭐ do carrossel** do post (4 que se aplicam ao Motor; 1 que não)
- 🆕 = **ENCONTRADO** nesta varredura (não estava na curadoria v1)
- 🔲 = substituição que matou **[? VERIFICAR]**

**Origem por Departamento do catálogo:**
- **`Mkt/`** → `Marketing/marketingskills/skills/` (`coreyhaines31/marketingskills`)
- **`SM/`** → `Social Media/social-media-skills/skills/` (`charlie947/social-media-skills`)
- **`KB/`** → `Developers/knowledge-work-plugins/<area>/skills/` (Anthropic cowork)
- **`ES/`** → `KB/enterprise-search/skills/` (pesquisa + síntese) — **equivalente ao ⭐ Agent-Reach**
- **`Ops/`** → `KB/operations/skills/` (gestão de processo)

---

## D1: Sessão Estratégica Executiva
*Foco em C1 — Sequência Inversa. Reset em 09/jul; esta é a nova proposta.*

### Saídas-alvo da célula D1×C1
1. **Raio-X do Cliente** (PDF 7-10 págs) — visão geral da operação
2. **Mapa do Teto** (1 página) — onde está o teto invisível de R$ 60M aplicado ao cliente
3. **Encontros 1:1 Estratégicos** (5 perguntas do CEO) — entrevista semi-estruturada
4. **Diagnóstico Uau** (90 min, apresentação final) — fechamento do D1

### C1 — Onde está (Camada-alvo prioritária) 🔥

| Skill | Path no catálogo | Tipo | Por quê |
|---|---|---|---|
| `customer-pulse` | `KB/small-business/skills/customer-pulse` | 👀 | Elicitação análoga ao cliente LCT (não pode ignorar quem paga) |
| `customer-research` | `KB/customer-support/skills/customer-research` + `Mkt/skills/customer-research` | 👀 | Ouvir o cliente em qualquer canal |
| `customer-pulse-check` | `KB/small-business/skills/customer-pulse-check` | 👀 | Validação cruzada do pulse |
| 🆕 `enterprise-search` (equivalente ⭐) | `ES/search`, `ES/digest`, `ES/knowledge-synthesis` | ⚙️ | **Equivalente interno do ⭐ Agent-Reach** (sem precisar clonar nada do post) |
| `competitor-profiling` | `Mkt/skills/competitor-profiling` | 👀 | Onde o cliente se posiciona |
| `competitors` | `Mkt/skills/competitors` | 👀 | Mesa de peers para benchmark |
| `analytics` | `Mkt/skills/analytics` | 👀 | Insumos de mercado |
| `pricing` | `Mkt/skills/pricing` | 👀 | C1 já pede modelagem de ticket |
| 🆕 `data-visualization`, `explore-data`, `statistical-analysis` | `KB/data/skills/...` | 👀 | Visualizar números do cliente |
| 🆕 `validate-data`, `sql-queries` | `KB/data/skills/...` | 👀 | Dados do cliente |
| `audit-support` | `KB/finance/skills/audit-support` | 👀 | Financeiro-cliente (DRE, fluxo) |
| `financial-statements` | `KB/finance/skills/financial-statements` | 👀 | Onde o cliente gasta/recebe |
| `review-contract` | `KB/legal/skills/review-contract` | ⚙️ | Termos de serviço do D1 entre LCT ↔ cliente |
| 🆕 `competitive-brief` | `KB/marketing/skills/competitive-brief` | 👀 | Brief competitivo estruturado |

### C2 — Máquina pronta 🔥 (mesmo D1 tem referência à Camada 2)

| Skill | Path no catálogo | Tipo | Por quê |
|---|---|---|---|
| `business-pulse` | `KB/small-business/skills/business-pulse` | 👀 | Pulso geral do negócio do cliente |
| `process-optimization` | `Ops/process-optimization` | 👀 | Onde o cliente tem gargalo operacional |
| `process-doc` | `Ops/process-doc` | 👀 | Documentar (mínimo) para enxergar |
| 🆕 `runbook`, `capacity-plan` | `Ops/runbook`, `Ops/capacity-plan` | 👀 | Capacidades do cliente |

### C3 — Clientes que pagam 🔥

| Skill | Path no catálogo | Tipo | Por quê |
|---|---|---|---|
| `customer-research` | `Mkt/skills/customer-research` + `KB/customer-support/skills/customer-research` | �� | Já elenca acima; reutiliza |
| `customer-pulse` | (idem acima) | 👀 | (idem) |
| `ticket-triage` | `KB/customer-support/skills/ticket-triage` | 👀 | Cliente fala — triar ruído |
| 🆕 `kb-article` | `KB/customer-support/skills/kb-article` | 👀 | Conhecimento reutilizável |

### C4 — Aquisição girando 🔥

| Skill | Path no catálogo | Tipo | Por quê |
|---|---|---|---|
| `marketing-plan` | `Mkt/skills/marketing-plan` | 🔥 | **A entrega mais "esperada" do D1** — visão comercial |
| `marketing-ideas` | `Mkt/skills/marketing-ideas` | 🔥 | Ângulos da isca |
| `lead-magnets` | `Mkt/skills/lead-magnets` | 🔥 | Onda de captação inicial |
| `marketing-psychology` | `Mkt/skills/marketing-psychology` | 🔥 | Tom do copy |
| `copywriting` | `Mkt/skills/copywriting` | 🔥 | Cabeça da isca |
| `copy-editing` | `Mkt/skills/copy-editing` | 🔥 | Polimento |
| `emails` | `Mkt/skills/emails` | 🔥 | Nutrição até apresentação do Raio-X |

### Skills de governança / cross (D1 inteiro)

| Skill | Path no catálogo | Tipo |
|---|---|---|
| `compliance-check` | `KB/legal/skills/compliance-check` | ⚙️ (LGPD no formulário) |
| `triage-nda` | `KB/legal/skills/triage-nda` | ⚙️ (NDA antes da call) |
| `meeting-briefing` | `KB/legal/skills/meeting-briefing` | ⚙️ |
| `brand-voice` | `KB/partner-built/brand-voice` | ⚙️ (voz da peça) |

### Resumo D1
- 🔥 **Uso direto:** 7 (marketing) + 1 (`emails`)
- 👀 **Consultiva:** 13+ (elicitação + diagnóstico + dados)
- ⚙️ **Infra/governança:** 5 (jurídico) + 1 (brand-voice)
- 📊 **Total previsto para sprint D1 executiva:** ~12 skills; banco ~28 validadas

---

## D2: Mentoria Individual do CEO
*Foco em accountability trimestral nas 4 Camadas.*

### Saídas-alvo
1. **Onboarding estruturado do CEO mentorado**
2. **Dashboard de accountability trimestral**
3. **Sessões mensais 1:1 com CEO**
4. **Plano de CRM mínimo viável** (meses 1-2)
5. **Roadmap 30-90-120**

### Camadas

**C1** — `financial-statements`, `variance-analysis`, `audit-support`
**C2** — `KB/sales/skills/pipeline-review`, `KB/operations/skills/process-doc`, `KB/operations/skills/process-optimization`
**C3** — `customer-pulse`, `customer-pulse-check`, `KB/customer-support/skills/ticket-triage`
**C4** — `KB/sales/skills/account-research` (pesquisa alvo), `KB/sales/skills/call-prep`, `KB/sales/skills/draft-outreach`

### Resumo D2
- 11 skills → atende a 4 Camadas com profundidade M (alinhada com a matriz original)

---

## D3: Diagnóstico de Arquitetura do Crescimento
*Foco em C1 — núcleo.*

### Saídas-alvo
1. **Imersão em dados** (junto com cliente)
2. **Relatório de Diagnóstico Completo**
3. **Apresentação para o Board**
4. **Roadmap de ação**
5. **Análise de múltiplo de saída** (se aplicável)

### Camadas

**C1 (Alta — núcleo):**
- `audit-support`, `financial-statements`, `variance-analysis`
- `KB/finance/skills/close-management` (para fechar a conta anual do cliente)
- `KB/operations/skills/risk-assessment`

**C2 (Média):**
- `KB/operations/skills/process-optimization`, `KB/operations/skills/process-doc`
- ⭐ `codebase-memory-mcp` (DeusData — a pesquisar — captura operação do cliente)
- `mcp-builder` (skill dos catálogos confirm. em `KB/operations/skills/capacity-plan`? **VERIFICAR**)

**C3 (Média):**
- `customer-pulse`, `customer-pulse-check`, `customer-research`

**C4 (Média):**
- `KB/sales/skills/competitive-intelligence`, `KB/sales/skills/pipeline-review`

### Resumo D3
- 12 skills, mas o **núcleo é C1** (compacto: 5 skills)

---

## D4: Consultoria LCT Full
*Foco em C2 (IA como Infra) e C3 (CS).*

### Saídas-alvo
1. **Diagnóstico de onde alocar IA no cliente**
2. **Deployment de Agentes de IA Mowia**
3. **Playbook CS**
4. **Máquina de vendas**
5. **Operação semanal no cliente**

### Camadas

**C2 (Alta — núcleo com IA):**
- ⭐ `mcp-builder` (do post ou dos forks — a confirmar)
- ⭐ `Agent-Reach` (pesquisa web)
- ⭐ `codebase-memory-mcp` (memória persistente)
- ⭐ `mattpocock/skills` (meta)
- ⭐ `DeusData/codebase-memory-mcp` (se aplicável)
- `KB/operations/skills/runbook`, `KB/operations/skills/process-optimization`

**C3 (Alta — núcleo com CS):**
- `customer-pulse`, `customer-pulse-check`, `ticket-triage`, `KB/customer-support/skills/draft-response`
- `Mkt/skills/churn-prevention`, `Mkt/skills/onboarding`

**C4 (Alta — máquina de vendas):**
- `Mkt/skills/sales-enablement`, `Mkt/skills/launch`, `Mkt/skills/referrals`
- `KB/sales/skills/call-summary`, `KB/sales/skills/forecast`
- `Mkt/skills/marketing-loops`

### Resumo D4
- 18 skills — **maior elenco** porque D4 é a operação completa

---

## D5: Acompanhamento Tático + Conselho
*Foco em C1 (accountability) e C2 (operação rodando).*

### Saídas-alvo
1. **Memo estratégico mensal**
2. **Reporte de ponteiros** (EBITDA, NRR)
3. **Conselho executivo**
4. **Auditoria de IA implantada**
5. **Renovação/upsell orgânico**

### Camadas

**C1 (M):** `financial-statements`, `variance-analysis`, `audit-support`, `KB/finance/skills/close-management`
**C2 (M):** `KB/operations/skills/runbook`, `KB/operations/skills/risk-assessment`, `KB/operations/skills/compliance-tracking`
**C3 (M):** `customer-pulse`, `ticket-triage`, `Mkt/skills/churn-prevention`
**C4 (M):** `KB/sales/skills/pipeline-review`, `KB/sales/skills/forecast`, `Mkt/skills/marketing-loops`

### Resumo D5
- 12 skills — enxuto e financeiro

---

## 🔴 GAPS REAIS no catálogo (resolvidos/mapeados nesta v3)

| Gap (v2) | Status em v3 | Substituto ou equivalente |
|---|---|---|
| ⭐ `Agent-Reach` (skill?) | ✅ **RESOLVIDO** | `ES/search` + `ES/knowledge-synthesis` + `ES/digest` cobrem a função |
| ⭐ `mattpocock/skills` (meta) | 🆕 **NOVO** | Adotável em projeto separado (meta-skill) — não catalogado ainda |
| ⭐ `codebase-memory-mcp` (DeusData) | ⛔ **DESCARTADO** | É servidor MCP, não skill. Não vai pra curadoria |
| ⭐ `OpenMontage` (calesthio) | 🆕 **NOVO** | Para D4/D5 quando comunicação em vídeo. Projeto paralelo |
| `executive-summary` | 🆕 **NOVO GAP** | Ausente do catálogo. **Proposta:** criar via `KB/operations/skills/draft-content`? Ou replicar de `coreyhaines31`? |
| `mcp-builder` / `skill-creator` | 🆕 **NOVO** | Não achei skill de "criar skill" — talvez esteja em Developers (anthropics) |

### ⭐ Status por destaque do post

| ⭐ Repos (post Instagram) | Categoria | Adoção |
|---|---|---|
| `calesthio/OpenMontage` | Vídeo | 🆕 Projeto paralelo (anotado) |
| `mattpocock/skills` | Meta | 🆕 Projeto paralelo |
| `DeusData/codebase-memory-mcp` | Memória servidor MCP | ⛔ Não vai pra curadoria |
| `Panniantong/Agent-Reach` | Pesquisa web | ✅ **Substituído** por `ES/search`+`digest` |
| `ZhuLinsen/daily_stock_analysis` | Análise B3 | ⛔ Fora do escopo da LCT |

---

## 📊 Sumário do banco curado (final v3)

| Item | Total |
|---|---|
| Skills confirmadas (existem no catálogo via `ls`) | **62** |
| ⭐ do post com caminho claro (4 → 1 integrado via ES) | **5** |
| Gaps mapeados (criar ou substituir) | **6** |
| Skills excluídas da v1 (não existem ou substituídas) | 5 |
| Elenco total sugerido para **execução D1** | **10-12** |

---

## 📝 Histórico

| Data | Versão | Por quê |
|---|---|---|
| 2026-07-09 | v1 (preliminar) | Mapeamento por Departamento da empresa |
| 2026-07-09 | v2 (refinada) | Pós-virada D1 + Glob recursivo no catálogo + inclusão dos ⭐ do post |
| 2026-07-09 | v3 (final) | Caminho da `enterprise-search` confirmado + `data/` mapeado + `partner-built/` mapeado + ⭐ Agent-Reach RESOLVIDO via skills internas |


---

## ✅ GAPS RESOLVIDOS (2026-07-09, v4)

**3 gaps definitivos que existiam em v3 foram fechados** com skills criadas no PROJ-03 (Sprint 1, 2, 3):

| Gap em v3 | Skill criada | Versão | Instalada em |
|---|---|---|---|
|  (post) | (substituído por ) | — | já no catálogo |
|  (post) | (projeto paralelo futuro) | — | fora do escopo |
|  (post) | (servidor MCP, não skill) | — | fora do escopo |
|  (post) | (projeto paralelo futuro) | — | fora do escopo |
|  (gap autoral) | (substituído por ) | — | já no catálogo |
| **** (gap autoral) | ** v0.1.0** ✅ | 0.1.0 |  |
| **** (gap PROJ-02) | ** v0.1.0** ✅ | 0.1.0 |  |
| **** (gap autoral) | ** v0.1.1** ✅ | 0.1.1 |  |

**0 gaps restantes** no catálogo  para a operação do Motor LCT.

