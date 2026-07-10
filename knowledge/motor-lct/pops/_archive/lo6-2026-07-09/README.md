# POPs — Procedimentos Operacionais Padrão

Esta pasta está vazia. Os POPs serão criados sob demanda, à medida que as células da [`matriz.md`](../matriz.md) forem preenchidas.

**Convenção de nomenclatura:** kebab-case, verbo-nome quando aplicável (ex.: `coleta-indicadores-financeiros.md`, `onboarding-cliente.md`, `qualificacao-leads-bant-turbo.md`).

**Estrutura de cada POP** (sugestão, não obrigatória):

```markdown
# POP: <nome>

## O que é
<descrição em uma frase>

## Quando usar
<gatilhos que disparam este POP>

## Pré-requisitos
<o que precisa estar pronto antes de rodar>

## Passo a passo
1. ...
2. ...
3. ...

## Insumos
- ...

## Saídas
- ...

## Critério de pronto
- ...

## Agentes digitais envolvidos
- (referência a `agents/<nome>/`)

## Notas / pegadinhas
- ...
```

Quando um POP for deprecado, **não deletar** — mover para `pops/_archive/<nome>.md` (ver [`governance.md`](../governance.md), tipo 4).
