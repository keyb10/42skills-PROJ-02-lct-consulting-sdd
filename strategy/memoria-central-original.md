# LCT Consulting SDD - Memória Central do Projeto

> **Objetivo deste arquivo:** Servir como o ponto de partida (Single Source of Truth) para qualquer sessão ou agente de IA (Claude, Gemini, Cursor, etc.) que for dar continuidade ao projeto. Antes de executar qualquer ação no repositório, o agente deve ler este arquivo para entender o contexto, o que já foi feito e onde paramos.

## 1. O Projeto e o Paradigma
A LCT Consulting está em transição do modelo artesanal de "Executivo de Aluguel" para um modelo "Consultech". 
O núcleo dessa operação é o **Motor LCT**, que é vivo e opera por dentro da operação do cliente, focado em quebrar o "Teto dos 60 Milhões" atacando a infraestrutura da empresa antes de focar em marketing e vendas (sequência inversa).
- Para entender a visão completa e a comunicação, leia `.specify/memory/manifesto.md`.
- Para entender o plano de 90 dias, leia `strategy/lct-transformation-90d.md`.

## 2. Estrutura do Repositório
*   `strategy/`: Planejamento e posicionamento interno da LCT como negócio (para captação).
*   `knowledge/motor-lct/`: A base metodológica que a LCT implanta nos clientes.
*   `knowledge/external/`: Referências de mercado (como o *The Revenue Codex*).

## 3. Estado Atual (Últimos Avanços)
*Snapshot vigente:* `knowledge/motor-lct/estado-atual-2026-07-07.md` mapeia o estado completo até julho de 2026.
*Histórico:* snapshots anteriores vivem em `knowledge/motor-lct/_archive/` (regra IX da constituição).

**O que foi consolidado nas sessões anteriores:**
1.  **Constituição Ratificada (2026-07-05):** `.specify/memory/constitution.md` contém as 10 leis fundamentais do Motor LCT (Sequência Inversa, IA como Infraestrutura, Sincronia Inegociável MD/JSON, etc.) — governança cross-LLM.
2.  **Separação Conceitual da Isca:** A **Isca** (conteúdo + formulário 1 + reunião de vendas de 1h) é etapa de captação **anterior** aos Degraus. O Degrau 1 só começa após a venda dele.
3.  **Fluxo do Degrau 1:**
    - *Pré-Degrau (Venda):* Conteúdo → Isca → Reunião de Vendas (30 min análise da isca + 30 min pitch do D1).
    - *Degrau 1 (Entrega):* Coleta de dados profunda → Reunião Estratégica de 90 min (gravada/transcrita com dados da isca e coleta profunda) → Apresentação do Diagnóstico Final (90 min, entrega do Raio-X + venda de upsell).
4.  **Princípio da Cadeia de Espetacularidade:** Cada etapa precisa ser excepcional para desbloquear a próxima.
5.  **Elo 6 Estruturado (Concluído):** `pops/template-raio-x.md` e `pops/pop-diagnostico-final.md` criados com qualidade "Uau". Motor atualizado para v0.0.3 em `matriz.md` e `matriz.json`.
6.  **Memória sincronizada (2026-07-07):** snapshot de junho arquivado em `_archive/`; novo snapshot de julho vigente; esta memória central recalibrada.

## 4. Onde a próxima sessão deve iniciar (Próximos Passos)
Quem assumir a partir daqui deve focar no detalhamento dos elos do Degrau 1 de trás para frente, na ordem:

1.  **Elo 5 - Reunião Estratégica (90 min):** Criar o `pop-sessao-90m.md` detalhando o roteiro da sessão de diagnóstico em profundidade, como usar os insumos das coletas e o que extrair/gravar do CEO.
2.  **Elo 4 - Coleta de Dados Profunda:** Definir os dados operacionais, financeiros e de clientes exigidos pós-venda.
3.  **Decidir as 6 peças em aberto do D1:** (a) quem produz o relatório-isca; (b) o que é vendido na call; (c) upsell para D2 ou D3; (d) conteúdo do formulário 1; (e) conteúdo do formulário 2; (f) estrutura da reunião de 90 min (fixa/orgânica/híbrida).
4.  **Elo 1 a 3 (Pré-Degrau):** Detalhar a reunião de vendas de 1h, a Isca e os conteúdos de atração.
5.  **Preencher célula D1 × C1 da matriz** com base no D1 fechado.
6.  **Só depois:** shortlist de skills/agentes dos 10 forks selecionados (decisão adiada até D1 fechar).

## 5. Governança e Regras Críticas (Cross-LLM)
*   **Sincronia Inegociável:** Qualquer alteração no framework do Motor deve ser atualizada simultaneamente em `knowledge/motor-lct/matriz.md` e `knowledge/motor-lct/matriz.json`. Eles são espelhos.
*   **Uso de Ferramentas:** Respeitar as diretrizes de governança listadas em `knowledge/motor-lct/governance.md` e os princípios em `constitution.md`.
*   **Atualização Contínua:** Sempre que uma sessão fechar um ciclo importante de desenvolvimento, o agente responsável DEVE atualizar a seção 3 deste arquivo (`Estado Atual`).
