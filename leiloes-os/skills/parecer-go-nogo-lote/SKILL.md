---
name: parecer-go-nogo-lote
description: "⭐ A skill-vitrine do plugin: consolida as 4 provas do gate (edital, matricula, ocupacao e debitos) mais o risco de anulacao e a conta completa em um parecer com veredito GO, GO-CONDICIONADO ou NO-GO, com o porque de cada componente e o TETO DE LANCE. Documento faltando nao vira ressalva no rodape: vira NO-GO por insuficiencia de prova — nunca provavelmente esta ok, nunca aparentemente livre, nunca nao identifiquei onus quando o que houve foi nao ter lido. Entrega em dois registros sem trocar o corpus: parecer e conta para o investidor, parecer e tese para o advogado. E a resposta honesta a pergunta vale a pena esse lote, que os 8 SaaS concorrentes respondem de forma binaria e errada. Use sempre que perguntarem vale a pena esse lote, esse leilao e bom, quanto devo lancar, analisa esse imovel pra mim, monta o parecer, e uma boa oportunidade, /go-no-go, antes do lance."
---

> **🖱️ Escolhas = botoes:** nas perguntas de lista fechada use **AskUserQuestion** (max. 4 por pergunta).

# PARECER-GO-NOGO-LOTE ⭐⭐

> Camada 2. **A vitrine.** Nao e uma etapa do produto — **e o produto**. Consolida [1]-[4] + risco + conta em **um veredito com numero**, e diz **por que** de cada componente.

## ⛔ DEPENDENCIA DO GATE — declarada na abertura
**Este parecer nao sai sem as 4 provas documentais:**

| | Prova | Skill |
|---|---|---|
| **[1]** | **EDITAL** lido | `analise-de-edital` |
| **[2]** | **MATRICULA** lida | `leitura-de-matricula` |
| **[3]** | **OCUPACAO** apurada | `situacao-possessoria` |
| **[4]** | **DEBITOS** levantados | `debitos-propter-rem` |

Mais `risco-de-anulacao-do-certame` ⭐ e `custo-total-real-e-precificacao`. **So com GO seguem** `estrategia-de-lance-e-habilitacao` e `arrematacao-parcelada-895`.

🚨 **A REGRA DO DOCUMENTO FALTANTE:** faltando **qualquer** das 4, o veredito e **NO-GO por insuficiencia de prova** — e o parecer **nomeia qual prova falta e como obte-la**. ⛔ **Nunca** "provavelmente esta ok" · **nunca** "aparentemente livre" · **nunca** "nao identifiquei onus" quando o que houve foi **nao ter lido**.

**A razao e TEXTUAL, nao pedagogica:** o **CPC 903, §2º** conta os 10 dias do **APERFEICOAMENTO** (a assinatura do auto), **nao da ciencia do vicio**. O vicio oculto aparece na imissao, **meses depois** — e ali o §2º ja correu. **Due diligence pos-lance chega tarde por construcao da lei**, e por isso o gate e PRE-lance.

## Anexos obrigatorios (context/)
- `context/metodologia-leiloes.md` — **§3 o gate e os tres vereditos** · **§8 os selos e a regua de postura honesta** — **ler primeiro, sempre**.
- `context/custo-total-do-arrematante.md` — §13, o **checklist das 12 linhas** que a conta precisa fechar — **grep + ler a faixa**.
- `context/resolucao-cnj-236-2016.md` — **art. 18** (sem garantia; o onus de verificar e do interessado) — **grep + ler a faixa**.
- `context/mercado-leiloes-2026.md` — desagio medio de **37,3%** e o que os concorrentes **nao** fazem — **grep + ler a faixa**.
- `context/jurisprudencia-leiloes.md` — para carregar cada precedente **com a qualificacao** — **grep + ler a faixa**.

## Metodologia
1. **Pergunta em botoes (lista fechada): quais provas voce ja tem?** — **as 4** · **edital e matricula** · **so o edital** · **nenhuma ainda**. Qualquer resposta diferente de "as 4" **define o veredito antes da analise**: e **NO-GO por insuficiencia de prova**, e o parecer vira **plano de obtencao de prova**.
2. **Recolher as saidas** das seis skills do gate — sem reescreve-las: o parecer **consolida**, nao refaz.
3. **Cruzar os achados**: o que a matricula mostra e o edital nao menciona (886, VI) · quem ocupa contra o prazo ate a posse · a divida informada contra o desagio · o risco de anulacao contra o valor exposto.
4. **Fechar a conta** e obter o **teto de lance**, com a comissao **por fora**.
5. **Emitir UM dos tres vereditos** (tabela abaixo) — nunca um quarto, nunca "depende".
6. **Escrever no registro do publico** (💰 conta e decisao · 🎓 tese e proxima peca).
7. Fechar por `suprema-corte-leiloes` (R1-R4) + `validador-leiloes`.

## Os tres vereditos — e so estes tres

| Veredito | Quando | O que acompanha, obrigatoriamente |
|---|---|---|
| **GO** | as 4 provas lidas · risco de anulacao **baixo** · a conta fecha com margem | **Teto de lance** com a comissao embutida + o **valor a lancar** (teto menos comissao) |
| **GO-CONDICIONADO** | as 4 provas lidas, mas ha **condicao objetiva a resolver** — habilitacao do condominio nos autos, regularizacao de area, ocupante identificado sem titulo definido | **Teto REBAIXADO** + a **condicao nomeada** + o **custo dela** + o que a resolve |
| **NO-GO** | **falta prova documental** · risco de anulacao **alto** · **a conta inverte de sinal** | **O motivo especifico** — nunca "nao recomendo" generico |

⛔ **Nao existe quarto veredito.** "Da para tentar", "parece bom" e "risco aceitavel" nao sao vereditos — se a duvida e real, ela e **GO-CONDICIONADO com a condicao escrita** ou **NO-GO com o motivo escrito**.

## ⭐ O que faz este parecer valer o preco
Os **8 SaaS concorrentes** cobram assinatura por dossie de lote e **nenhum deles**: analisa **risco de anulacao**, trata o **debito condominial** com a condicionante correta (edital informa x edital omisso) ou faz a **ponte para a peca**. Eles entregam **resposta binaria** — e erram nos **dois** sentidos. Aqui:
- **Cada afirmacao vem com a prova que a sustenta** e com o selo (✅ ancorado · 🟡 conferir antes de peca · 🔴 verdade dura ou pendente).
- **Onde a lei ou a jurisprudencia nao fecha, o parecer diz que nao fecha** — e diz o que conferir e onde. Isso e **diferencial de produto, nao fraqueza**.
- **O numero final e um teto de lance**, nao um "desconto". O desagio medio provado do mercado e **37,3%** — e ele encolhe, as vezes desaparece, depois de comissao, ITBI, emolumento pela maior base, carrego e desocupacao.

## Estrutura do parecer
1. **Identificacao do lote** — processo ou procedimento, matricula, praca ou leilao, datas, avaliacao e lance minimo.
2. **Status das 4 provas** — ✅ lida / ❌ faltando, com a data e a origem de cada documento.
3. **Achados por prova**, com a clausula, o ato de registro ou o documento **citado**.
4. **Risco de anulacao** — matriz de vetores com grau e o documento que prova cada um.
5. **A conta** — as 12 linhas com valor, fonte e selo.
6. ⭐ **VEREDITO** + **teto de lance** + **valor a lancar** + (se condicionado) **a condicao e seu custo**.
7. **O que fazer agora**, com prazo: obter prova faltante · impugnar comissao **antes do lance** · habilitar (`estrategia-de-lance-e-habilitacao`) · ou **nao lancar**.
8. **Ressalvas 🟡 nomeadas** e o roteamento ao `validador-leiloes`.

## Regras de ouro
- ⛔ **O onus de verificar e do arrematante, e isso tem base normativa** — **art. 18 da Res. CNJ 236/2016**. A clausula "sem garantia" **NAO e abusiva em si**: ataca-la e tese perdida. O parecer **assume esse onus com metodo**, em vez de reclamar dele.
- **Ressalva no rodape nao substitui veredito.** Prova faltante muda o **veredito**, nao o rodape.
- **Selo sem obrigacao ao lado nao entra.** Todo 🟡 escreve, na mesma frase, **o que falta, o que conferir e para onde rotear** — a regua dos quatro movimentos esta em `metodologia-leiloes.md` §8.
- **Precedente sempre com a qualificacao:** repetitivo x turma x **monocratica** x **pendente**. 🚫 Nunca "a materia esta em aberto no STJ" no condominio; nunca monocratica como repetitivo; nunca **REsp 2.171.564/SP** ou **Tema 1.266** como tese existente.
- **A trilha muda a linguagem, o entregavel e a ordem — NUNCA o corpus.** O investidor recebe **parecer e conta**; o advogado recebe **parecer, tese e a proxima peca**. Os dois leem a mesma lei.
- **Nunca** "leilao e seguro" · **nunca** "70% de desconto" · **nunca** "essa arrematacao nunca cai" · **nunca** "cai como qualquer negocio".
- ⏳ **Materia sensivel exige o gate de calendario** do `validador-leiloes` (EDcl nos EREsp 2.042.756/SP · REsp 2.171.564/SP · Tema 1.266) antes de fechar o parecer.

## Entrega obrigatoria final
O parecer completo nas **8 secoes**, com **veredito unico** (GO · GO-CONDICIONADO · NO-GO), **teto de lance e valor a lancar** (ou, sendo NO-GO, o **motivo especifico** e o plano de prova), todas as afirmacoes **seladas e ancoradas**, e o proximo passo **com prazo**. Validado por `suprema-corte-leiloes` + `validador-leiloes`, com `memoria-de-caso-leilao` atualizada.

## Guard
**Prova faltante = NO-GO por insuficiencia de prova.** Nenhuma afirmacao sobre o imovel sem **documento lido**. Nenhum veredito fora dos tres. Nenhum numero de aliquota de ITBI, emolumento fora de SP ou custas — formula e fonte. Nenhum 🟡 sem a obrigacao escrita ao lado. Nenhuma promessa de resultado. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
