---
name: pop-garantia-indevista
description: Política de garantia incondicional de devolução do D1 + cláusulas anti-risco + processo de acionamento
version: 1.0.0
applies_to: [LCT Consulting / Degrau 1 / Etapa 1 - Contrato]
related_skills:
  - brand-lct                ← tom da garantia (Honestidade Brutal)
  - motor-governance        ← qualquer mudança precisa de checks
caps_referenced:
  - Cap. 18 (Desmistificando vendas) — vender = servir (cliente satisfeito = melhor vendedor)
  - Cap. 21 (BANT Turbo) — qualificação antes de aceite
governance:
  - Constituição §V (Honestidade Brutal) — garantia é real, não gimmick
  - LCT Manifesto §5 (o problema quase nunca é vendas) — extensão para garantia
related_pops:
  - pop-etapa-1-reuniao-1h.md     (Etapa 1 — referencia garantia)
  - template-contrato-d1.md      (anexo contratual)
---

# pop-garantia-indevista

## 1. Visão geral

Este POP define a **política de garantia incondicional de devolução do D1** — uma promessa que o Leandro (LCT) dá ao cliente: **se o Raio-X do Cliente (entregável-âncora da Etapa 4) não trouxer valor claro, a LCT devolve 100% do valor pago**.

> **Por que essa garantia existe:** o D1 é a **porta de entrada** da LCT Consulting. O risco principal é o lead pensar "tá caro" ou "vai dar errado". A garantia **remove o risco do cliente** e **força a LCT a entregar valor real** (senão devolve). É um **comprometimento simétrico** com a Honestidade Brutal (Constituição §V).

> **⚠️ Atenção crítica:** essa garantia **NÃO** é gimmick. É **real**. Se acionada, **devolve** o valor. Por isso, o POP define também **critérios para acionar** (sem cair em reclamação gratuita) e **processo de acionamento** (com 1 call de alinhamento antes de devolver).

---

## 2. A garantia em 1 parágrafo (para o email de Etapa 1)

> "Garantia incondicional de devolução: se, em até 30 dias após a entrega do Raio-X do Cliente (PDF 7-10 págs), você considerar que o relatório não entregou valor concreto para a sua operação, a LCT Consulting devolve integralmente os R$ 2.500 pagos. Sem letras miúdas, sem perguntas, sem reentrância. **Uma call de alinhamento** (30 min) será oferecida antes da devolução para confirmar o descompasso — e, se confirmado, devolvemos."

> Por que a call de alinhamento **antes** da devolução: para **confirmar que o descompasso é real** (e não confusão do cliente). A LCT acredita que a maioria dos casos resolve nessa call.

---

## 3. Cláusulas formais (no `template-contrato-d1.md`)

### 3.1 Texto exato da cláusula no contrato

> **CLÁUSULA X — GARANTIA INCONDICIONAL DE DEVOLUÇÃO**
>
> 1. A CONTRATADA (LCT CONSULTING) garante à CONTRATANTE a devolução integral do valor pago (R$ 2.500,00) caso o **Raio-X do Cliente** (entregável-âncora do D1) não entregue valor concreto à operação da CONTRATANTE.
>
> 2. O prazo para acionamento da garantia é de **30 (trinta) dias corridos** contados da entrega formal do Raio-X (data do email de entrega com anexo).
>
> 3. O procedimento de acionamento é:
>    a. CONTRATANTE solicita a devolução por email ao Leandro Tavares (contato principal);
>    b. CONTRATADA oferece, em até 5 dias úteis, uma **call de alinhamento** de 30 min para entender o descompasso;
>    c. Se após a call, CONTRATANTE mantiver o pedido de devolução, CONTRATADA devolve integralmente em até 10 dias úteis.
>
> 4. A garantia cobre **devolução integral** (100% do valor pago), sem cobrança de taxa administrativa ou parcialmente.
>
> 5. Excluem-se da garantia:
>    a. Não-entrega de informações pelo CONTRATANTE na Etapa 2 (Coleta Densa) que impeça o Raio-X de ter dados suficientes;
>    b. Cancelamento da Reunião 2 (Etapa 3) por iniciativa do CONTRATANTE com menos de 5 dias úteis de antecedência, mais de 1 vez.
>
> 6. Esta garantia é **adicional** aos direitos do consumidor previstos no Código de Defesa do Consumidor (Lei 8.078/90) e não os substitui.

### 3.2 Exclusões (sub-cláusula 5)

As exclusões existem para **proteção simétrica**:
- Se o cliente não entrega dados, a LCT não pode gerar Raio-X com qualidade.
- Se o cliente cancela reunião sem aviso, o esforço de preparação é desperdiçado.

---

## 4. Processo de acionamento (operacional)

### 4.1 Se cliente aciona a garantia

```
1. Cliente envia email: "Quero acionar a garantia"
2. LCT responde em 5 dias úteis com proposta de call de 30 min
3. Call acontece (audio ou video)
4. Decisão:
   a. Se alinhou → cancela devolução + oferece D2/D3/D4/D5
   b. Se mantém devolução → processa em 10 dias úteis (Pix ou estorno)
5. Documenta o caso em [cliente-lct-{empresa}/post-mortem-garantia.md]
```

### 4.2 Se cliente **não** aciona

- Raio-X é considerado entregue com sucesso
- Cadência de upsell (Etapa 4) segue normal
- Caso de sucesso vira referência (com permissão do cliente)

---

## 5. Critério de qualidade "Uau"

- A garantia **reduz atrito de compra** (lead não hesita)
- **Taxa de acionamento < 5%** (saúde da garantia = saúde do D1)
- Quando acionada, **call de alinhamento resolve 50%+ dos casos** (LCT identificou descompasso que tinha solução)
- **Nenhuma reclamação pública** (Procon, Reclame Aqui) — a LCT age antes de chegar nisso

---

## 6. Anti-patterns (não fazer)

- ❌ **Não usar "garantia de 30 dias"** como copy chamativa — a LCT não é loja de varejo
- ❌ **Não criar letra miúda** — a Constituição §V manda Honestidade Brutal
- ❌ **Não oferecer garantia maior do que isso** (ex.: 60 dias) — dilui o comprometimento
- ❌ **Não condicionar devolução a "satisfação subjetiva"** — exige critério objetivo: "o Raio-X não trouxe valor concreto"
- ❌ **Não usar "satisfação garantida"** — é frase de coaching

---

## 7. Cross-reference na matriz

- **D1 inteiro** — garantia é parte do **contrato do D1**, não de uma Camada específica
- Estudo: `estudos/celula-D1-C1.md` (origem da garantia) + `estudos/celula-D1-C4.md` (garantia como argumento de venda na Etapa 1)
- Anexos: `template-contrato-d1.md`

---

## 8. Bump policy

- **patch (1.x.y)**: ajustar texto da garantia, processo de acionamento
- **minor (x.0)**: mudar prazo (ex.: 30 → 45 dias), mudar exclusões
- **major (X.0.0)**: reformular filosofia (ex.: garantia condicional, escalonada)

---

## 9. Histórico

| Data | Versão | Mudança |
|---|---|---|
| 2026-07-11 | 1.0.0 | Publicação inicial — Política de garantia incondicional + processo de acionamento + cláusulas anti-risco. |
