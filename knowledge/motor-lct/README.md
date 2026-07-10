# Motor LCT

## O que é

O motor operacional da LCT Consulting. É a **matriz que cruza os 5 Degraus da Escada de Valor com as 4 Camadas do Método LCT** e diz, para cada combinação, **o que entregar, como, com quais agentes, e quando está pronto**.

É a peça que transforma a LCT de "consultoria artesanal" em "consultech" — onde cada entrega é previsível, versionada, replicável e delegável (inclusive a agentes de IA).

## Origem

Construído a partir de três fontes fundacionais que moram no projeto:

- **Estratégia** — [`strategy/lct-transformation-90d.md`](../../strategy/lct-transformation-90d.md) (Relatório de Inteligência Estratégica, abril 2026). Define os 5 Degraus da Escada de Valor e a sequência inversa das 4 Camadas.
- **Voz** — [`.specify/memory/manifesto.md`](../../.specify/memory/manifesto.md). Define tom, identidade e sistema de crenças que toda entrega deve respeitar.
- **Práticas de mercado** — [`knowledge/external/revenue-codex/`](../../knowledge/external/revenue-codex/) (compêndio de organização consolidada de práticas de mercado). Insumo referencial para porções do motor.

## Estrutura

```
motor-lct/
├── README.md          ← este arquivo (visão geral + como usar)
├── matriz.md          ← tabela 5 Degraus × 4 Camadas (markdown, legível por humanos)
├── matriz.json        ← mesma matriz em JSON (carregável por agentes sem ler markdown)
├── governance.md      ← regras de evolução, contribuição de práticas, depreciação
└── pops/              ← procedimentos operacionais padrão (um arquivo por POP)
    └── (a popular)
```

Expansão sob demanda: pastas dedicadas por Degrau (`degraus/degrau-X/`) só aparecem quando o conteúdo de uma combinação específica merece um arquivo próprio.

## Como agentes leem o motor

1. Carregam [`matriz.json`](./matriz.json) — visão compacta da estrutura.
2. Carregam a(s) **célula(s) específica(s) do escopo do agente** (ex.: um agente de qualificação lê a célula `[degrau-1][camada-3]`).
3. Quando uma célula referencia um POP, carregam só o arquivo `pops/<nome>.md` necessário.
4. Carregam [`.specify/memory/manifesto.md`](../../.specify/memory/manifesto.md) para tom de voz.

Agentes **não** precisam ler o motor inteiro. A indexação em JSON permite carregar só o que cabe no escopo funcional.

## Princípios

- **Profundidade variável por célula.** Não é matriz simétrica — alguns Degraus aprofundam mais uma Camada que outra. A profundidade vive na `matriz.md`.
- **Prática de cliente pode virar motor.** Quando um cliente traz uma prática que não está no compêndio, ela pode ser internalizada aqui (ver `governance.md`).
- **Prática obsoleta pode sair.** Versões antigas do motor podem ser aposentadas — nada aqui é eterno, tudo é vivo.
- **Tudo é vivo.** Este motor vai nascer com estrutura e vai evoluir. As regras de evolução estão em [`governance.md`](./governance.md).
