# Governance — Motor LCT

> Regras de manutenção do motor. **Ler antes de adicionar/alterar/remover qualquer coisa em `motor-lct/`.**

## Princípio-raiz

O motor é **vivo**. Nasceu com estrutura mínima (`matriz.md` + `matriz.json` nomeando Degraus, Camadas e a tabela 5×4 com células vazias) e vai ganhar profundidade à medida que a LCT opera clientes reais. **Nada aqui é eterno.** Mas toda mudança precisa seguir as regras abaixo pra não quebrar o que depende do motor (agentes digitais, novos membros do time, novos clientes).

## Tipos de mudança

### 1. Preencher uma célula (mudança mais comum)

- Uma célula da matriz vai de profundidade `.` para `B`, `M`, ou `A`.
- **Quem decide:** o founder (Leandro), sozinho ou em conversa com quem estiver rodando o Degrau correspondente.
- **Como:**
  1. Atualizar `matriz.md` (substituir `·` pelo nível e descrever entregável/POPs/agentes/insumos/critério).
  2. Atualizar `matriz.json` na mesma entrada de `celulas` (manter os dois sincronizados).
  3. Se nascer um POP novo, criar `pops/<nome-descritivo>.md` e referenciar.
  4. Se nascer um agente novo, criar pasta `agents/<nome>/` e referenciar.
- **Versionamento:** incrementar a versão patch de `matriz.json` (0.0.1 → 0.0.2).

### 2. Adicionar prática de cliente (internalização)

Quando um cliente traz uma prática de mercado que não está no compêndio de referência e que vale ser motor (reutilizável), este é o caminho:

1. Documentar a prática primeiro onde ela foi vista — em material de cliente, com link reverso.
2. Avaliar se é **genérica** (vale pra qualquer cliente do ICP) ou **específica** (só serve pro contexto daquele cliente).
   - **Específica:** não entra no motor. Pode virar nota em `pops/` se for detalhe operacional.
   - **Genérica:** entra no motor.
3. Para prática genérica:
   - Adicionar como nova entrada em um POP existente, OU criar POP novo em `pops/`.
   - Marcar a célula correspondente com a profundidade ajustada se for o caso.
   - Adicionar nota no `matriz.md` da célula: "prática internalizada de <cliente> em <data>".
4. Sincronizar `matriz.json`.

### 3. Adotar prática do compêndio de mercado

Quando uma prática do compêndio [`knowledge/external/revenue-codex/`](../../knowledge/external/revenue-codex/) é adotada formalmente no motor:

1. Identificar a célula e o POP onde a prática se encaixa.
2. Atualizar `matriz.md` e `matriz.json` (procedimento padrão de "preencher célula").
3. No capítulo do compêndio correspondente, adicionar marcador `[adotado em <data> → motor-lct/célula-X-Y / pops/Z]`.
4. O marcador `[adotado: ...]` é a única anotação permitida no compêndio — ele liga o compêndio ao motor sem reescrever o material de referência.

### 4. Aposentar prática (depreciação)

Quando uma prática do motor se torna obsoleta:

1. **Não deletar.** Mover o conteúdo para `pops/_archive/<nome>.md` (criar pasta se não existir) com nota de depreciação.
2. Atualizar `matriz.md` indicando a depreciação na célula correspondente.
3. Atualizar `matriz.json` mudando `pops` da célula (retirar referência, mover nome para `pops_arquivados`).
4. **Nunca** deletar a versão antiga do POP — pode ser que ela volte a ser útil ou que um cliente novo tenha o mesmo contexto.

### 5. Mudança estrutural (arquitetura)

Este é o tipo de mudança que **não** se faz no dia a dia. Exemplos:

- Renomear um Degrau (ex.: "Sessão Estratégica" virar "Diagnóstico Relâmpago").
- Dividir uma Camada em duas (ex.: Camada 2 virar 2A — pessoas, 2B — tecnologia).
- Criar uma terceira dimensão da matriz.
- Mover o motor para outra pasta.

**Regra:** mudança estrutural exige:

1. Justificativa explícita (por que a estrutura atual não serve mais).
2. Avaliação de impacto em todos os agentes que leem o motor (todos vão precisar atualizar o que carregam).
3. Avaliação de impacto em todos os clientes em andamento.
4. Decisão documentada em ADR (Architecture Decision Record) — criar `knowledge/motor-lct/adr/0001-<titulo>.md`.

Versionamento de mudança estrutural: **minor** (0.1.0) ou **major** (1.0.0) em `matriz.json`.

## Sincronização obrigatória

Estes pares **precisam** ser mantidos em sincronia:

| Origem | Espelho | Risco se dessincronizar |
|--------|---------|------------------------|
| `matriz.md` | `matriz.json` | Agentes leem JSON e operam em dado errado |
| Células da matriz | POPs em `pops/` | POP fica órfão ou célula referencia POP inexistente |
| Células da matriz | Agentes em `agents/` | Agente entra em célula que mudou e gera entrega errada |
| Compêndio de mercado | Marcador `[adotado: ...]` | Compêndio vira lixo desatualizado |

## Checklist antes de commitar mudança no motor

- [ ] Li este `governance.md`?
- [ ] A mudança é de tipo 1, 2, 3, 4 ou 5?
- [ ] Se tipo 5: ADR criado e impacto avaliado?
- [ ] `matriz.md` e `matriz.json` foram ambos atualizados?
- [ ] Versão de `matriz.json` foi incrementada (patch / minor / major conforme tipo)?
- [ ] POPs novos foram criados em `pops/`? Antigos foram movidos para `_archive/` em vez de deletados?
- [ ] Agentes referenciados existem ou estão planejados em `agents/<nome>/`?
- [ ] Se prática do compêndio foi adotada, o marcador `[adotado: ...]` está no capítulo correspondente?
- [ ] Mensagem de commit descreve a mudança em linguagem humana (não técnica)?

## Quando rever este governance

Este documento também é vivo. Quando uma regra mostrar ser:

- **Ineficaz** (alguém seguindo à risca não consegue operar) → simplificar ou reescrever.
- **Incompleta** (surgiu um tipo de mudança que não se encaixa em 1-5) → adicionar tipo.
- **Ossificada** (segurando mudanças que a LCT precisa fazer) → desafiar o próprio documento.

Mudanças neste `governance.md` são tipo 5 (mudança estrutural) — exigem ADR.
