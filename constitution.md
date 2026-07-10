# 📜 Constitution — Princípios do Projeto LCT

> **Atenção:** Este arquivo define as regras **deste envelope de projeto** dentro da empresa-de-skills.
>
> Não confundir com [`constitution-do-motor-lct.md`](./constitution-do-motor-lct.md) — aquela governa o **Motor LCT** (ativo-fim). Esta aqui governa **como operamos o Motor dentro da nossa estrutura de skills**.

---

## 1. Hierarquia de princípios

A Constituição do Motor LCT **sempre vence** qualquer decisão de skills ou processo deste envelope. Se uma escolha de skill ou workflow colidir com um dos 10 princípios (Sequência Inversa, Sincronia MD↔JSON, Cadeia de Espetacularidade etc.), ela é bloqueada antes de ser executada.

## 2. Princípios do envelope

### 2.1 Semântica > estética
Toda skill escolhida precisa **mudar uma saída** do Motor ou da LCT. Skill por skill, sem score de decoração.

### 2.2 Elenco enxuto
3-12 skills por sprint. Mais que isso vira skill-spam.

### 2.3 Sempre com elo anterior pronto
A "Cadeia de Espetacularidade" do Motor se estende aqui: nenhuma Etapa nova começa antes da anterior estar **excelente**.

### 2.4 Skills referenciadas, não copiadas
Toda skill vem de `../../../skills-catalogo/`. Nunca dup-a dentro do PROJ-02.

### 2.5 Memória > capacidade
Decisões, escolhas de skill, erros — tudo em [`memory.md`](./memory.md). Não confie em chat longo, confie em arquivo.

### 2.6 Cross-LLM é histórico
A constituição original definia 3 integrações paralelas (Claude, Gemini, Opencode). **Não importamos essa infraestrutura para este envelope**. Operamos só com Claude + spec-kit + skills. Se precisar de outro LLM no futuro, é projeto separado.

## 3. Limites

### 3.1 Conflitos com o usuário
- Você é sócio-fundador. Decisões de preço, escopo, posicionamento final são suas.
- Sugestões de skill ou copy são minhas — você aprova.

### 3.2 O que **NÃO** fazer
- ❌ Modificar o `manifesto.md` sem autorização
- ❌ Tocar `LCT_Consulting_SDD/` (original fica intocado)
- ❌ Sincronizar matriz só MD ou só JSON
- ❌ Pular Etapas da Cadeia de Espetacularidade

## 4. Histórico de revisões

| Data | Mudança | Por quê |
|---|---|---|
| 2026-07-09 | Versão inicial | Setup do envelope |
