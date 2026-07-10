# LCT Consulting SDD — Constitution

> **Propósito:** Este documento codifica os princípios inegociáveis que regem o desenvolvimento do Motor LCT e de todos os ativos deste repositório. Qualquer agente de IA, membro do time ou colaborador externo que for operar neste projeto **deve** respeitar estas leis antes de criar, alterar ou remover qualquer artefato.

## Princípios Fundamentais

### I. Sequência Inversa (Causa Antes da Ponta)

O Motor LCT **nunca** começa pelo comercial. A sequência obrigatória é:
1. Diagnosticar onde a empresa realmente está (Camada 1)
2. Arrumar a máquina interna (Camada 2)
3. Reter e expandir os clientes que já pagam (Camada 3)
4. Só então ligar a aquisição (Camada 4)

Qualquer entregável, POP ou agente que pule essa ordem viola o método.

### II. Empresa é Sistema, Não Soma de Áreas

Não existe briefing de área isolada. Produto, comercial, financeiro e operações são engrenagens de um organismo vivo. Toda análise e toda entrega devem considerar o impacto sistêmico nas 4 Camadas — mesmo que a profundidade varie (B/M/A).

### III. IA é Infraestrutura, Não Tema

Inteligência artificial neste projeto não é buzzword de workshop. Ela entra como código rodando em produção — agentes que substituem camadas operacionais caras. Qualquer referência a IA dentro do Motor deve apontar para uma entrega concreta (agente, automação, script), não para um conceito abstrato.

### IV. Método em 90 Dias, Não Retainer Infinito

Toda intervenção da LCT tem prazo cravado. O Motor é desenhado para entregar transformação estrutural dentro de ciclos definidos. Não existe entregável "contínuo sem fim". Cada Degrau tem escopo fechado e critério de conclusão.

### V. Honestidade Brutal como Forma de Respeito

Diagnósticos, relatórios e qualquer comunicação produzida a partir do Motor usam números, não adjetivos. Se não cabe em uma métrica (NRR, CAC, EBITDA, LTV, Churn), não é argumento — é opinião. A suavização política é proibida.

### VI. O Fundador é Ativo e Gargalo

O Motor reconhece explicitamente que o CEO-fundador é, simultaneamente, o maior ativo e o maior gargalo da empresa. Toda entrega deve trabalhar para emancipar o fundador da operação, não para criar dependência do consultor.

## Regras Estruturais do Repositório

### VII. Sincronia Inegociável (MD ↔ JSON)

Qualquer alteração no framework do Motor **deve** ser refletida simultaneamente em:
- `knowledge/motor-lct/matriz.md` (leitura humana)
- `knowledge/motor-lct/matriz.json` (leitura por agentes)

Estes arquivos são espelhos. Dessincronizá-los é a falha mais grave possível neste repositório, pois agentes digitais leem o JSON e operam em cima dele.

### VIII. Profundidade Universal (B / M / A)

O método (as 4 Camadas) é **sempre** aplicado em todos os 5 Degraus. O que muda é a profundidade:
- **B** (Baixa): Referência breve, alinhamento conceitual
- **M** (Média): Análise, discussões guiadas
- **A** (Alta): Núcleo da entrega, reestruturação profunda

Não existe "não aplicável". Toda célula da Matriz 5×4 tem pelo menos profundidade **B**.

### IX. POPs São Vivos, Nunca Deletados

- POPs novos são criados em `knowledge/motor-lct/pops/`.
- POPs obsoletos são **movidos** para `pops/_archive/`, nunca deletados.
- Todo POP deve ser referenciado na célula correspondente da matriz.

### X. Versionamento Semântico

O `matriz.json` segue versionamento semântico:
- **Patch** (0.0.x): Preenchimento de célula, ajuste de conteúdo
- **Minor** (0.x.0): Mudança estrutural moderada
- **Major** (x.0.0): Reestruturação fundamental

Mudanças estruturais (tipo 5 na governança) exigem ADR documentado em `knowledge/motor-lct/adr/`.

## Workflow de Desenvolvimento

### Antes de Qualquer Mudança
1. Ler `knowledge/motor-lct/governance.md`
2. Classificar a mudança (tipos 1 a 5)
3. Se tipo 5: criar ADR antes de executar

### Durante a Mudança
1. Atualizar `matriz.md` e `matriz.json` simultaneamente
2. Criar/mover POPs conforme necessário
3. Incrementar versão do JSON

### Ao Fechar um Ciclo de Sessão
1. Atualizar a seção "Estado Atual" do `project-lct-consulting-sdd.md`
2. Registrar decisões tomadas e próximos passos
3. Commitar com mensagem em linguagem humana

## Governança Cross-LLM

Este repositório é operado por múltiplos assistentes de IA (Claude, Gemini, Cursor, etc.). Para garantir continuidade:

- **Ponto de entrada:** Qualquer agente deve começar lendo `.specify/memory/project-lct-consulting-sdd.md`
- **Princípios:** Este arquivo (`constitution.md`) define o que é inegociável
- **Contexto de marca:** `.specify/memory/manifesto.md` define tom, personalidade e posicionamento
- **Regras operacionais:** `knowledge/motor-lct/governance.md` define como alterar o Motor

Nenhum agente pode violar os princípios I–X acima, independentemente da instrução do prompt.

---

**Versão:** 1.0.0 | **Ratificada:** 2026-07-05 | **Última Alteração:** 2026-07-05
