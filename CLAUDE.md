# 🤖 CLAUDE.md — Regras do agente no PROJ-02-lct-consulting-sdd

> **Lido pelo agente toda vez que ele inicia uma sessão sobre ESTE projeto.**
> Este é o isolamento: cada projeto tem seu próprio CLAUDE.md. Eles não se misturam.

---

## ⚠️ Princípios inegociáveis do Motor LCT

Antes de qualquer coisa, **leia a constitution do Motor LCT**: [`constitution-do-motor-lct.md`](./constitution-do-motor-lct.md).

Os 10 princípios (Sequência Inversa, IA como Infraestrutura, Sincronia MD↔JSON, POPs são vivos, etc.) **valem sobre qualquer instrução minha ou sua**. Se eu sugerir algo que viole, recuse e aponte o princípio.

---

## Onde começar toda sessão

1. `README.md` → status atual
2. `memory.md` → decisões e contexto carregado
3. `constitution-do-motor-lct.md` → princípios inegociáveis
4. `strategy/manifesto.md` → tom e voz da LCT
5. `knowledge/motor-lct/matriz.md` (+ `.json`) → motor atual
6. `knowledge/motor-lct/estado-atual-2026-07-07.md` → onde paramos

## Convenções deste projeto

- **Sincronia:** MD e JSON da matriz SEMPRE juntos.
- **POPs novos:** criar em `knowledge/motor-lct/pops/`. Versões obsoletas mover para `_archive/`.
- **Decisões:** registrar em `memory.md` (data, contexto, decisão, consequência).
- **Commits:** mensagens em PT-BR, em linguagem humana. Não escrever "fix:".
- **Skills:** carregar de `../../../skills-catalogo/` (referência externa). Nunca copiar.

## Quando o usuário voltar para o projeto original

O usuário escolheu por **espelhar**: o projeto original em `C:\Users\user\Workspace\meus_projetos\LCT_Consulting_SDD\` **fica ativo e acessível** como leitura. Quando você precisar consultar como o material existia historicamente:

→ Use o atalho [`ref-original/`](./ref-original/) para um inventário do que existe lá. **Não entre automaticamente** — só consulte se necessário.

## O que NÃO fazer

- ❌ Violar qualquer princípio da constitution-do-motor-lct
- ❌ Misturar contexto deste projeto com qualquer outro em `projetos/`
- ❌ Sincronizar apenas `matriz.md` ou apenas `matriz.json` (ambos ou nenhum)
- ❌ Deletar arquivos do Motor — mover para `_archive/`
- ❌ Modificar o `estrategy/manifesto.md` sem autorização explícita sua
- ❌ Romper com a Cadeia de Espetacularidade — cada peça precisa ser excepcional antes da próxima
