---
name: pop-etapa-3-pulse-clientes
description: Etapa 3 do D1 — Pulse dos clientes atuais durante a Reunião 2 (Matriz Valor×Fit, expansão orgânica, 2 perguntas provocadoras)
version: 1.0.0
applies_to: [LCT Consulting / Degrau 1 / Etapa 3 - Sessão Estratégica 90 min]
related_skills:
  - customer-pulse            ← elicitação inicial (formulário 1)
  - customer-pulse-check      ← validação cruzada
  - ticket-triage             ← fricção do cliente como proxy de saúde
  - kb-article                ← verifica se conhecimento é tribal ou documentado
  - churn-prevention         ← frame geral
caps_referenced:
  - Cap. 08 (ICP: Matriz Valor × Fit)
  - Cap. 25 (Retenção Turbinada)
  - Cap. 26 (Onboarding 30-30-30)
  - Cap. 28 (Renovação 90d + upsell orgânico)
governance:
  - Constituição §I (Sequência Inversa: C3 vem depois de C2)
  - Manifesto LCT §5 (retenção = "oxigênio do crescimento barato")
related_study: estudos/celula-D1-C3.md
---

# pop-pulse-clientes-atuais

## 1. Visão geral

Este POP mapeia a **base atual de clientes** do CEO-cliente — onde estão, quanto valem, se prestam, e se cresce com eles. Saída: **Matriz Valor×Fit (1 página)** + **lista de expansão orgânica** (½ página) + **2 perguntas provocadoras** (linha do entregável), alimentando a seção "C3" do Raio-X.

**Quem aplica:** Arquiteto de Crescimento
**Quando:** entre `pop-auditoria-maquina-cliente.md` e o Raio-X entregue
**Pré-requisitos:** os dois POPs anteriores já rodaram (CEO + time técnico)

---

## 2. Convocação (24-48h antes)

Rodar `customer-pulse` (KB/small-business) expandido:

| Pergunta | Resposta |
|---|---|
| Top-5 clientes em receita anual (anonimizado): #1 / #2 / #3 / #4 / #5 | (em R$) |
| Em qual cliente cada um deles está em fase de: uso intenso / uso moderado / pagamento mas não usa / cancelou | (check por cliente) |
| Clientes com contrato renovado nos últimos 30 dias (quantos) | |
| Clientes com churn voluntário nos últimos 30 dias (quantos) | |
| Clientes com churn involuntário (cartão expirado, etc.) nos últimos 30 dias (quantos) | |
| Top-1 cliente insatisfeito (cliente nomeado) | (anonimizado) |
| Top-1 cliente insatisfeito (cliente nomeado) | (anonimizado) |

> ⚠️ **Atenção:** se CEO hesitar em responder top-1 insatisfeito, **isso é sinal amarelo de saúde da base**. Anotar.

---

## 3. Os 60-90 minutos com o CEO

### 3.1 Abertura (5 min)

```
"Agora vamos olhar a sua base de clientes atuais. Eu vou fazer
algumas perguntas provocadoras. Você responde o que souber —
não precisa inventar dados que não tem. Onde você não souber,
isso também é insumo pra gente."
```

---

### 3.2 Plotar a Matriz Valor×Fit (30 min) — Cap. 08

**Processo:** para cada um dos top-5 clientes:

```
"Vamos pegar o cliente #1 (que pagou R$ X). Numa escala de 1-5,
o quanto ele é valioso pro seu negócio? E numa escala 1-5, o
quanto ele se encaixa no seu público-alvo (fit)?"

#1: Valor [___] / Fit [___]   → Q1 (alto valor + alto fit) ou outro
#2: Valor [___] / Fit [___]   → ...
```

**Onde plotar (4 quadrantes — Cap. 08):**

```
                  FIT alto  │  FIT baixo
      ┌─────────────────────┬─────────────────────┐
      │ Q1                  │ Q2                  │
VALOR │ ALTO                │ ALTO                │
alto  │ Sonho. Foco.        │ Dilema. Aceito mas  │
      │                     │ custoso.            │
      ├─────────────────────┼─────────────────────┤
      │ Q3                  │ Q4                  │
VALOR │ Fan, menor hoje.    │ "Demitir"           │
baixo │ Pode crescer.       │ educadamente.       │
      └─────────────────────┴─────────────────────┘
```

**Anotar (no Raio-X):** marcar os 5 top-clientes em quadrantes.

---

### 3.3 Expansão Orgânica (15 min) — Cap. 28

Para cada cliente Q1 e Q2:

> "Você enxerga nesse cliente uma **expansão natural** que ainda não conversou? O que vendeu + o que poderia vender? Que frequência de comunicação tem com ele?"

**Anotar (no Raio-X):**
- Top-3 clientes com expansão natural não capturada
- Frequência atual vs. frequência ideal (QBR 90d é o cap. 28)

**Atenção:** "expansão orgânica" não é "empurrar upgrade". É **encontrar fit não explorado** que beneficia o cliente.

---

### 3.4 Onboarding Estruturado (10 min) — Cap. 26

> "Quando um cliente novo entra hoje, o que acontece com ele nos primeiros 30 dias? Quem fala com ele? Quantas vezes? Você tem o que o Cap. 26 chama de '30-30-30' (3 primeiros dias intensos, 30 dias ativos, 90 dias renovados)? Ou mais 'fill-the-pool-and-pray'?"

**Marcar:**
- ✅: onboarding estruturado (sondagem + 30-30-30)
- 🔴: "cliente entra e ninguém mexe por 60-90 dias"

---

### 3.5 Saúde da renovação (10 min) — Cap. 28

> "Quem cuida das renovações no seu time? Com que antecedência a renovação é tratada? Tem alguém sabendo se vai renovar, ou você descobre 30 dias antes?"

**Marcadores:**
- ✅: QBR 90d antes da renovação
- 🔴: "renovação vira surpresa"

---

### 3.6 As 2 Perguntas Provocadoras (5 min) — fechamento

```
P-P1: "Como você sabe se o cliente vai renovar?"
P-P2: "Qual a taxa de churn que você acha que tem, mas não mede?"
```

⚠️ **Atenção:** essas perguntas ficam ecoando. CEO sai da sessão pensando nelas. Se ele "respondeu rapidamente" — provavelmente a resposta é "feeling", não dado. Anotar no Raio-X como "sinais de saúde da base não medidos".

---

## 4. Saída

Documentar **2 entregas**:

1. **Matriz Valor×Fit (1 página)** — visual com os top-5 plotados
2. **Lista de expansão orgânica (½ página)** — 3-5 clientes Q1/Q2 com hipótese de cross-sell

Vão como **seções do Raio-X** (ver `template-raio-x.md`).

**Perguntas provocadoras** ficam no Raio-X como **linha-selo** (não como resposta) — continuam ecoando.

---

## 5. Cross-reference na matriz

Esta seção do Raio-X alimenta:
- **D1×C3** do Motor (já documentado em `estudos/celula-D1-C3.md`)
- Preparação de **D2×C3** (Mentoria: Health Score 1.0 + Retenção Turbinada, caps 25-28)
- Preparação de **D3×C3** (Diagnóstico: Health Score 2.0 com coortes, caps 25-28+31)
- Preparação de **D4×C3** (Consultoria: Playbook CS, caps 25-28 — núcleo A)

---

## 6. Critério de qualidade "Uau"

- O CEO sai do D1 com **lista nominal de 3-5 clientes insatisfeitos** que ele não conhecia como insatisfeitos.
- Ele sai perguntando "**como medir churn invisível?**" (gatilho para D2×C3).
- A Matriz Valor×Fit tem **pelo menos 1 cliente plotado em Q4** ("demitir educadamente") — isso cria coragem na decisão.
- Lista de expansão orgânica tem **pelo menos 1 cliente com hipótese testável em ≤ 30 dias**.

---

## 7. Anti-patterns (não fazer)

- ❌ **Não chamar de "cancelar cliente"** — usar "descontinuar comercialmente" ou "demitir educadamente" (Cap. 08)
- ❌ **Não prometer retenção numérica** — Cap. 29 + LCT Constitution §V
- ❌ **Não pressionar o CEO a listar insatisfeitos** — se ele hesitar, anote a hesitação
- ❌ **Não confundir fit alto com valor alto** — quadrante Q4 (alto fit, baixo valor) é o fan que cabe, baixa ainda — não é ruim

---

## 8. Bump policy

- **patch (1.x.y)**: ajustar perguntas, refinar marcadores
- **minor (x.0)**: adicionar quadrant (ex.: "Q5 - cliente em churn ativo em processo de salvamento")
- **major (X.0.0)**: trocar Cap. 08 por outra metodologia de segmentação de base

---

## 9. Histórico

| Data | Versão | Mudança |
|---|---|---|
| 2026-07-10 | 1.0.0 | Publicação inicial — Matriz Valor×Fit + expansão orgânica + 2 perguntas provocadoras |
