# 🧠 Memória do Projeto — PROJ-02 LCT Consulting

> **Esta é a memória de longo prazo DESTE ENVELOPE dentro do arranjo skill-first.**
> Não é cópia da memória central original (essa está em [`strategy/memoria-central-original.md`](./strategy/memoria-central-original.md)).
> Esta aqui é só da operação nova, dentro de `42_skills - Projeto 1/projetos/PROJ-02-*/`.

---

## 📅 Linha do tempo de decisões

### 2026-07-09 — Decisão: espelhar em vez de migrar definitivamente
- **Contexto:** Você tinha `LCT_Consulting_SDD/` rodando desde abril/2026 (constitution ratificada em 05/jul, Motor v0.0.3, 3 POPs prontos). Precisava dar continuidade sem perder nada.
- **Opções:** (1) migrar tudo e tornar o novo canônico, (2) espelhar e manter ambos ativos, (3) só atalhar via ponteiro.
- **Decisão:** opção (2) — espelhar.
- **Por quê:** você quer poder consultar o original como referência (em `.gemini/`, `.opencode/`, etc.) enquanto opera daqui. Cross-LLM original fica lá; aqui a gente opera com Claude + spec-kit + skills.
- **Consequência esperada:** 100% das sessões futuras operam aqui; original fica preservado como histórico.

### 2026-07-09 — Decisão: quais ativos migrar
- **Contexto:** O Motor tem arquivos de integração (`.claude/`, `.gemini/`, `.opencode/`, `.specify/`) e arquivos substantivos (constitution, manifesto, estratégia, matriz, POPs).
- **Decisão:** migrar só os substantivos. Integrações ficam no original.
- **Por quê:** reduz duplicação; mantém o envelope lean; o original serve como "cápsula de integração" histórica.

### 2026-07-09 — Decisão: elenco de skills iniciais
- **Contexto:** Precisava escolher sem virar skill-spam.
- **Decisão:** 22 skills curadas, cobrindo: marketing captação, social/autoridade, design material, jurídico, financeiro, operação interna, e criação de agentes.
- **Por quê:** espelham os 7 departamentos da empresa-de-skills; cobrem as 4 Camadas × 5 Degraus do Motor (não exaustivamente — adicionar sob demanda).

### 2026-07-09 — Decisão: shortlist de skills dos forks era "adiada" — não é mais
- **Contexto:** Estado atual marcava "shortlist de skills dos forks adiada até D1 fechar".
- **Decisão:** essa shortlist vira o **próximo alvo** do PROJ-02 (curadoria em [`skills-curadoria/`](./skills-curadoria/)), antes de tentar fechar D1.
- **Por quê:** agora temos catálogo estruturado — a curadoria ajuda a fechar o D1 com elenco enxuto e justificado.

### 2026-07-09 — VIRADA DE CHAVE (mesma data, decisão de porte)
- **Contexto:** os 3 POPs do Elo 6 (`template-raio-x`, `pop-diagnostico-final`, `README` antigo do índice de pops) foram criados no vácuo — antes da curadoria de skills. Você quer **reconstruir o Degrau 1 inteiro** cruzando 5 Degraus × 4 Camadas com o novo catálogo.
- **Decisão:** reset de D1 inteiro (profundidade `.`), arquivamento dos 3 POPs (regra IX), incremento de patch da matriz (v0.0.3 → v0.0.4), novo snapshot de estado (09/jul).
- **Por quê:** POPs sem alinhamento com skills viram artefatos órfãos. O C1 (Sequência Inversa) do D1 vai ser reconstruído à luz das capacidades reais do catálogo.
- **Consequência:** Sprint 1 da curadoria passa a ser o foco absoluto. Ações que dependiam dos POPs arquivados (ex.: `pop-sessao-90m.md`, `Elo 5 do D1`) precisam ser replanejadas após Sprint 1.
- **Política:** Elo 5 (`pop-sessao-90m`) **foi automaticamente rebaixado** de "próximo alvo" para "aguardando Sprint 1" — não vamos mais criar POPs no vácuo.

### 2026-07-09 — ENRIQUECIMENTO ESTRATÉGICO DA MATRIZ (v0.0.4 → v0.0.5)
- **Contexto:** Você lembrou que os **5 Degraus foram desenhados pela LUZ HUB** no relatório `lct-transformation-90d.md` (§"A Escada de Valor — Cinco Degraus"). Eu tinha mapeado `formato` e `ticket_referencia` no `eixo_y` do JSON, mas estavam achatados — sem o **papel no funil**, **gatilho para o próximo degrau**, nem o **link explícito para a fonte estratégica**.
- **Decisão:** v0.0.5 — extender o Eixo Y com 3 campos estratégicos: `papel_no_funil`, `gatilho_proximo_degrau`, `fonte_estrategica_linha`. Adicionei a **lógica do funil** da LUZ HUB §390 como campo top-level do `eixo_y`.
- **Por quê:** o cruzamento metodológico (D×C×Cap. Codexo) sem entender o **substrato estratégico** do Degrau vira exercício abstrato. Cada Degrau tem **por que** e **pra quê**, não só **o quê**.
- **Consequência:** o exercício de estudo de cada célula (próximo passo) usa 3 fontes (LUZ HUB + Motor + The Revenue Codex) — não só 2.

### 2026-07-09 — ESTUDO PROFUNDO POR CÉLULA (novo formato aprovado)
- **Contexto:** Você apontou que o apontamento de capítulos não basta — precisamos entender profundamente cada cruzamento.
- **Decisão:** cada célula (D×C) vira um **documento de estudo formal** em `knowledge/motor-lct/estudos/celula-Dx-Cy.md`, produzido com skills do catálogo: `search` → `digest` → `knowledge-synthesis` → `write-spec` (ou `competitive-brief`).
- **Por quê:** o catálogo tem skills de pesquisa/síntese que servem como "estudiosos". Sem isso, o cruzamento fica raso.
- **Consequência:** Sprint 1 da curadoria vira Sprint de Estudo. Enfoque inicial: D1×C1 (Sequência Inversa). Aprofundamos 1 célula por turn com seu peer-review antes da próxima.

---

## 🔍 Contexto carregado

- **Quem é o cliente:** Leandro (LCT Consulting). ICP dele: fundadores-CEO de empresas B2B tech (R$ 20-70M), 42-58 anos, travados no teto, crendo que o problema é vendas.
- **Onde está o Motor:** v0.0.5 — D1 resetado, Eixo Y enriquecido com substrato estratégico LUZ HUB.
- **Onde está o próximo gap:** **Estudo profundo de D1×C1** com kit completo (search → digest → knowledge-synthesis → write-spec). Documento em [`knowledge/motor-lct/estudos/celula-D1-C1.md`](./knowledge/motor-lct/estudos/celula-D1-C1.md).
- **Decisões abertas (do estado 07/jul, seguem em aberto):**
  1. Quem produz o relatório-isca (formulário 1)?
  2. O que é vendido na call de 1h?
  3. Upsell para D2, D3 ou caso a caso?
  4. Conteúdo do formulário 1.
  5. Conteúdo do formulário 2.
  6. Estrutura da reunião 90 min (fixa/orgânica/híbrida).

---

## 📚 Referências e links úteis

| Tipo | Descrição | Link |
|---|---|---|
| Constitution do Motor | Princípios inegociáveis | [`constitution-do-motor-lct.md`](./constitution-do-motor-lct.md) |
| Manifesto LCT | Voz e personalidade | [`strategy/manifesto.md`](./strategy/manifesto.md) |
| Estratégia 90 dias | Diagnóstico + plano de transformação | [`strategy/lct-transformation-90d.md`](./strategy/lct-transformation-90d.md) |
| Motor LCT | Matriz + Governance + POPs | [`knowledge/motor-lct/`](./knowledge/motor-lct/) |
| Estado atual (09/jul — virada) | Onde paramos em 09/jul (reset D1) | [`knowledge/motor-lct/estado-atual-2026-07-09.md`](./knowledge/motor-lct/estado-atual-2026-07-09.md) |
| Cruzamento metodológico | 5×4 × Cap. The Revenue Codex (v1 validação) | [`knowledge/motor-lct/cruzamento-motor-x-codex.md`](./knowledge/motor-lct/cruzamento-motor-x-codex.md) |
| Planejamento D1 macro | D1 × 4 Camadas (macro) | [`knowledge/motor-lct/d1-por-camada.md`](./knowledge/motor-lct/d1-por-camada.md) |
| Matriz (Motor × Cap. Codexo) | Matriz enriquecida v0.0.5 | [`knowledge/motor-lct/matriz.md`](./knowledge/motor-lct/matriz.md) |
| Catálogo de skills | Inventário global | `../../../skills-catalogo/` |
| Original LCT_SDD | Cápsula cross-LLM (read-only por convenção) | `C:\Users\user\Workspace\meus_projetos\LCT_Consulting_SDD\` |

---


## ✅ REVISÃO DE BRAND-LCT (2026-07-09, Sprint 1 do PROJ-03 concluída)

A skill **brand-lct v0.1.0** foi instalada em  (com 218 linhas, 11.9KB), após:
- RED baseline (cap com skill genérica: violava 6/10 regras)
- GREEN Cenário 1 (cap D1 com skill: 10/10)
- GREEN Cenário 2 (1 dos 5 ângulos do D1×C4: 9/10 aplicáveis)
- GREEN Cenário 3 (follow-up email pós-D1: 10/10)
- REFACTOR + v0.1.0 fechado

**Revisão retroativa (todos os artefatos do PROJ-02 passaram pela checklist de 10 regras):**

| Artefato | Status |
|---|---|
| estudos/celula-D1-C1.md | ✅ sem violações (uso de 'único' em 'pagamento único' e 'ICP único' são técnicos) |
| estudos/celula-D1-C2.md | ✅ sem violações |
| estudos/celula-D1-C3.md | ✅ sem violações |
| estudos/celula-D1-C4.md | ✅ sem violações |
| cruzamento-motor-x-codex.md | ✅ sem violações |
| d1-por-camada.md | ✅ sem violações |
| estado-atual-2026-07-09.md | ✅ sem violações |

**Conclusão:** os artefatos já estavam coerentes com a brand-lct antes mesmo da skill existir. Isso valida que o estudo metodológico prévio (intencionalmente construído com base no Manifesto) produziu peças alinhadas. A skill agora formaliza e protege essa coerência para o que vier depois.

**Próximo passo (Sprint 2 do PROJ-03):** construir a skill **ceo-interview** — protocolo das 5 perguntas-chave do Cap. 07 (The Revenue Codex). Mesmo ciclo TDD. Bloqueio de D1×C1 entrar em produção.


## 🎉 MOTOR LCT METODOLOGICAMENTE COMPLETO (2026-07-09, v0.0.7 da matriz)

**20 estudos publicados** em `knowledge/motor-lct/estudos/` — D1-D5 inteiro × C1-C4 inteiro. Cada estudo cruzando 3 fontes (LUZ HUB + Motor + The Revenue Codex) com caps mapeados, skills identificadas, POPs a criar/especificados, e lentes LCT integradas.

**Resumo:**
- **20 células estudadas** (5 Degraus × 4 Camadas)
- **30+ POPs identificados** para criar/reativar
- **Cap. 20 censurado em D1×C4, D2×C4, D3×C4** (Fundador lidera vendas — choca com Manifesto LCT §1)
- **Cap. 18 substitui Cap. 20** em contextos onde o capítulo fala de fundador nas vendas iniciais (substituição honesta)
- **3 novos skills** instaladas no fork `meus_forks/42_skills/`:
  - brand-lct/SKILL.md (Marketing/) — voz LCT codificada
  - ceo-interview/SKILL.md (Developers/knowledge-work-plugins/design/skills/) — protocolo 5 perguntas-chave Cap. 07
  - motor-governance/SKILL.md (Developers/superpowers/skills/) — validador 6 checks para mudanças no Motor

**Conformidade:**
- Constituição §I (Sequência Inversa): respeitada
- Constituição §II (Profundidade Universal B/M/A): sem não aplicável
- Regra VII (Sincronia MD↔JSON): MD em v0.0.7, JSON em v0.0.7
- Regra IX (POPs são Vivos): 3 POPs do Elo 6 arquivados (sem delete)
- Regra X (Versionamento Semântico): 5 bumps sucessivos (0.0.3 → 0.0.7)

**Próximas ações (NÃO-Projeto):**
1. Iniciar **produção do D1** (4 POPs + 2 reativações do archive) usando as 3 skills novas
2. Aplicar **marcadores [adotado:] / [rejeitado:]** no The Revenue Codex original (governance Regra III)
3. Git init no PROJ-02 + commit documentado

**Lição aprendida durante o exercício:**
Apontamento de caps (v1) ≠ entendimento profundo (v3+). O estudo profundo com knowledge-synthesis foi essencial para cruzar as 3 fontes e descobrir coisas que a matriz isoladamente escondia — ex: Cap. 20 censurado, Cap. 18 como substituto, o Múltiplo de Saída como lente autoral LCT (Gap G3).

## 🎉 D1 INTEIRO FECHADO (2026-07-09, v0.0.6 da matriz)

**Com 4/4 células do D1 estudadas**, o Degrau 1 está metodologicamente estruturado. Detalhes completos em [knowledge/motor-lct/estudos/](./knowledge/motor-lct/estudos/).

| Célula | Profundidade | Caps do The Revenue Codex | Saída tangível |
|---|---|---|---|
| **D1×C1** (Onde está) | M | 02, 03, 04, 06, 07 | Raio-X do Cliente (PDF 7-10 págs, base de tudo) |
| **D1×C2** (Máquina pronta) | B/M | 06, 10, 24 | Mapa de ineficiência (1 pág) + lista de IA-amplificáveis |
| **D1×C3** (Clientes que pagam) | B | 08, 25, 26, 27, 28 | Matriz Valor×Fit (1 pág) + expansão orgânica |
| **D1×C4** (Aquisição girando) | B | 11, 12, 13, 14, 15, 18, 21 (Cap. 20 censurado) | 5 ângulos de posicionamento + convite D2 |

**Próxima fase (plano de produção por célula):**
1. Criar 4 POPs novos: pop-diagnostico-ceo-90m, pop-auditoria-maquina-cliente, pop-pulse-clientes-atuais, pop-5-angulos-posicionamento-cliente
2. Reativar 2 POPs do : template-raio-x, pop-diagnostico-final
3. Construir a skill  (gap do PROJ-03) — protocolo das 5 perguntas-chave do Cap. 07
4. Construir a skill  (gap do PROJ-03) — coerência de voz nas peças D1×C4
5. Aplicar marcadores  /  no The Revenue Codex original (Regra III da governance)
6. Bump da matriz para v0.0.6 com profundidade final e caps por célula
7. (futura) Estudos de D2-D5 seguindo o mesmo kit

**Conformidade confirmada:**
- Sequência Inversa (Constituição §I): ✅ C1 → C2 → C3 → C4
- Profundidade universal (Constituição §II): ✅ sem '.' — todas as células tem B/M/A
- Sincronia MD ↔ JSON (Regra VII): ✅ ambas em v0.0.6
- POPs são vivos (Regra IX): ✅ 3 POPs do Elo 6 arquivados, não deletados
- Versionamento semântico (Regra X): ✅ bumps 0.0.3 → 0.0.4 → 0.0.5 → 0.0.6 (patches consistentes)

---

## 📚 Referências dos estudos D1

- **D1×C1:** [knowledge/motor-lct/estudos/celula-D1-C1.md](./knowledge/motor-lct/estudos/celula-D1-C1.md)
- **D1×C2:** [knowledge/motor-lct/estudos/celula-D1-C2.md](./knowledge/motor-lct/estudos/celula-D1-C2.md)
- **D1×C3:** [knowledge/motor-lct/estudos/celula-D1-C3.md](./knowledge/motor-lct/estudos/celula-D1-C3.md)
- **D1×C4:** [knowledge/motor-lct/estudos/celula-D1-C4.md](./knowledge/motor-lct/estudos/celula-D1-C4.md)
- **Cruzamento 5×4 × Codexo:** [knowledge/motor-lct/cruzamento-motor-x-codex.md](./knowledge/motor-lct/cruzamento-motor-x-codex.md)

---

## 💡 Aprendizados (do envelope, não do Motor)

> (Vazio — projeto recém-criado)

---

## 🚧 Tentei e não funcionou (do envelope)

> (Vazio)

---

## 👥 Pessoas chave

| Nome | Papel | Contato |
|---|---|---|
| Você | Sócio-fundador / decisor | direto aqui |
