# 🗂️ ref-original — Atalho de leitura para o projeto original

> Por convenção, **não modifique nada** no diretório original. Use este atalho quando precisar consultar como o material existia historicamente.

---

## 📍 Caminho original

```
C:\Users\user\Workspace\meus_projetos\LCT_Consulting_SDD\
```

## 📦 Inventário do que existe lá

### Estratégia
- `strategy/lct-transformation-90d.md` — Relatório de Inteligência Estratégica (abril/2026). Diagnóstico + plano 90 dias.
- *(Migrado para dentro deste envelope em `../strategy/`)*

### Knowledge — Motor LCT
- `knowledge/motor-lct/README.md` — Visão geral do Motor
- `knowledge/motor-lct/matriz.md` — Matriz 5 Degraus × 4 Camadas (v0.0.3)
- `knowledge/motor-lct/matriz.json` — Espelho JSON
- `knowledge/motor-lct/governance.md` — Regras de manutenção
- `knowledge/motor-lct/estado-atual-2026-07-07.md` — Snapshot vigente
- `knowledge/motor-lct/_archive/estado-atual-2026-06-21.md` — Snapshot anterior
- `knowledge/motor-lct/pops/template-raio-x.md` — POP pronto
- `knowledge/motor-lct/pops/pop-diagnostico-final.md` — POP pronto
- `knowledge/motor-lct/pops/README.md` — Índice
- *(Tudo migrado para `../knowledge/motor-lct/`)*

### Knowledge — Compêndio externo
- `knowledge/external/revenue-codex/` — Compêndio de práticas de mercado (34 capítulos + front matter + README + índice). **NÃO migrado**, fica só como referência acessível via filesystem.

### Especificações / integrações cross-LLM (NÃO MIGRADAS)
- `.claude/skills/speckit-*/` — Skills do spec-kit instaladas no Claude
- `.claude/settings.local.json`
- `.gemini/commands/speckit-*.toml` — Comandos para Gemini
- `.opencode/commands/speckit-*.md` — Comandos para Opencode
- `.specify/templates/` — Templates do spec-kit
- `.specify/scripts/` — Scripts utilitários
- `.specify/workflows/` — Workflows
- `.specify/extensions/`, `.specify/integrations/`
- `.specify/memory/constitution.md` — *(migrado)*
- `.specify/memory/manifesto.md` — *(migrado)*
- `.specify/memory/project-lct-consulting-sdd.md` — *(migrado para `../strategy/memoria-central-original.md`)*
- `.specify/init-options.json`, `.specify/extensions.yml`, `.specify/integration.json`

### Git
- `.git/` — Repositório git do original (3 commits). **Não mexa.**

### Top level
- `CLAUDE.md`, `AGENTS.md`, `GEMINI.md` — Marcadores com `<!-- SPECKIT START -->` (placeholders simples)

---

## 🚦 Política de uso

| Operação | Permitido? |
|---|---|
| Ler arquivos do original | ✅ Sempre |
| Usar como referência pra consulta | ✅ Sempre |
| Editar/modificar arquivos do original | ❌ Nunca — projeto congelado nesta data |
| Re-executar comandos cross-LLM | ❌ Não pelo Claude; cada LLM opera do seu lado |
| Adicionar/remover commits no `.git/` do original | ❌ Não |
| Mover/renomear coisas no original | ❌ Não |
