# 🗺️ Plan — Plano de Execução do PROJ-02

> **Atenção:** Este plano é do **envelope skill-first**, não do Motor LCT original.
> As Etapas do Motor seguem o que está em `knowledge/motor-lct/`.
> Aqui organizamos como vamos atacá-las com skills do catálogo.

---

## 1. Stack / abordagem

- **Skills:** referenciadas de `../../../skills-catalogo/` (read-only).
- **Memória:** [`memory.md`](./memory.md) (envelope) + estado-atual do Motor (interior).
- **Catálogo-curadoria:** [`skills-curadoria/`](./skills-curadoria/) — onde a matriz skills-por-Degrau vai morar.

## 2. Fases de execução (dentro deste envelope)

### Sprint 1 — Curadoria de skills (PRÓXIMO ALVO)

- **Saída:** [`skills-curadoria/matriz-skills-por-degrau.md`](./skills-curadoria/matriz-skills-por-degrau.md) refinada — uma matriz que cruza as 4 Camadas × 5 Degraus com skills **realmente existentes** no catálogo (validar com `Glob`).
- **Skills envolvidas:** nenhuma skill precisa ser executada; é trabalho analítico (leitura + agrupamento + justificativa).
- **Critério de saída:** você aprova o elenco; nenhum Degrau fica sem skill(s) candidatas para suas células-alvo.

### Sprint 2 — Elo 5 (pop-sessao-90m.md) — só se Sprint 1 estabilizar

- **Saída:** `knowledge/motor-lct/pops/pop-sessao-90m.md` (redigido e referenciado na matriz).
- **Skills envolvidas:** `marketing-ideas` (para roteiro inspirado em práticas), `marketing-psychology` (para extração do CEO), `review-contract` (compliance da call gravada).
- **Critério de saída:** POP pronto, com qualidade "Uau" (Cadeia de Espetacularidade).

### Sprint 3 — Elo 4 (coleta pós-venda) — segue Sprint 2

- **Saída:** lista de dados financeiros / operacionais / comerciais exigidos do cliente pós-venda.
- **Skills envolvidas:** `financial-statements`, `audit-support`, `customer-pulse`.
- **Critério de saída:** checklist validável, pronto pra entrar como input do `pop-sessao-90m`.

### Sprint 4 — 6 peças em aberto do D1

- **Saída:** decisões registradas em [`memory.md`](./memory.md).
- **Skills envolvidas:** `marketing-ideas` (ângulos da isca), `pricing` (modelos de upsell), `lead-magnets` (formato).
- **Critério de saída:** ≥ 4 das 6 peças decididas.

### Sprint 5 — Criação de 1 agente de IA do Motor (Camada 2 — IA como Infra)

- **Saída:** 1 agente de catálogo adaptada (ex.: agente que produz o relatório-isca) rodando.
- **Skills envolvidas:** `mcp-builder`, `skill-creator`, `frontend-design`.
- **Critério de saída:** agente está em `agents/<nome>/` (a ser criado) e referenciado na célula da matriz.

## 3. Workflow visual

```
[Sprint 1: curadoria] → [Sprint 2: Elo 5] → [Sprint 3: Elo 4] → [Sprint 4: 6 peças] → [Sprint 5: agente]
        ↓                   ↓                  ↓                   ↓                       ↓
skills-curadoria/    pops/pop-sessao-   skill sugerida      memory.md +              agents/<name>/
                     90m.md             em plan.md          outputs/drafts/
```

## 4. Riscos do plano
| Risco | Plano B |
|---|---|
| Curadoria vira brainstorm infinito | Regra: cada skill candidata precisa de justificativa em 1 frase |
| POP Elo 5 nascer sem qualidade "Uau" | Aplicar `pop-diagnostico-final` como peer review |
| Skill não encontrada no catálogo | Criar via `skill-creator` ou marcar como gap explícito |

## 5. Critérios de "pronto"
- [ ] 5 sprints entregues
- [ ] matriz-skills atualizada
- [ ] 1 agente rodando em produção
- [ ] Memória consolidada e versionada
- [ ] Você aprova todas as Etapas antes de avançar
