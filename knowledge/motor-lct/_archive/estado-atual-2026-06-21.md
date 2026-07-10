# Estado da conversa — 2026-06-21

> **Status:** documento de transição. Captura o que foi decidido na conversa mas ainda não virou artefato canônico. Não substitui `matriz.md`, `governance.md` ou qualquer outro arquivo oficial — é um snapshot do "onde paramos".

---

## Decisões consolidadas

### Sobre o Motor LCT

- **Nome:** `motor-lct` (não `framework-lct`, não `metodologia-lct`).
- **Granularidade inicial:** matriz única primeiro, expansão por Degrau sob demanda (pastas dedicadas só aparecem quando conteúdo de uma combinação específica merece arquivo próprio).
- **Governance:** documento separado `governance.md` (5 tipos de mudança + checklist).
- **Conteúdo:** matriz contém **só "para cliente"** — material que sai da LCT e o cliente usa na operação dele. Material de uso interno (marketing, prospecção, processo Leandro) mora em pasta separada quando aparecer.
- **Sobre rejeição de capítulos do The Revenue Codex:** "decidir caso a caso, sem rejeição automática por choque de tese". Eu levanto o choque, você arbitra.

### Sobre os documentos fundacionais

- **Relatório Estratégico** (`strategy/lct-transformation-90d.md`) é **insumo interno da LCT** — escrita sobre a LCT, seus desafios e seu plano de 90 dias. As ofertas (Degraus) são objeto de cruzamento com a metodologia (The Revenue Codex).
- **O que estamos construindo agora** é método/conteúdo **para o cliente da LCT** — não para a LCT.
- **Compêndio (The Revenue Codex)** é insumo de práticas de mercado. Sem menção a autor na operação interna. Pasta preparada para receber outros autores no futuro.

### Sobre os 7 choques metodológicos (The Revenue Codex × Manifesto)

| Choque | Tese do The Revenue Codex | Tese do Manifesto | Status |
|---|---|---|---|
| **C1** Funil direto vs. sequência inversa | Funil top-down (Aquisição→Vendas→CS→Métricas) | Sequência inversa (Causa→Máquina→Clientes→Aquisição) | Adaptação necessária — material do compêndio é reaproveitável se renomeado |
| **C2** "Vender mais" como objetivo vs. consequência | Aquisição como objetivo | Aquisição como consequência da arquitetura estar pronta | **MAIS GRAVE sob "para cliente"** — cliente percebe como incoerência grave |
| **C3** POPs portáteis vs. cirurgia/operação por dentro | Artefatos portáteis pra leitor executar sozinho | Código rodando no P&L do cliente, agente de IA, presença semanal | Igual — formato do entregável |
| **C4** ICP amplo vs. ICP nível CPF | ICP genérico (matriz Valor×Fit) | ICP nível CPF (fundador 42-58, R$20-70MM) | Quase neutro — cliente não vê o ICP direto |
| **C5** Métricas SaaS vs. métricas de teto/saída | MRR, CAC, LTV, Churn, North-Star Dashboard | EBITDA, múltiplo de saída, NRR como sinal de arquitetura, redução de custo via IA | **MAIS GRAVE sob "para cliente"** — cliente do ICP LCT não tem MRR puro |
| **C6** Cadência contínua vs. prazo cravado | Plano 30/90/120 contínuo (RevOps full throttle) | 90 dias cravados, recusa retainer infinito | Menos grave — adaptar horizonte temporal |
| **C7** Framework importado vs. cicatriz (NOVO sob lente "para cliente") | Cases do Vale do Silício (Airbnb, PayPal, Slack) | Autoridade vem da cicatriz brasileira, não de framework importado | Grave — censura narrativa importada sem perder lógica técnica |

### Sobre os 8 gaps (DNA-LCT que precisa virar motor autoral)

- **G1** Transição Fundador-Técnico → CEO Estrategista
- **G2** Substituição de camada operacional por agentes de IA
- **G3** Construção de múltiplo de saída (M&A readiness) — tem fonte externa (Advisia, Vinci Partners)
- **G4** "Operar por dentro" do cliente (presença semanal)
- **G5** Diagnóstico de teto invisível ("Teto dos 60M") — tem fonte parcial (estudo FDC 2024)
- **G6** Comitês executivos / conselho de administração — tem fonte externa (literatura clássica de board)
- **G7** Precificação de consultoria de ticket alto — entregável nativo do Motor
- **G8** Honestidade brutal como método (não técnica, postura)

---

## Matriz de cruzamento Degrau × Camada × Conteúdo do The Revenue Codex

> Gerada por mapeador agent em 2026-06-21. Cada célula lista capítulos/temas do The Revenue Codex que se encaixam, com justificativa em 1 frase. **Não tem profundidade, POPs, agentes nem automações ainda — só conteúdo.**

### D1 — Sessão Estratégica Executiva (90 min + relatório 7-10 pp, R$ 2.500)

**C1 — Onde está:** caps 02 (Impacto silencioso dos gargalos), 03 (Simulação financeira), 04 (Efeito nos números), 07 (Re-check PMF 5 perguntas), 30 (CAC/Payback/LTV), 29 (Métricas 20/80).

**C2 — Máquina pronta:** caps 06 (Fundamentos), 24 (CRM mínimo), 32 (North-Star Dashboard).

**C3 — Clientes que pagam:** caps 31 (Churn/NRR), 08 (ICP Matriz Valor×Fit), 25 (Retenção turbinada), 26 (Onboarding 30-30-30), 28 (Renovação 90d).

**C4 — Aquisição girando:** caps 11 (Aquisição relâmpago — como "o que NÃO fazer agora"), 22 (Demo 7 passos — referência rápida), 09 (Oferta/preço 80/20 — leitura crítica).

D1 é o degrau de menor densidade (4-6 capítulos por camada) — coerente, é degrau curto.

### D2 — Mentoria Individual do CEO (3-6 meses, 2 sessões/mês)

**C1:** caps 03, 07, 30, 29, 32.

**C2:** caps 06, 24, 10 (Roadmap RICE), 33 (Plano 30-90-120).

**C3:** caps 25, 26, 27 (Health Score 1.0), 28, 31.

**C4:** caps 08, 09, **20** ⚠ (Fundador lidera vendas), 19, 21 (BANT Turbo).

**Choque:** Cap. 20 (Fundador lidera vendas iniciais). Codex diz fundador é o melhor vendedor inicial; LCT diz fundador precisa parar de ser vendedor. Tensão a resolver.

### D3 — Diagnóstico de Arquitetura do Crescimento (2-4 sessões + relatório + board)

**C1:** caps 02, 03, 04, 07, 30, 31, 29, 32, 33. (9 capítulos — célula mais densa da Camada 1.)

**C2:** caps 06, 10, 24, 33.

**C3:** caps 08, 25, 26, 27, 28, 31.

**C4:** caps 11, 12 (Content Velocity), 13 (Cadência Outbound), 14 (ABM pocket), 15 (Programa indicação), 16 (Ads), 09.

### D4 — Consultoria LCT Full (90-180 dias, equipe + Mowia)

**C1:** caps 03, 30, 31, 29, 32, 33.

**C2:** caps 06, 10, 24, 19, 22, 23.

**C3:** caps 25, 26, 27, 28, 31.

**C4:** caps 11, 12, 13, 14, 15, 16, 08, 09, 21, 19, **20** ⚠, 17 (Conversão Express), 18 (Desmistificando vendas), 33. (14 capítulos — célula mais densa do motor.)

### D5 — Conselho Estratégico (mensal, ± equity)

**C1:** caps 32, 29, 30, 31, 33.

**C2:** caps 24, 10, 06.

**C3:** caps 28, 25, 27, 31.

**C4:** caps 09, 11, 14, **20** ⚠, 16 ⚠, 30, 33.

### Síntese da matriz

**5 capítulos onipresentes (todos os 5 Degraus):**
- 32 — North-Star Dashboard
- 30 — CAC, Payback e LTV
- 31 — Churn e NRR
- 29 — Métricas 20/80
- 25 — Retenção turbinada

**Células mais densas (em volume de material):**
1. D4 × C4 — 14 capítulos
2. D3 × C1 — 9 capítulos
3. D3 × C4 — 8 capítulos
4. D4 × C3 — 5 capítulos mas POPs canônicos densos
5. D4 × C1 — 6 capítulos, todos de métrica

**Choques mais sistêmicos (aparecem em mais Degraus):**
- Cap. 20 (Fundador lidera vendas) — D2, D4, D5 (3 Degraus).

---

## Fluxo do Degrau 1 (em 6 peças — não decidido ainda)

Você descreveu o fluxo do Degrau 1 com precisão. As 6 peças que ainda precisam de decisão:

1. **Quem produz o relatório-isca do formulário 1?** — você mesmo manual? template semi-pronto? 100% automatizado?
2. **O que é vendido na call presencial?** — só D1 (R$ 2,5k), pacote D1+D2, ou D1 com oferta clara de D2 no final?
3. **Upsell da reunião final de 1h** — D2 (Mentoria) ou D3 (Diagnóstico)? Ou depende do caso?
4. **Conteúdo do formulário 1** — quantas perguntas, qual a "pergunta top" (matadora ou topo de funil)?
5. **Conteúdo do formulário 2 (pós-compra)** — financeiro, comercial, operacional, estratégico, tudo?
6. **Estrutura da reunião de 90 min** — agenda fixa, conversa orgânica, híbrido?

**Decisão acordada:** ordem invertida — primeiro curadoria do conteúdo do The Revenue Codex por Degrau (já feito), depois estruturar cada entregável, depois profundidade/POPs/agentes/automações.

---

## Sobre os forks de agentes

10 forks em `C:\Users\user\Workspace\meus_forks\` foram selecionados pra consulta:

1. **agency-agents** — coleção de agentes com personalidade pra Claude Code.
2. **claude-skills-for-mckinsey-analysis** — 10 skills de estratégia (Diagnosis + Execution).
3. **conselho-executivo-ia** — framework que simula conselho de administração.
4. **content-skill-graph** — motor de conteúdo (pastas audience/engine/outputs/platforms/voice, com `outputs_mowia/`).
5. **goose-skills** — 108 skills de Growth & GTM.
6. **growth-os-skills** — time de IA em 3 níveis, em português, brasileiro (Accelera 360).
7. **marketingskills** — skills de marketing (CRO, SEO, growth engineering).
8. **open-saas** — template SaaS completo (Wasp + React + NodeJS + Prisma) — **diferente, é starter kit não skill**.
9. **opensquad** — framework de orquestração multi-agente (squads persistentes com checkpoints de aprovação humana). Suporta 9 IDEs incluindo Claude Code.
10. **ui-ux-pro-max-skill** — design intelligence pra UI/UX (161 regras, 67 estilos).

**Discussão sobre opensquad:** levantada a hipótese de ser orquestrador de outros agentes. Conclusão: **Claude já é o orquestrador da sessão** (efêmero, síncrono, com você no loop). opensquad seria orquestrador de **pipeline persistente** (marketing recorrente, prospecção, geração de conteúdo do motor) — nível diferente. **Decisão adiada** até saber qual é a demanda real de capabilities do Degrau 1.

---

## Próximos passos (parado em 2026-06-21)

Sequência acordada (caminho 1-2-3-4):

1. **Mapear escopo do Degrau 1** para fechar o desenho antes de partir pra motor — **em progresso**.
2. **Decidir as 6 peças do Degrau 1** (formulário 1, relatório-isca, call, formulário 2, reunião 90 min, reunião final, upsell).
3. **Preencher célula D1 × C1 da matriz** com base no Degrau 1 fechado.
4. **Só depois:** shortlist de skills/agentes dos forks selecionados que viriam pra esse caso.

---

## Convenções estabelecidas

- **Tudo versionado em git.** Working tree limpo, 3 commits na `master`.
- **3 integrações paralelas ativas:** claude, gemini, opencode.
- **Constraint cross-LLM** é invariante: `.specify/` e `specs/` são fonte canônica, skills são atalhos.
- **Não rodar `/init` do Claude Code** neste projeto (colide com `CLAUDE.md` gerenciado pelo spec-kit).
- **Marketing é uso interno**, não um terceiro bucket separado.
- **Cada camada tem profundidade por Degrau** (não é matriz simétrica).
- **Material de uso interno da LCT** (processos Leandro, prospecção, marketing) **não entra na matriz** — vive em pasta separada (`motor-lct/interno/` ou similar) quando aparecer.

---

## Última ação antes de fechar a sessão

Salvar este documento como snapshot e atualizar a memória do projeto (`project-lct-consulting-sdd.md`) pra apontar pra ele. Isso garante que a próxima sessão (você ou outro LLM) consegue achar o estado completo em `knowledge/motor-lct/estado-atual-2026-06-21.md` carregando a memória persistente.