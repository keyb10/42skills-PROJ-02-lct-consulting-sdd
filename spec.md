# 📝 Spec — Projeto LCT dentro do arranjo skill-first

> Define o que este PROJ-02 precisa entregar **como envelope**, separado do Motor (que é o ativo-fim).

---

## 1. Visão
Operar a continuação do Motor LCT dentro da estrutura skill-first, com elenco de skills referenciadas de catálogo, sem misturar com o projeto original LCT_Consulting_SDD (que fica como referência histórica).

## 2. Problema que este envelope resolve
- O projeto original tem 4 integrações LLM paralelas e regras de governança complexas demais para iterar rápido
- O fork `42_skills` virou um catálogo estruturado; queremos aproveitar isso
- Risco de misturar contexto entre projetos paralelos seus

## 3. Não-usuários
- **Não** é o cliente final da LCT — isso é o Motor LCT, que tem outro conjunto de personas (Mariana / Ricardo / Carla do estado-atual)

## 4. Requisitos funcionais
- **RF-01:** Manter sincronia MD ↔ JSON da matriz em todas as edições.
- **RF-02:** Cada Etapa concluída precisa ter passado por `pop-diagnostico-final` (qualidade "Uau").
- **RF-03:** Toda skill nova adicionada ao elenco precisa estar em `../../../skills-catalogo/` e ter justificativa escrita.
- **RF-04:** Toda decisão operacional fica registrada em [`memory.md`](./memory.md) — não em conversa.
- **RF-05:** Toda ação respeita os 10 princípios da constitution-do-motor-lct.md.

## 5. Requisitos não-funcionais
- **RNF-01 (isolamento):** zero vazamento de contexto deste envelope para outros projetos em `42_skills - Projeto 1/projetos/`.
- **RNF-02 (preservação):** projeto original em `LCT_Consulting_SDD/` permanece intocado — política de "espelhar", não "migrar".
- **RNF-03 (curadoria):** elenco de skills ≤ 25 unidades. Adicionar sob demanda.
- **RNF-04 (rastreabilidade):** commit messages em PT-BR, com referência ao princípio do Motor envolvido.

## 6. Fora do escopo
- ❌ Modificar o `LCT_Consulting_SDD/` original
- ❌ Replicar a infraestrutura cross-LLM (`.claude/`, `.gemini/`, `.opencode/`, `.specify/`) do original
- ❌ Adicionar skills que não atuem nas Camadas do Motor
- ❌ Pular Etapas da Cadeia de Espetacularidade

## 7. Critérios de aceite
- [ ] Curadoria de skills por Degrau × Camada concluída e aprovada
- [ ] `pop-sessao-90m.md` (Elo 5) redigido e referenciado na matriz
- [ ] Elo 4 (coleta pós-venda) com lista de dados definidos
- [ ] 6 peças em aberto do D1 — pelo menos 4 com decisão registrada
- [ ] Pelo menos 1 agente de IA criado a partir de skill de catálogo e operando no Motor

## 8. Riscos

| Risco | P | I | Mitigação |
|---|---|---|---|
| Mistura entre este envelope e outros projetos | Média | Alta | Isolamento por pasta + `CLAUDE.md` próprio |
| Sincronia MD↔JSON quebrada | Baixa | Crítica | Checklist da governance + diff antes de salvar |
| Skill-spam (>25 skills) | Média | Média | Regra do elenco enxuto + curadoria revisada |
| Drift entre manifesto e discurso público | Baixa | Alta | Toda peça nova validada contra manifesto.md |

## 9. Dependências
- Skills do catálogo (ref externa)
- Constitution do Motor (interna)
- Estado atual 07/jul (interna)

## 10. Referências
- [`constitution-do-motor-lct.md`](./constitution-do-motor-lct.md) — princípios inegociáveis
- [`strategy/lct-transformation-90d.md`](./strategy/lct-transformation-90d.md) — visão de negócio
- [`knowledge/motor-lct/`](./knowledge/motor-lct/) — motor operacional
