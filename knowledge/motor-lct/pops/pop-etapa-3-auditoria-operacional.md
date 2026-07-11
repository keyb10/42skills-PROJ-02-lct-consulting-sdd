---
name: pop-etapa-3-auditoria-operacional
description: Etapa 3 do D1 — Auditoria operacional da máquina-cliente (60-90 min) durante a Reunião 2 (mapa de ineficiência, 4 Fundamentos, candidatos a IA)
version: 1.0.0
applies_to: [LCT Consulting / Degrau 1 / Etapa 3 - Sessão Estratégica 90 min]
related_skills:
  - business-pulse            ← pulso geral da operação
  - process-doc               ← verificar documentação
  - process-optimization      ← identificar gargalos
  - runbook                   ← verificar replicabilidade
  - capacity-plan             ← verificar dimensionamento
  - internal-comms            ← verificar comunicação interna
caps_referenced:
  - Cap. 06 (Fundamentos que travam/libertam crescimento)
  - Cap. 10 (Roadmap RICE)
  - Cap. 24 (CRM Mínimo Viável)
governance:
  - Constituição §I (Sequência Inversa) - D1×C2 segue D1×C1
  - Constituição §II (Profundidade M em D1)
  - Manifesta §3 (IA como amplificador, não magia)
related_study: estudos/celula-D1-C2.md
---

# pop-auditoria-maquina-cliente

## 1. Visão geral

Este POP operacionaliza a **Auditoria Operacional Leve** do LCT — uma sessão de **60-90 minutos** (pode ser rodada imediatamente após o `pop-diagnostico-ceo-90m` ou em horário separado, mesmo dia) que produz a seção "Mapa de ineficiência" do Raio-X do Cliente.

**Quem aplica:** Arquiteto de Crescimento (Leandro ou prep)
**Quando:** entre a sessão 90 min e o Raio-X entregue (7 dias)
**Pré-requisito:** `pop-diagnostico-ceo-90m.md` rodado antes
**Saída:** Mapa de ineficiência (1 página), lista de capacidades a IA-amplificar (½ página), ambos alimentando o Raio-X

---

## 2. Convocação (24-48h antes)

Rodar `customer-pulse` (KB/small-business) com formulário estendido para o **time técnico/operacional** (não só o CEO).

**Envolvidos (1-2 pessoas):**
- COO ou Diretor de Operações (se houver)
- Head de TI / Engenheiro-líder (se houver) ou pessoa de referência
- ⚠️ **Não** envolver o CEO na parte técnica — queremos diagnosticar a máquina dele sem o viés dele

| Pergunta | Objetivo |
|---|---|
| "Quem faz o quê na sua área? (cargo, não nome)" | Mapa de papéis |
| "Qual processo seu time faz que você acha que poderia ser automatizado?" | Identificar candidatos a IA |
| "Onde sua área costuma falhar/atrasar?" | Identificar gargalos |
| "Quanto tempo no mês vocês gastam em planilhas/relatórios manuais?" | Calcular custo oculto |
| "Vocês têm CRM? Qual? Quem atualiza?" | Avaliar Cap. 24 (CRM Mínimo) |
| "Existe documentação dos processos (runbook, SOP)?" | Avaliar Cap. 06 (Fundamentos) |
| "Quando alguém entra no time, como aprende a rotina?" | Medir se replicabilidade existe |
| "Se o Leandro saísse amanhã, o que para?" | Detector de centralização |
| "Quanto do seu tempo vai em report (CEO+board)?" | Detector de gargalo-pessoa |
| "Qual processo você tem medo de mexer?" | Detector de pré-requisito bloqueado |

---

## 3. Os 60-90 minutos

### 3.1 Abertura (5 min)

```
"Obrigado por dispor desse tempo. Esta conversa é entre nós.
Eu vou perguntar sobre como a [empresa] opera hoje em termos
muito práticos — para onde o tempo vai, onde as coisas travam.
Não é avaliação do seu trabalho, é sobre o desenho da operação."
```

**Garantir:** ambiente confortável. Pode ser presencial ou call gravada.

---

### 3.2 Os 4 Fundamentos Desalinhados (15-20 min) — Cap. 06

Para cada um dos 4 fundamentos, fazer a pergunta-base e marcar com ✅ (alinhado), ⚠️ (parcialmente) ou 🔴 (desalinhado).

#### F1 — **PMF (Product-Market Fit)**

> "Vocês sentem que o produto 'encaixa' no cliente? Recebem feedback de que **resolveram** um problema real? Ou é mais 'legal mas não indispensável'?"

**Marcadores:**
- ✅: "clientes usam, amam, indicam, apontam upgrades"
- 🔴: "usam pouco, poderiam trocar por concorrente sem sentir"

---

#### F2 — **ICP (Perfil de Cliente Ideal)**

> "Vocês sabem quem é o cliente ideal? Tem documento escrito, ou é mais 'sentimento'? E quando um lead entra, como vocês decidem se vale a pena?"

**Marcadores:**
- ✅: ICP escrito, qualificação caseira (BANT-like), taxa de conversão saudável
- 🔴: "todo lead é tratado igual", "nunca atualizamos o perfil"

**Bonus:** perguntar "qual seu cliente-que-deu-mais-lucro-no-ano-passado, e quanto?". Anote.

---

#### F3 — **Oferta & Preço**

> "Vocês têm preço tabelado? Tem cliente que conseguiu desconto recente? Qual percentual de vendas exigiu desconto nos últimos 6 meses?"

**Marcadores:**
- ✅: preço tabelado, baixa customização
- 🔴: "mais de 30% das vendas fecharam com desconto"

---

#### F4 — **Roadmap de Produto**

> "Vocês têm roadmap escrito dos próximos 90 dias? Quem decide o que entra? E quanto do roadmap é 'pedido de cliente vs. iniciativa própria'?"

**Marcadores:**
- ✅: roadmap escrito, score (RICE ou similar), calendarizado
- 🔴: "entra o que cliente gritar mais alto" (Cap. 10 §6.6 sinal amarelo)

---

### 3.3 Mapeamento de Processos Críticos (15-20 min) — Cap. 10+24

Para cada processo crítico perguntar:
- Quem faz? (papel)
- Quantas horas/semana?
- Quantas etapas manuais?
- Onde trava?

| Processo (CEO/C-level menciona) | Dono (papel) | Tempo/sem | Manual steps | Onde trava |
|---|---|---|---|---|
| Ex: "fechar proposta" | "time comercial" | "8h" | "3 (CRM, modelo, aprovação)" | "aprovação do CEO" |
| "atendimento do cliente" | "CSM" | "..." | ... | ... |

**Cross-reference:** se processo tem **muitos steps manuais + trava em aprovação**, é candidato a IA-amplificar (D4 implantará).

---

### 3.4 Gargalos & Candidatos a IA (10-15 min)

Perguntar:
> "Quais processos do seu dia-a-dia mais te fazem perder tempo?"
> "Quais você não faria se pudesse voltar no tempo?"
> "Se você pudesse delegar 3 coisas para um agente IA, quais seriam?"

⚠️ **Atenção:** perguntar à pessoa OPERACIONAL (não CEO). CEO tende a superestimar o que IA pode fazer.

**Anotar Top-3 candidatos a IA-amplificar**, com nota:

```
Candidato 1: [descrição]
  - Volume: (semanal/mensal)
  - Tempo economizado: ___ h/sem
  - Risco: (baixo/médio/alto)
  - Pode ir pra D4? (sim/não/depende)
```

---

### 3.5 Dimensão Humana (5 min)

> "Sua equipe cresce? Quanto? Onde costuma travar contratação?"
> "Existe documentação de onboarding? Walkthrough de 90 dias?"

**Anotar:**
- Crescimento previsto: ___ pessoas nos próximos 12m
- Tempo de ramp-up para novo funcionário: ___ dias
- Onde a centralização trava: (no CEO, em X, etc.)

---

## 4. Saída

Documentar **2 entregas**:

1. **Mapa de ineficiência (1 página)** — quadro com:
   - 4 Fundamentos ✅/⚠️/🔴
   - Processos críticos x gargalo
   - Lista de centralização

2. **Lista de capacidades a IA-amplificar (½ página)** — bullet-list de 3-8 candidatos, com volume/risco.

Ambos vão como **seções do Raio-X** (ver `template-raio-x.md`).

---

## 5. Cross-reference na matriz do Motor

Esta seção do Raio-X alimenta:
- **D1×C2** do Motor (já documentado em `estudos/celula-D1-C2.md`)
- Preparação de **D2×C2** (Mentoria: máquina pronta, caps 10+24+33)
- Preparação de **D4×C2** (Consultoria Full: implantação Mowia, caps 10+11+núcleo A)

---

## 6. Critério de qualidade "Uau"

- O time técnico sai da sessão dizendo "ok, **finalmente alguém perguntou**". Não aconteceu antes.
- O CEO sai do Raio-X vendo **2-3 lugares específicos** onde IA pode entrar antes de qualquer D4.
- **Nenhum dos 4 Fundamentos** deveria estar ✅+ + ✅ + ✅ + ✅ — sempre há pelo menos 1 ⚠️ ou 🔴.

---

## 7. Anti-patterns (não fazer)

- ❌ **Não envolver o CEO na parte técnica** — perderia o viés
- ❌ **Não prometer automatização no D1** — promessa de IA só depois de D3×C2 confirmar viabilidade
- ❌ **Não diagnosticar áreas que não envolvem a operação** (vendas/CS/dados têm suas próprias auditorias)
- ❌ **Não usar mais que 90 min** — profundidade sem extensão é melhor que superficialidade

---

## 8. Bump policy

- **patch (1.x.y)**: ajustar perguntas, refinar marcadores
- **minor (x.0)**: adicionar Fundamento (ex.: "5º" como governança)
- **major (X.0.0)**: trocar Cap. (ex.: Cap. 06 → outro compêndio)

---

## 9. Histórico

| Data | Versão | Mudança |
|---|---|---|
| 2026-07-10 | 1.0.0 | Publicação inicial — auditoria operacional leve, 4 Fundamentos Cap. 06 + Processos Cap. 10 + CRM Cap. 24 |
