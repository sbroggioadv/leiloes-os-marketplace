---
name: tutela-de-urgencia-leiloes
description: "Tutela de urgencia no dominio do leilao: suspender o certame ANTES de acontecer, suspender a imissao/reintegracao, ou destravar carta e mandado. Monta o pedido com probabilidade + perigo + reversibilidade (CPC 300 — fora da faixa capturada, confira na fonte) e carrega as duas travas do dominio: no extrajudicial o art. 30, paragrafo unico da Lei 9.514 quase nada obsta a reintegracao (exceto notificacao), e no judicial o CPC 903 §6o pune vicio infundado com multa de ate 20% do valor atualizado do bem. Use quando disserem preciso de liminar, suspender o leilao, parar a imissao, juiz negou a carta, quero liminar na anulatoria, destravar a arrematacao."
---

> **🖱️ Escolhas = botoes:** nas perguntas de lista fechada use **AskUserQuestion** (max. 4 por pergunta).

# TUTELA-DE-URGENCIA-LEILOES

> Camada transversal. Publico 🎓. **A liminar e o que decide o caso antes do merito** — e no leilao a fase e a via erradas matam o pedido mesmo com tese boa.

## Anexos obrigatorios (context/)
- `context/cpc-leilao-879-903.md` — **CPC, art. 903, §§1º a 6º** (relogio, 3 portas, freio do §6º) e **CPC, art. 901, §§1º-2º** (carta e mandado) — **grep + ler a faixa**.
- `context/lei-9514-consolidada.md` — **Lei 9.514, art. 30** caput e **paragrafo unico** (liminar + 60 dias; eixo unico) — **grep + ler a faixa**.
- `context/jurisprudencia-leiloes.md` — §8 (intimacao = eixo) · §10 (**REsp 2.171.564/SP pendente**) — **grep + ler a faixa**.
- `context/metodologia-leiloes.md` — fase, selos, documento faltante = **nao alegar** — **ler primeiro**.

## Objetivo
Produzir o **pedido de tutela** (na inicial, em peticao intermedia ou em agravo) com os **tres requisitos**, o **documento que prova cada um**, e o alerta honesto de **quando a liminar e fraca por construcao da lei**.

## 🟡 CPC 300 NAO esta na faixa capturada
`context/cpc-leilao-879-903.md` cobre **876-903 + 804 + 826 + 908 §1º**. O **art. 300 do CPC** (tutela de urgencia) **nao foi capturado verbatim** neste corpus. Cite-o **pelo numero e pelo conteudo** (probabilidade do direito · perigo de dano ou risco ao resultado util do processo · **reversibilidade**); **nao** ponha o texto entre aspas como se fosse verbatim. 🟡 **Antes de protocolar, confira a redacao vigente na fonte oficial** → `validador-leiloes`. O R4 da `suprema-corte-leiloes` ja manda checar CPC 300 quando cabivel.

## Metodologia
1. **Botoes: o que voce quer da liminar?** — **suspender o leilao antes** · **suspender imissao/reintegracao** · **destravar carta/mandado** · **efeito suspensivo em agravo** (detalhe em `agravo-de-instrumento-leiloes`).
2. **Botoes: via e fase?** — **judicial** · **extrajudicial AF (9.514)** · **hipoteca art. 9º da 14.711** × **antes do pregao** · **pos-lance <10 dias do auto** · **pos-carta** · **pos-imissao**. A fase decide se ainda ha o que suspender.
3. **Rodar os 3 requisitos** com **documento** em cada um. Sem documento = **nao pedir** (ou pedir fraco e honesto).
4. **Aplicar a trava da via** (tabela abaixo) — no extrajudicial a lei **ja comprime** o que a liminar pode fazer.
5. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## Os 3 requisitos (sempre os tres)

| Requisito | O que provar no leilao | Documento tipico |
|---|---|---|
| **Probabilidade do direito** | Vicio **concreto** (intimacao, omissao de onus, preco vil com a regua certa) | Edital, matricula, AR/intimacao, auto, avaliacao |
| **Perigo / risco ao resultado util** | Consumacao **irreversivel** do certame, desocupacao, consolidacao do titulo | Data do leilao, mandado, auto assinado, carta |
| **Reversibilidade** | A liminar **nao** cria dano desproporcional a parte contraria se o merito cair | Oferta de caucao quando o juizo exigir; escopo minimo do pedido |

⛔ **Pedido generico ("suspenda tudo") sem amarrar os tres e pedido que convida ao indeferimento.**

## ⭐ As 3 hipoteses de uso

### 1) Suspender o leilao **ANTES** de acontecer
- **Quando:** edital publicado, pregao ainda nao realizado (ou entre 1º e 2º).
- **Judicial:** impugnacao nos autos da execucao + tutela; cabimento de agravo se indeferida (`agravo-de-instrumento-leiloes`).
- **Extrajudicial:** anulatoria (ou cumpra-se) **com liminar** para obstar o certame — peca-mae em `anulatoria-de-leilao-extrajudicial`.
- ⭐ Fundamento forte: **vicio de intimacao/notificacao** (Lei 9.514, art. 26, inclusive §4º-B). Preco e clausula, sozinhos, sao **fracos** para parar o leilao apos consolidacao (ver trava do art. 30).
- 🟡 **REsp 2.171.564/SP** (ex-AREsp 2.471.891, 3a Turma, **PENDENTE** — sem julgamento, sem tese): **nao** existe precedente do STJ estendendo o CPC 886, VI ao edital extrajudicial. Quem pede liminar por omissao de onus no extrajudicial funda-se em **dever de informacao e boa-fe**, nao em tese inexistente.

### 2) Suspender a **imissao / reintegracao**
- **Judicial:** mandado de imissao so depois de preco + comissao + despesas + **ITBI** e dos **10 dias** do CPC 903, §2º (**CPC 901, §§1º-2º** · **903, §3º**). Suspender imissao sem atacar o titulo e **uphill**.
- **Extrajudicial — a trava que decide:**

> **Lei 9.514, art. 30, paragrafo unico** (redacao da 14.711/2023): arrematado o imovel ou consolidada definitivamente a propriedade, acoes sobre **estipulacoes contratuais ou requisitos procedimentais** de cobranca e leilao **nao obstam** a reintegracao e resolvem-se em **perdas e danos** — **excetuada a exigencia de notificacao** do devedor / terceiro fiduciante.

🔴 **Consequencia para a liminar:** no extrajudicial, **quase nada obsta** a reintegracao. Pedido liminar de manutencao de posse fundado em **preco vil, avaliacao ou publicidade** pede o que a lei **nao da**. Sobra o eixo da **notificacao**. Caput do art. 30 Lei 9.514 da liminar **expressa + 60 dias** ao **arrematante** — do outro lado do balcao a liminar e **contra** o ocupante.

### 3) Destravar **carta** ou **mandado**
- Pedido do **arrematante** quando o juizo retarda a carta apos os 10 dias do §2º sem alegacao, ou condiciona indevidamente.
- Checklist textual: preco depositado · comissao · despesas · **prova de ITBI na carta** (CPC 901, §2º). Sem isso, a tutela **nao** "forca" o que a lei condiciona.
- Pos-carta, invalidacao so por **acao autonoma** com arrematante como **litisconsorte necessario** (CPC 903, §4º) — a tutela muda de objeto (efeito da acao, nao "reabrir" o §2º).

## 🔴 Freio do CPC 903, §6º — base colada
> Suscitar vicio **infundado** para ensejar a desistencia do arrematante e **ato atentatorio** a dignidade da justica: multa de **ate 20% do valor atualizado do bem**, devida ao exequente, sem prejuizo de perdas e danos.

⛔ **Nunca** confunda com **CPC 896, §2º** (20% da **avaliacao**, beneficio do incapaz) nem com a janela de **10 dias** do **CPC 903, §2º** (prazo, nao multa). Na liminar: **documento primeiro**; alegacao especulativa expoe o cliente ao §6º.

## Regras de ouro
- **Fase primeiro.** Errar a fase entrega liminar impossivel.
- **Via primeiro.** Extrajudicial = art. 30, §unico Lei 9.514; judicial = 903 + 901.
- **Documento = tese.** Faltando prova, a entrega e **NO-GO de liminar** ou pedido **residual** (so perdas e danos), nunca "provavelmente o juiz aceita".
- Cross-link soft: anulatoria extrajudicial → `anulatoria-de-leilao-extrajudicial` · judicial → `anulatoria-de-arrematacao-judicial` · imissao → `imissao-na-posse-do-arrematante` · defesa do ocupante → `defesa-contra-imissao-e-embargos-de-terceiro` · agravo da liminar → `agravo-de-instrumento-leiloes` · intimacao → `nulidades-de-intimacao-e-notificacao`.

## Entrega obrigatoria final
Pedido de tutela com: (a) **hipotese** (suspender leilao / suspender imissao / destravar carta); (b) **via e fase**; (c) os **3 requisitos** com o documento de cada um; (d) pedido **minimo e reversivel**; (e) alerta do **art. 30, §unico** quando extrajudicial; (f) alerta do **903, §6º** (ate **20% do valor atualizado do bem**) se houver risco de vicio fraco; (g) ressalva 🟡 do CPC 300 e do **REsp 2.171.564/SP pendente** se tocados. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Nunca liminar extrajudicial contra reintegracao fundada em **preco** — so **notificacao** obsta (art. 30, §unico). Nunca citar **REsp 2.171.564/SP** como tese existente. Nunca percentual sem base: **20% do valor atualizado do bem** (§6º) ≠ **20% da avaliacao** (896, §2º). Nunca aspas de CPC 300 como verbatim. Nunca alegar sem documento. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
