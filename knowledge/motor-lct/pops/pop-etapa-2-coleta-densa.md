---
name: pop-etapa-2-coleta-densa
description: Etapa 2 do D1 — Coleta Densa remota (formulário + repositório) para construir os dados que entram na Reunião 2 (Etapa 3, 90 min "vamos fundo")
version: 1.0.0
applies_to: [LCT Consulting / Degrau 1 / Etapa 2 - Entre Reuniões 1 e 2]
related_skills:
  - brand-lct                ← voz LCT no email/formulário
  - ceo-interview            ← as 5 perguntas-chave se ampliam aqui
  - data-ingester            ← (skill futura) normaliza arquivos do cliente
caps_referenced:
  - Cap. 02 (Impacto dos Gargalos) — para auditar processos
  - Cap. 06 (Fundamentos) — 4 fundamentos para validar
  - Cap. 07 (Re-check PMF) — 5 perguntas-chave ampliam
  - Cap. 31 (Churn/NRR) — dados quantitativos necessários
governance:
  - Cap. 24 (CRM Mínimo Viável) — base antes de qualquer dado
  - Cap. 10 (Roadmap RICE) — priorização do que entra
related_pops:
  - pop-etapa-1-reuniao-1h.md     (Etapa 1 — alimentou esta Etapa)
  - pop-etapa-3-reuniao-2-90m.md (próxima Etapa — consome estes dados)
related_studies:
  - estudos/celula-D1-C1.md
  - estudos/celula-D1-C2.md
---

# pop-etapa-2-coleta-densa

## 1. Visão geral

Este POP é a **Etapa 2** da jornada D1. Após o aceite + pagamento do D1, o lead vira **cliente** e entra em **Coleta Densa** — o que **alimenta a Reunião 2 (90 min "vamos fundo", Etapa 3) com dados na mão**.

> **Por que essa etapa é crucial:** sem dados, a Reunião 2 vira "consultoria genérica". Com dados, a Reunião 2 vira **cirurgia** com **achados verificáveis**.

**Quem aplica:** LCT (Arquiteto de Crescimento) — dispara email + formulário
**Quem preenche:** o **cliente** (agora pagante)
**Saída:** Pasta/diretório com **5-10 entregáveis densos** que entram na Reunião 2

---

## 2. Workflow operacional

### 2.1 Email disparado em até 2h após confirmação de pagamento

Aplicar `brand-lct`. Componentes:

- **Assunto:** "Próximo passo: Reunião Estratégica — preciso de alguns documentos"
- **Corpo:** 2-3 parágrafos curtos:
  - "Parabéns pelo aceite. Para a nossa sessão de 90 min funcionar bem, preciso de alguns documentos."
  - "Abaixo, formulário + link para repositório. **Prazo sugerido: 5 dias úteis.**"
  - "Se travar em algum, me avise — a gente antecipa a reunião ou pula o ponto."
- **Anexos:** 2 links
  - Link 1: Formulário (Tally/Typeform/Notion Form)
  - Link 2: Repositório (GitHub private / S3 / dropbox-style)

### 2.2 Formulário (7-12 perguntas, online)

| # | Pergunta | Por que está aqui |
|---|---|---|
| 1 | "Anexe a DRE dos últimos 12 meses" (PDF/Excel) | Base de C1 |
| 2 | "Anexe o funil de vendas dos últimos 6 meses" (CRM export) | Base de C4 |
| 3 | "Qual a taxa de churn mensal dos últimos 6 meses?" | Base de C3 |
| 4 | "Liste os 10 maiores clientes em valor e o status de cada (ativo/fantasma/cancelou)" | Base de C3 (Matriz Valor×Fit) |
| 5 | "Tem dashboard de North-Star atual? Anexe se sim." | Base de C1 |
| 6 | "Quantas pessoas no time? Distribua por cargo/função." | Base de C2 |
| 7 | "Liste os 3 principais processos manuais que ocupam mais tempo" | Base de C2 (RICE) |
| 8 | "Existe documentação de runbook/SOP? Anexe os principais" | Base de C2 |
| 9 | "Tem CRM? Qual? Quem atualiza?" | Base de C2 (CRM Mínimo) |
| 10 | "Existe playbook de atendimento/CS? Anexe" | Base de C3 |
| 11 | "Já teve tentativas de consultoria anteriores? Quais? Resultados?" | Diagnóstico de padrão |
| 12 | "Há 3 anos, o que mudou no seu mercado?" | Pergunta-chave P5 do Cap. 07 |

> **Dica:** todas as perguntas são **multi-formato** (texto + anexo) — porque algumas precisam de número, outras de contexto.

### 2.3 Repositório (acesso para arquivos grandes)

**Opções de implementação:**
- **GitHub private** (se cliente for tech-savvy) — `cliente-lct-{empresa}/` com README estruturado
- **S3 / dropbox-style** (se cliente não-técnico) — link de upload único
- **Drive compartilhado** (Google Drive / OneDrive) — última opção, menos seguro

**Estrutura sugerida do repositório:**
```
cliente-lct-{empresa}/
├── README.md                 ← índice do que foi upado
├── 01-dre/
├── 02-funil-vendas/
├── 03-churn-metrics/
├── 04-clientes-top10/
├── 05-north-star/
├── 06-time/
├── 07-processos-manuais/
├── 08-runbooks/
├── 09-crm/
├── 10-cs-playbook/
├── 11-historico-consultoria/
└── 12-mercado-contexto/
```

### 2.4 Acompanhamento durante a Coleta (5 dias úteis)

- Email de check-in no **dia 2** ("alguma dúvida sobre o formulário?")
- Email de check-in no **dia 4** ("falta pouco — quer antecipar a reunião?")
- **Não cobrar agressivamente** — `brand-lct` (sem pressionar)

---

## 3. O que a LCT faz enquanto o cliente preenche

### 3.1 Pré-processamento (não-IA, humano)

Quando os documentos começam a chegar, **LCT (Leandro) lê** cada um — não dá pra delegar tudo a agente de IA aqui, porque o objetivo é **construir contexto antes da sessão**.

### 3.2 Rascunho de achados preliminares

LCT cria um **rascunho** em [`outputs/{cliente}/coleta-densa-rascunho.md`](../../outputs/) com:

- **3-5 hipóteses** sobre o teto do cliente
- **Lista de perguntas pendentes** (a fazer na Reunião 2)
- **Esboço do Raio-X** (preencher durante/após a Reunião 2)

> **Skill futura:** `data-ingester` (não existente) automatizaria parte desse pré-processamento. Por enquanto é humano.

---

## 4. Critério de qualidade "Uau"

- O cliente **completa o formulário em ≤ 5 dias úteis** (sem precisar cobrar)
- **Pelo menos 8 de 12 perguntas têm anexo ou resposta estruturada** (não texto vazio)
- **LCT consegue ler tudo em 1-2 horas** (preparação Reunião 2)
- **A Reunião 2 vira "cirurgia"** — 90 min com dados na mão, não com perguntas genéricas

---

## 5. Anti-patterns (não fazer)

- ❌ **Não fazer mais de 12 perguntas** — fadiga de formulário
- ❌ **Não aceitar texto vazio** — se for importante, **exija** (anexo ou número)
- ❌ **Não cobrar diariamente** — `brand-lct` (sem pressão)
- ❌ **Não prometer que a Reunião 2 vai ser genérica** — sempre cirúrgica
- ❌ **Não usar IA para resumir antes de ler** — leitura humana do LCT constrói contexto que agente não substitui

---

## 6. Cross-reference na matriz

- **D1×C1 (Onde está)** + **D1×C2 (Máquina)** + **D1×C3 (Clientes)** + **D1×C4 (Aquisição)** — todos se alimentam destes dados
- Estudo: `estudos/celula-D1-C1.md` §"Saída tangível" — o Raio-X começa a ser construído aqui
- Alimenta: `pop-etapa-3-reuniao-2-90m.md` (próxima Etapa)

---

## 7. Bump policy

- **patch (1.x.y)**: ajustar perguntas, simplificar campos
- **minor (x.0)**: trocar 1-2 perguntas (ex.: adicionar pergunta sobre M&A readiness, Gap G3)
- **major (X.0.0)**: reformular estrutura inteira (ex.: trocar repositório por questionário guiado)

---

## 8. Marcador no The Revenue Codex original

```
[cap. 02 — adotado em 2026-07-11 → motor-lct/Etapa 2 (auditar processos manuais)]
[cap. 06 — adotado em 2026-07-11 → motor-lct/Etapa 2 (validar 4 fundamentos)]
[cap. 07 — adotado em 2026-07-11 → motor-lct/Etapa 2 (5 perguntas-chave ampliam)]
[cap. 31 — adotado em 2026-07-11 → motor-lct/Etapa 2 (churn/NRR)]
[cap. 24 — adotado em 2026-07-11 → motor-lct/Etapa 2 (CRM Mínimo Viável como base)]
[cap. 10 — adotado em 2026-07-11 → motor-lct/Etapa 2 (Roadmap RICE)]
```

---

## 9. Histórico

| Data | Versão | Mudança |
|---|---|---|
| 2026-07-11 | 1.0.0 | Publicação inicial — Etapa 2 do D1. Coleta Densa remota (formulário + repositório) com 12 perguntas. |
