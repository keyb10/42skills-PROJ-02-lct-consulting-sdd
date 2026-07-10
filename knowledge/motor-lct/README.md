# Motor LCT

## O que é

O motor operacional da LCT Consulting. É a **matriz que cruza os 5 Degraus da Escada de Valor com as 4 Camadas do Método LCT** e diz, para cada combinação, **o que entregar, como, com quais agentes, e quando está pronto**.

É a peça que transforma a LCT de "consultoria artesanal" em "consultech" — onde cada entrega é previsível, versionada, replicável e delegável (inclusive a agentes de IA).

## Estado atual — 2026-07-10 (v0.0.8)

**Degrau 1 (Sessão Estratégica Executiva) está 100% estudado E produzido.**

- **6 POPs prontos** em [`pops/`](./pops/) — prontos para entrar em operação com clientes
- **4 estudos publicados** em [`estudos/`](./estudos/) (D1×C1, C2, C3, C4)
- **20 células estudadas** no Motor inteiro (D1-D5 × C1-C4)
- **20 marcadores [adotado:] / [rejeitado:] aplicados** no The Revenue Codex original (ver [`governance.md`](./governance.md) §3)
- **2 skills no fork `meus_forks/42_skills/`** instaladas: `brand-lct`, `ceo-interview`

Próxima camada do Motor: **produção do D2** (10 POPs — Mentoria CEO).

## Estrutura

```
motor-lct/
├── README.md               ← este arquivo
├── matriz.md               ← tabela 5 Degraus × 4 Camadas (markdown, humano-legível)
├── matriz.json             ← espelho JSON para agentes (sincronizado MD↔JSON)
├── governance.md           ← regras de manutenção
├── estado-atual-YYYY-MM-DD.md  ← snapshots datados do estado vigente
├── pops/                   ← POPs por célula (1 arquivo por POP)
│   ├── pop-diagnostico-ceo-90m.md            (D1×C1, v1.0.0)
│   ├── pop-auditoria-maquina-cliente.md      (D1×C2, v1.0.0)
│   ├── pop-pulse-clientes-atuais.md          (D1×C3, v1.0.0)
│   ├── pop-5-angulos-posicionamento-cliente.md (D1×C4, v1.0.0)
│   ├── template-raio-x.md                    (reativado v2.0.0)
│   ├── pop-diagnostico-final.md              (reativado v2.0.0)
│   ├── README.md                             (índice)
│   └── _archive/lo6-2026-07-09/              (NOTA + README — Regra IX, sem delete)
├── estudos/                ← 20 estudos publicados
│   ├── celula-D1-C1.md ... celula-D1-C4.md
│   ├── celula-D2-C1.md ... celula-D2-C4.md
│   ├── celula-D3-C1.md ... celula-D3-C4.md
│   ├── celula-D4-C1.md ... celula-D4-C4.md
│   └── celula-D5-C1.md ... celula-D5-C4.md
├── cruzamento-motor-x-codex.md   ← tabela 5×4 × Cap. The Revenue Codex
├── d1-por-camada.md             ← planejamento macro do D1
└── _archive/                    ← versões obsoletas (governance snapshot)
```

## Origem

Construído a partir de três fontes fundacionais que moram no projeto:

- **Estratégia** — [`../../strategy/lct-transformation-90d.md`](../../strategy/lct-transformation-90d.md) (Relatório de Inteligência Estratégica LUZ HUB, abril 2026). Define os 5 Degraus da Escada de Valor e a sequência inversa das 4 Camadas.
- **Voz** — [`../../strategy/manifesto.md`](../../strategy/manifesto.md). Define tom, identidade e sistema de crenças que toda entrega deve respeitar.
- **Práticas de mercado** — [`../../../LCT_Consulting_SDD/knowledge/external/revenue-codex/`](../../../LCT_Consulting_SDD/knowledge/external/revenue-codex/) (compêndio The Revenue Codex — 34 capítulos + frontmatter). Insumo referencial com marcadores `[adotado:]` / `[rejeitado:]` aplicados.

## Como agentes leem o motor

1. Carregam [`matriz.json`](./matriz.json) — visão compacta da estrutura.
2. Carregam a(s) **célula(s) específica(s) do escopo do agente** (ex.: um agente de qualificação lê `[degrau-2][camada-4]`).
3. Quando uma célula referencia um POP, carregam só o arquivo `pops/<nome>.md` necessário.
4. Carregam o estudo correspondente em `estudos/celula-Dx-Cy.md` para contexto metodológico profundo.
5. Carregam [`../../strategy/manifesto.md`](../../strategy/manifesto.md) para tom de voz (validado pela skill `brand-lct` instalada no fork).

Agentes **não** precisam ler o motor inteiro. A indexação em JSON permite carregar só o que cabe no escopo funcional.

## Skills que sustentam o motor (instaladas em `meus_forks/42_skills/`)

| Skill | Path | Função no Motor |
|---|---|---|
| `brand-lct` | `Marketing/brand-lct/SKILL.md` | Voz LCT em qualquer peça (10 regras) |
| `ceo-interview` | `Knowledge-Work-Plugins/design/skills/ceo-interview/` | Protocolo 5 perguntas-chave (Cap. 07) |
| `motor-governance` | `superpowers/skills/motor-governance/` | Validação 6 checks para mudanças no Motor |
| `writing-skills` (superpowers) | `superpowers/skills/writing-skills/` | Meta-guia do TDD de Skills (criou as 3 acima) |

## Princípios

- **Profundidade variável por célula.** Não é matriz simétrica — alguns Degraus aprofundam mais uma Camada que outra. A profundidade vive na `matriz.md`.
- **Prática de cliente pode virar motor.** Quando um cliente traz uma prática que não está no compêndio, ela pode ser internalizada aqui (ver `governance.md`).
- **Prática obsoleta pode sair.** Versões antigas do motor podem ser aposentadas — nada aqui é eterno, tudo é vivo.
- **Tudo é vivo.** Este motor vai nascer com estrutura e vai evoluir. As regras de evolução estão em [`governance.md`](./governance.md).

## Histórico de versões

| Versão | Data | Mudança |
|---|---|---|
| 0.0.3 | (origem) | Estado recebido do projeto LCT_Consulting_SDD original |
| 0.0.4 | 2026-07-09 | VIRADA DE CHAVE: D1 resetado, POPs do Elo 6 arquivados |
| 0.0.5 | 2026-07-09 | Enriquecimento estratégico LUZ HUB (Eixo Y completo) |
| 0.0.6 | 2026-07-09 | D1 inteiro estudado (4/4 células) |
| 0.0.7 | 2026-07-09 | D1-D5 inteiro estudado (20/20 células) |
| **0.0.8** | **2026-07-10** | **D1 PRODUZIDO — 6 POPs prontos, 20 marcadores no The Revenue Codex original, commit & push no GitHub** |
