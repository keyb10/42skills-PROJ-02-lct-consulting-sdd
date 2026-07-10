# 🪜 D1 × 4 Camadas — Plano integrado (macro)

> **Documento vivo de planejamento do D1.** Carrega o cruzamento do Degrau 1 com cada uma das 4 Camadas do Método LCT (Sequência Inversa: C1 → C4).
>
> **Como ler:** para cada Camada, listo **saída da camada** (o que sai de lá), **skills envolvidas** (referência ao catálogo), **operação** (o que se faz), **POP a criar** (ou reativar do archive), **profundidade** (B/M/A).
>
> **Origem dos ativos:** a matriz do Motor (`knowledge/motor-lct/matriz.md/.json`) tinha D1 resetado em 09/jul. Este documento **re-constrói** as 4 células usando a curadoria v3 (`skills-curadoria/matriz-skills-por-degrau.md`).

---

## 🎯 Visão do D1 inteiro (macro)

**D1: Sessão Estratégica Executiva** — 90 min + relatório executivo de 7-10 págs.
**Ticket de referência:** R$ 2.500 (pagamento único).
**Promessa para o cliente:** *"Mostrar onde está o seu teto invisível e por que a causa quase nunca é vendas."*

Fluxo geral do D1 (Sequência Inversa):

```
[Pré-D1: atratividade → isca → venda] (não faz parte do D1 entregue)
                              ↓
[D1 — Entrega]
   C1: Onde está o cliente → diagnóstico real (Raio-X)
   C2: Como está a máquina → o que pode ser substituído por IA
   C3: O que ele tira dos clientes que já pagam → retenção invisível
   C4: O que está girando (ou não) na aquisição → máquina de vendas
                              ↓
[Apresentação 90 min (elo final do D1)] → Upsell D2/D3
```

---

## 📋 C1 — Onde você está (Camada diagnóstico) — profundidade **M**

### Saída tangível
- **Raio-X do Cliente** (PDF, 7-10 págs) com análise do estado real do negócio do cliente
- Apresentado na **Sessão 90 min** (entrega final)

### Operação
1. **Elo 1: Formulário 1 (pré-captação)** — perguntas iniciais para entender o que o cliente traz antes da call
2. **Elo 2: Call de Qualificação (30 min)** — leitura da isca + verificações iniciais
3. **Elo 3: Coleta Profunda (pós-venda)** — dados financeiros, operacionais, comerciais via formulário 2
4. **Elo 4: Sessão Estratégica (90 min, gravada/transcrita)** — perguntas-chave ao CEO (com a skill `ceo-interview`)
5. **Elo 5: Apresentação Final do Raio-X (90 min)** — entrega com template `template-raio-x.md` (arquivado, reativável)

### Skills envolvidas
**Curadas pelo catálogo (todas confirmadas):**
- `customer-pulse` (`KB/small-business/skills/customer-pulse`)
- `customer-research` (`Mkt/skills/customer-research` + `KB/customer-support/skills/customer-research`)
- `data-visualization`, `explore-data`, `validate-data`, `sql-queries` (`KB/data/skills/...`)
- `audit-support`, `financial-statements` (`KB/finance/skills/...`)
- `variance-analysis` (`KB/finance/skills/variance-analysis`)
- `competitors`, `competitor-profiling` (`Mkt/skills/...`)
- `ES/search`, `ES/knowledge-synthesis`, `ES/digest` (`KB/enterprise-search/skills/...`)

**Gap a ser criado pelo PROJ-03:** `ceo-interview` — protocolo de entrevista profunda com CEO.

### POPs a criar (ou reativar)
- **A criar:** `pop-diagnostico-ceo-90m.md` — roteiro da sessão estratégica (ex-`pop-sessao-90m`, agora formalizado)
- **A reativar do archive** (`knowledge/motor-lct/pops/_archive/lo6-2026-07-09/`):
  - `template-raio-x.md` — template do relatório de 7-10 págs
  - `pop-diagnostico-final.md` — POP da apresentação final 90 min

### Critério de qualidade "Uau"
- Cliente sai do D1 dizendo: "olha, pela primeira vez alguém me mostrou com dados onde eu estou e onde eu poderia estar."
- Raio-X é reverenciado por clientes como "material que eu uso na cabeça toda semana".

### Profundidade real
**M** (análise média, discussões guiadas) — porque D1 só dá a foto. A reestruturação fica em D3.

### Sequência inversa → **começar por aqui**

---

## 📋 C2 — Máquina pronta (operacional) — profundidade **B/M**

### Saída tangível
- **Mapa de ineficiência** na operação atual do cliente (1 página visual)
- Componentes substituíveis por IA sinalizados

### Operação
1. **Diagnóstico rápido de operações** — 1 seção do Raio-X inteiro (não é POP próprio)
2. **Identificação de gargalos** — onde o cliente perde tempo/talentos
3. **Sinalização de camadas substituíveis por IA** — onde entrar com `mcp-builder` em D4 (sem instalar nada agora)

### Skills envolvidas
**Curadas:**
- `business-pulse` (`KB/small-business/skills/business-pulse`)
- `process-doc`, `process-optimization`, `runbook`, `capacity-plan` (`KB/operations/skills/...`)
- `KB/engineering/skills/system-design` (para arquitetura do cliente)
- `Mkt/skills/product-marketing` (se produto/serviço do cliente estiver incoerente)

**Gap do PROJ-03:** nenhum (skills existentes cobrem)

### POPs a criar
- Nenhum POP próprio — usa o `template-raio-x.md` (seção "Operação" do Raio-X)

### Critério de qualidade
- Cliente entende em ≤ 5 min qual a operação dele está vs. poderia estar
- Sem entrar em IA ainda — só iluminação do gap

### Profundidade real
**B/M** (referência breve, análise leve) — D1 só planta curiosidade, profundidade real fica em D4.

### Dependência
- Depende de C1 estar mapeada (Sequência Inversa: sem foto do todo, não dá pra ver gargalos)

---

## 📋 C3 — Clientes que pagam (CS/Retenção) — profundidade **B**

### Saída tangível
- **Heatmap de retenção** (1 página) — onde o cliente tem churn invisível
- Golden nuggets de expansão (upsell/co-sell possíveis)

### Operação
1. **Análise do portfolio atual** — quem são os clientes que pagam, quanto cada um paga, tempo de casa
2. **Cálculo de NRR/LTV implícito** — sem entrar nas métricas do D2 (sem dashboard trimestral)
3. **Lista de expansão orgânica** — clientes com upgrade/cross-sell natural possível

### Skills envolvidas
**Curadas:**
- `customer-pulse`, `customer-pulse-check` (`KB/small-business/skills/...`)
- `ticket-triage` (`KB/customer-support/skills/ticket-triage`)
- `kb-article` (`KB/customer-support/skills/kb-article`)
- `customer-research` (já curada)
- `churn-prevention` (`Mkt/skills/churn-prevention`)

**Gap:** nenhum (skills de catálogo cobrem)

### POPs a criar
- Nenhum POP próprio — usa 1 seção do Raio-X (C3)

### Critério de qualidade
- Cliente entende que tem receita escondida na base (expansão)
- Não entra em playbooks do D5 — só iluminação

### Profundidade real
**B** (referência breve) — D1 só expõe o gap; reestruturação entra em D4.

### Dependência
- Depende de C1 (sem saber onde o cliente está, não dá pra mapear retenção real)

---

## 📋 C4 — Aquisição girando (comercial/marketing) — profundidade **B**

### Saída tangível
- **5 ângulos de posicionamento** prontos para a isca
- **Esboço de página de captura** (texto, não peça final — entregue após D2 upsell)

### Operação
1. **Diagnóstico de aquisição atual** — onde o cliente busca clientes hoje (sem ofensividade)
2. **Lições da pré-D1** — o que funcionou/não funcionou na isca/formulário 1
3. **5 ângulos de marketing** — 5 formas de falar o mesmo valor (usar `marketing-ideas`)

### Skills envolvidas
**Curadas:**
- `marketing-plan`, `marketing-ideas`, `marketing-psychology` (`Mkt/skills/...`)
- `lead-magnets`, `copywriting`, `copy-editing`, `emails` (`Mkt/skills/...`)
- `competitor-profiling`, `programmatic-seo` (`Mkt/skills/...`)
- `brand-voice` (`KB/partner-built/brand-voice`)

**Gap do PROJ-03:** `brand-lct` — aplicar manifesto da LCT em qualquer peça, incluindo essas novas do cliente (uso cross, não só LCT)

### POPs a criar
- **A criar:** `pop-isca-pre-d1.md` — POP genérico da isca que antecede o D1 (não faz parte do D1 entregue, mas prepara)
- `pop-execucao-posicionamento-cliente.md` — roteiro dos 5 ângulos

### Critério de qualidade
- Cliente sai do D1 com 5 opções reais, não com recomendação vaga
- Sem entrar em produção de peça — só insight

### Profundidade real
**B** (referência breve) — operacional de fato fica no D2 ou no Upsell Pós-D1

### Dependência
- Depende de C1 estar sólida — sem saber onde está, falar de aquisição soa desconectado

---

## 🧬 O que une as 4 camadas (macro)

| Camada | Saída | Skill-âncora | POP central | Profundidade | Depende de |
|---|---|---|---|---|---|
| **C1** | Raio-X completo | `customer-research` + `data-visualization` + `ceo-interview` (gap) | `pop-diagnostico-ceo-90m.md` | **M** | — |
| **C2** | Mapa de ineficiência (1 pág) | `process-optimization` | (seção Raio-X) | **B/M** | C1 |
| **C3** | Heatmap de retenção (1 pág) | `customer-pulse` | (seção Raio-X) | **B** | C1 |
| **C4** | 5 ângulos de posicionamento | `marketing-ideas` + `brand-lct` (gap) | `pop-execucao-posicionamento-cliente.md` | **B** | C1 |

## 🪜 Plano macro → micro

**Sequência de execução sugerida (Sequência Inversa):**

1. **Macro** (esta página): visão das 4 camadas, saídas, skills, ordens ✅ (esta página)
2. **Micro Fechado:** pega-se cada camada e detalha **entregáveis específicos** (esqueleto de Raio-X, esqueleto de heatmap, esqueleto de 5 ângulos, etc.)
3. **Micro Vivo:** cada camada vira entregável real quando escolhida

**Para onde ir agora?**

A escolha "C1 primeiro" da Sequência Inversa está alinhada. **A próxima sprint é criar `pop-diagnostico-ceo-90m.md`** (elo central do D1 — sessão 90 min) + reativar `template-raio-x.md` do archive. Esse é o **primeiro entregável micro da camada C1**.

Antes de partir pra execução, decidir:

### Próxima ação sugerida

| Opção | O que faz | Quem decide |
|---|---|---|
| **A** | Detalhar C1: definir 5 perguntas-chave do CEO + 7 seções do Raio-X + esqueleto POP | Eu (C1) + Você (validar 5 perguntas-chave) |
| **B** | Detalhar outra camada (C2/C3/C4) primeiro — útil se quiser ver com clareza todas as camadas antes de atacar uma | Eu (detalhe da camada selecionada) |
| **C** | Todas as 4 camadas detalhadas em página só com esqueleto (então a página macro fica completa) | Eu — 4 entregáveis |
| **D** | Pensar antes no que você traz pra próxima sessão | Você |

Sugestão firme: **A**, porque é a Sequência Inversa do método e o C1 é o núcleo.

---

## 📝 Histórico

| Data | Mudança | Quem |
|---|---|---|
| 2026-07-09 | v1 inicial da página (macro) | eu |
