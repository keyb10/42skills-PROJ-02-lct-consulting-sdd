# Estado da conversa — 2026-07-07

> **Status:** documento de transição. Captura o que foi decidido na conversa e o estado físico do Motor nesta data. Não substitui `matriz.md`, `governance.md`, `constitution.md` ou qualquer outro arquivo oficial — é o snapshot do "onde paramos".
>
> **Histórico:** o snapshot anterior (`estado-atual-2026-06-21.md`) foi movido para `knowledge/motor-lct/_archive/`, conforme a regra IX da constituição (nada se deleta, move-se).

---

## 1. Onde a régua está hoje

- **Matriz do Motor:** v0.0.3 — 5 Degraus × 4 Camadas conceitualmente desenhados, com profundidade B/M/A variável por célula.
- **Sincronia MD↔JSON:** mantida (regra VII da constituição — espelho inegociável).
- **Constituição:** ratificada em 2026-07-05, versão 1.0.0, 10 princípios inegociáveis.
- **Governança:** 5 tipos de mudança + checklist antes de commitar.
- **Manifesto:** vivo, 10 seções (identidade → soluções), é a fonte de tom e crenças.
- **3 integrações paralelas ativas:** Claude, Gemini, Opencode. `.specify/` e `specs/` são fonte canônica; skills são atalhos.

## 2. POPs físicos existentes

| Arquivo | Elo | Status |
|---|---|---|
| `pops/template-raio-x.md` | Elo 6 (template do relatório) | Pronto (v1.0.0) |
| `pops/pop-diagnostico-final.md` | Elo 6 (POP de condução da call) | Pronto (v1.0.0) |
| `pops/README.md` | — | Pronto (índice) |

Os demais POPs citados na matriz (`pop-sessao-90m`, `pop-onboarding-mentoria`, `pop-accountability-trimestral`, `pop-imersao-dados`, `pop-geracao-diagnostico`, `pop-implantacao-mowia`, `pop-reestruturacao-processos`, `pop-maquina-vendas`, `pop-preparacao-conselho`) **ainda são placeholders conceituais**, não artefatos físicos.

## 3. Degrau 1 — Estado do fluxo (Elo 1 a 6)

Sequência acordada: fechamento de trás pra frente, partindo do entregável final.

| Elo | Descrição | Status |
|---|---|---|
| **Elo 1-3** | Pré-Degrau: conteúdo de atração → isca (formulário 1) → reunião de vendas 1h (30 min análise da isca + 30 min pitch do D1) | Não iniciado |
| **Elo 4** | Coleta de dados profunda pós-venda (financeiro, comercial, operacional, estratégico) | Não iniciado |
| **Elo 5** | Reunião Estratégica 90 min (gravada/transcrita) — insumos: isca + coleta profunda | Não iniciado — **próximo alvo** |
| **Elo 6** | Apresentação do Diagnóstico Final 90 min: entrega do Raio-X + upsell | **Concluído** (template + POP com qualidade "Uau") |

## 4. Decisões consolidadas que permanecem válidas

Estas vinham do snapshot de junho e seguem em vigor — não foram revisitadas nem revogadas:

- **Nome do motor:** `motor-lct` (não `framework-lct`, não `metodologia-lct`).
- **Granularidade inicial:** matriz única primeiro; expansão por Degrau sob demanda.
- **Conteúdo da matriz:** só "para cliente" — material que sai da LCT e o cliente usa na operação dele. Material de uso interno (marketing, prospecção, processo Leandro) vive em pasta separada (`motor-lct/interno/`) quando aparecer.
- **Rejeição de capítulos do The Revenue Codex:** decidir caso a caso, sem rejeição automática por choque de tese. Eu levanto o choque, Leandro arbitra.
- **Relatório Estratégico** (`strategy/lct-transformation-90d.md`) é insumo interno da LCT — escrita sobre a LCT, seus desafios e seu plano de 90 dias.
- **O que está sendo construído agora** é método/conteúdo para o cliente da LCT — não para a LCT.
- **Compêndio (The Revenue Codex)** é insumo de práticas de mercado. Sem menção a autor na operação interna. Pasta preparada para receber outros autores no futuro.
- **Cadeia de Espetacularidade:** cada etapa precisa ser excepcional para desbloquear a próxima.
- **Marketing é uso interno**, não terceiro bucket separado.
- **Não rodar `/init` do Claude Code** neste projeto (colide com `CLAUDE.md` gerenciado pelo spec-kit).
- **Working tree versionado em git**, 3 commits na `master` (estado em 21/jun — não revalidado nesta sessão).

## 5. Choques metodológicos (The Revenue Codex × Manifesto) — análise de 21/jun mantida

Tabela de mapeamento segue válida (C1 a C7). Os choques mais sistêmicos a arbitrar em algum momento:

- **C2** "Vender mais" como objetivo vs. consequência (mais grave sob lente "para cliente").
- **C5** Métricas SaaS vs. métricas de teto/saída (mesma gravidade).
- **C7** Framework importado vs. cicatriz (censura narrativa importada sem perder lógica técnica).
- **Cap. 20 (Fundador lidera vendas iniciais)** aparece em D2, D4, D5 — precisa ser reescrito/censurado antes de virar material entregue a cliente.

## 6. 8 gaps (DNA-LCT autoral) — referência viva

- **G1** Transição Fundador-Técnico → CEO Estrategista
- **G2** Substituição de camada operacional por agentes de IA
- **G3** Múltiplo de saída / M&A readiness (fonte: Advisia, Vinci Partners)
- **G4** "Operar por dentro" do cliente (presença semanal)
- **G5** Diagnóstico de teto invisível ("Teto dos 60M") (fonte: FDC 2024)
- **G6** Comitês executivos / conselho de administração
- **G7** Precificação de consultoria de ticket alto
- **G8** Honestidade brutal como método (não técnica, postura)

## 7. Forks revisados (decisão adiada)

10 forks em `C:\Users\user\Workspace\meus_forks\` foram selecionados pra consulta. **Decisão de quais importar adiada até o D1 fechar** — sem demanda concreta de capability antes disso.

## 8. Decisões abertas que seguem pendentes

Estas vinham do snapshot de junho e **não foram resolvidas** entre 21/jun e 07/jul:

1. **As 6 peças do Degrau 1:**
   - Quem produz o relatório-isca do formulário 1? (manual / template / automatizado)
   - O que é vendido na call presencial? (só D1 / pacote D1+D2 / D1 com D2 no final)
   - Upsell da reunião final: D2, D3 ou caso a caso?
   - Conteúdo do formulário 1: quantas perguntas, qual a pergunta top?
   - Conteúdo do formulário 2 (pós-compra): escopo completo?
   - Estrutura da reunião de 90 min: agenda fixa / orgânica / híbrido?

2. **Curadoria do conteúdo do The Revenue Codex por Degrau** — parcialmente feita (mapeamento por capítulo), falta virar POP/entregável físico.

3. **Shortlist de skills/agentes dos forks** — adiada.

## 9. Próximos passos (a partir de 2026-07-07)

Sequência recomendada, mantendo o princípio de fechar o D1 de trás pra frente:

1. **Atualizar memória de projeto** (este snapshot vira referência) ✅ concluído nesta sessão.
2. **Elo 5** — criar `pop-sessao-90m.md` (roteiro da sessão de 90 min, inputs da coleta, outputs pro Elo 6).
3. **Elo 4** — definir dados operacionais, financeiros e de clientes exigidos pós-venda.
4. **Decidir as 6 peças em aberto** do D1 (formulários 1 e 2, call de 1h, upsell).
5. **Elos 1-3** — detalhamento da reunião de vendas de 1h, isca e conteúdos de atração.
6. **Preencher célula D1 × C1** da matriz com base no D1 fechado.
7. **Só então:** shortlist de skills/agentes dos forks selecionados.

## 10. Convenções ativas

- Tudo versionado em git.
- 3 integrações paralelas: claude, gemini, opencode.
- Constraint cross-LLM invariante: `.specify/` e `specs/` são fonte canônica, skills são atalhos.
- Cada camada tem profundidade por Degrau (não é matriz simétrica).
- Material de uso interno da LCT (processos Leandro, prospecção, marketing) não entra na matriz — vive em pasta separada quando aparecer.
- Ao fechar ciclo de sessão: atualizar `project-lct-consulting-sdd.md` (memória central) e a seção 3 deste snapshot.

---

**Última atualização:** 2026-07-07
**Snapshot anterior arquivado em:** `knowledge/motor-lct/_archive/estado-atual-2026-06-21.md`
