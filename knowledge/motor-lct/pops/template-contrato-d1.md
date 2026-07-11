---
name: template-contrato-d1
description: Template do contrato D1 (LCT Consulting ↔ Cliente) + link de pagamento + anexo de garantia incondicional. PDF 1 página com cláusulas claras (sem letra miúda, em voz `brand-lct`)
version: 1.0.0
applies_to: [LCT Consulting / Degrau 1 / Etapa 1 - Envio de contrato]
related_pops:
  - pop-etapa-1-reuniao-1h.md   (Etapa 1 — dispara o envio deste contrato)
  - pop-garantia-indevista.md    (anexo contratual principal)
governance:
  - Constituição §V (Honestidade Brutal) — sem letra miúda
---

# template-contrato-d1

## 1. Visão geral

Este é o **template do contrato** enviado para o cliente **após aceite da Etapa 1 (Reunião 1)**, junto com o **link de pagamento**. É um **PDF de 1 página** (não 5, não 10) com cláusulas claras.

> **Por que 1 página:** quanto mais longo o contrato, mais hesitação. **1 página, com tudo claro, com garantia visível** é o que fecha a venda do D1.

---

## 2. Estrutura do PDF (1 página)

```
─────────────────────────────────────────────
CONTRATO DE PRESTAÇÃO DE SERVIÇO — D1 SESSÃO ESTRATÉGICA EXECUTIVA
─────────────────────────────────────────────

ENTRE:
CONTRATANTE: [Nome do Cliente], [CPF/CNPJ], [Endereço]
CONTRATADA: LCT CONSULTING LTDA, CNPJ XX.XXX.XXX/0001-XX, Leandro Tavares (representante legal)

OBJETO:
Realização de Sessão Estratégica Executiva (D1) da LCT Consulting, conforme especificações:
- 1 (uma) reunião estratégica de 90 minutos com o CEO-fundador (Leandro Tavares)
- 1 (um) Relatório Raio-X do Cliente (PDF 7-10 págs) entregue em até 7 dias corridos
- Acesso ao portal digital do cliente com todos os artefatos gerados

VALOR:
R$ 2.500,00 (dois mil e quinhentos reais) — pagamento único, à vista ou em parcela única via Pix/cartão.

VIGÊNCIA:
Da data de assinatura até a entrega do Raio-X ou 30 dias após o aceite (o que vier primeiro).

GARANTIA INCONDICIONAL DE DEVOLUÇÃO (CLÁUSULA PRINCIPAL):
A CONTRATADA garante à CONTRATANTE a devolução integral do valor pago (R$ 2.500,00) caso o Raio-X do Cliente não entregue valor concreto à operação da CONTRATANTE, conforme procedimento detalhado em anexo próprio ("Política de Garantia LCT") e em conformidade com o CDC (Lei 8.078/90).
Prazo para acionamento: 30 dias corridos após a entrega do Raio-X.

RESPONSABILIDADES DA CONTRATANTE:
(a) Disponibilizar-se para a Reunião Estratégica no horário agendado.
(b) Fornecer documentos e informações solicitados (Etapa 2 — Coleta Densa) em até 5 dias úteis.
(c) Não cancelar a Reunião com menos de 5 dias úteis de antecedência, mais de 1 vez.

RESPONSABILIDADES DA CONTRATADA:
(a) Conduzir a Reunião Estratégica com diligência técnica.
(b) Entregar o Raio-X do Cliente em até 7 dias corridos.
(c) Cumprir integralmente a Política de Garantia LCT.

DISPOSIÇÕES GERAIS:
Este contrato é regido pelas leis brasileiras. Foro: Comarca de [Cidade do Leandro]. Assinatura digital via plataforma [DocuSign / Clicksign / similar] é aceita.

ASSINATURAS:
CONTRATANTE: ___________________________ Data: ___/___/______
CONTRATADA: ___________________________ Data: ___/___/______

ANEXO: Política de Garantia LCT (1 página)
─────────────────────────────────────────────
```

> **Texto exato a ser usado no PDF.** Não tem letra miúda, segue `brand-lct` (Honestidade Brutal, sem hype).

---

## 3. Email de envio (junto com o contrato)

Aplicar `brand-lct`. Componentes:

```
Assunto: O que combinamos na call — aqui está o contrato e o link

Corpo:

[Nome],

Conforme conversamos na call de hoje (DD/MM/AAAA), segue:

→ Contrato: [link para o PDF do contrato]
→ Link de pagamento: [link do gateway — R$ 2.500,00]
→ Anexo: Política de Garantia LCT (1 página)

Sobre a garantia (em 1 frase): se, em até 30 dias após a entrega do Raio-X, você considerar que o relatório não trouxe valor concreto, devolvo integralmente os R$ 2.500. Sem perguntas. Uma call de alinhamento antes para garantir que o descompasso é real.

Próximo passo: ao confirmar o pagamento, envio o formulário da Coleta Densa (Etapa 2) — onde você me passa os documentos que estruturam a Reunião Estratégica de 90 min.

Qualquer dúvida, me avise.

Leandro
```

---

## 4. Procedimento de geração

### 4.1 Quem gera
Leandro (Arquiteto de Crescimento) gera o contrato **manualmente** em **DocuSign / Clicksign / similar** com:

1. **Preencher dados do cliente:** nome, CPF/CNPJ, endereço
2. **Preencher dados da LCT:** CNPJ, representante
3. **Datas:** data de assinatura = data do aceite
4. **Vigência:** 30 dias a partir da assinatura

### 4.2 Quem assina
- **Cliente:** assinatura digital via DocuSign
- **LCT:** assinatura de Leandro (digital)

### 4.3 Pagamento
- Gateway: **Stripe / Asaas / InfinitePay** (escolha 1 e padronize)
- Link expira em **7 dias** (se não pagar, re-disparar)

### 4.4 Onde armazenar
- PDF do contrato assinado: `cliente-lct-{empresa}/contrato-{data}.pdf` (repositório do cliente)
- Backup: `meus_forks/lct-motor/clientes/{empresa}/contrato-{data}.pdf` (privado)

---

## 5. Critério de qualidade "Uau"

- O cliente assina em **< 1 dia** após receber o email (sem hesitação, sem pedir tempo)
- **Zero cliques** no "voltar" do navegador (sem solicitar esclarecimento adicional)
- **Conversão aceite verbal → contrato assinado > 80%** (sem "vou pensar")

---

## 6. Anti-patterns (não fazer)

- ❌ **Não fazer contrato de 5-10 páginas** — 1 página, com tudo claro
- ❌ **Não usar linguagem jurídica complexa** ("doravante", "outrossim") — a LCT fala como operador
- ❌ **Não esconder a garantia em letra miúda** — a garantia é o **argumento de venda principal**
- ❌ **Não parcelar o pagamento** — 1 pagamento único (R$ 2.500)
- ❌ **Não condicionar pagamento a "aprovação interna"** — se aceitou verbalmente, está aceito

---

## 7. Cross-reference na matriz

- **D1 inteiro** — contrato é parte do D1, não de uma Camada específica
- Anexos: `pop-garantia-indevista.md` (política completa de garantia)

---

## 8. Bump policy

- **patch (1.x.y)**: ajustar texto, ajustar cláusulas
- **minor (x.0)**: mudar estrutura (ex.: 1 página → 2 páginas para incluir LGPD)
- **major (X.0.0)**: reformular completamente (ex.: mudar gateway, mudar tipo de assinatura)

---

## 9. Histórico

| Data | Versão | Mudança |
|---|---|---|
| 2026-07-11 | 1.0.0 | Publicação inicial — Template de contrato D1 (1 página) com garantia visível + link de pagamento + política anexa. |
