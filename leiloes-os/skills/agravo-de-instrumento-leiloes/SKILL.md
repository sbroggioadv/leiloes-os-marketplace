---
name: agravo-de-instrumento-leiloes
description: "Agravo de instrumento no leilao judicial e extrajudicial — o recurso natural do dominio, porque quase tudo que decide dinheiro aqui e interlocutoria dentro da execucao: indeferimento de liminar na anulatoria, decisao sobre invalidacao, ineficacia ou resolucao nos proprios autos (CPC 903 §1º), imissao negada e arbitramento da comissao do leiloeiro. Carrega a chave que o rol taxativo esconde — na execucao o paragrafo unico do CPC 1.015 abre TODA interlocutoria ao agravo — e a legitimidade recursal do leiloeiro como terceiro prejudicado (CPC 996 · REsp 2.198.525, turma). Skill standalone: os requisitos estao escritos aqui, sem depender de outro plugin. Use ao dizer preciso agravar, cabe agravo disso, o juiz indeferiu a liminar, negaram a imissao, o juiz decidiu a invalidacao nos autos, o leiloeiro quer cobrar comissao, quero recorrer dessa decisao do leilao."
---

> **🖱️ Escolhas = botoes:** nas perguntas de lista fechada use **AskUserQuestion** (max. 4 por pergunta).

# AGRAVO-DE-INSTRUMENTO-LEILOES

> Camada 7. **Standalone** — modelado no civel, **sem dependencia dura** dele: os requisitos estao escritos **aqui**. Recebe de `anulatoria-de-arrematacao-judicial`, `anulatoria-de-leilao-extrajudicial`, `invalidacao-embargos-e-desistencia-903`, `imissao-na-posse-do-arrematante` e `leiloeiro-comissao-e-prestacao-de-contas`.

## Anexos obrigatorios (context/)
- `context/cpc-leilao-879-903.md` — **903** (§§1º a 6º, o relogio), **804** (ineficacia relativa), **884 §unico** (comissao sem percentual legal), **901 §§1º-2º** (carta e imissao), **886, VI** — **grep o artigo e leia a faixa**.
- `context/jurisprudencia-leiloes.md` — **§5** (REsp 2.198.525, legitimidade do leiloeiro) e a qualificacao de cada precedente — **grep + ler a faixa**.
- `context/metodologia-leiloes.md` — **§7.1** (homonimo de criterio: percentual so com a base colada) · **§8** (selos) · **§10** (o relogio) — **ler primeiro**.

## Objetivo
Produzir o agravo **com o cabimento provado na abertura** — porque no leilao o erro caro nao e a tese, e a **via**. Devolve peca fundamentada, com o capitulo recorrido delimitado e o pedido de efeito suspensivo justificado, fechada por `suprema-corte-leiloes` + `validador-leiloes`.

## 🔴 A faixa recursal do CPC NAO esta neste corpus — e como citar mesmo assim
`context/cpc-leilao-879-903.md` cobre **876-903 + 804 + 826 + 908 §1º**. Os artigos de **recurso** (996 · 1.009-1.044) **nao foram capturados** neste plugin, e o **AVISO 3 do proprio anexo** manda conferir na fonte oficial qualquer artigo do CPC **fora** daquela faixa antes de transcrever — a pagina compilada do Planalto exibe redacao revogada e vigente lado a lado.

**Regra desta camada, sem excecao:** cite o artigo **pelo numero e pelo conteudo**; **nao ponha entre aspas como se fosse verbatim conferido**; antes de protocolar, confira a redacao vigente na fonte oficial e roteie ao `validador-leiloes`. 🟡

## ⭐⭐ A chave do dominio: na execucao, o rol taxativo NAO limita
O leilao acontece **dentro da execucao ou do cumprimento de sentenca**. O **paragrafo unico do art. 1.015 do CPC** abre o agravo de instrumento contra **toda** decisao interlocutoria proferida no processo de execucao, na liquidacao e no cumprimento de sentenca — o rol do **caput** e taxativo **fora** dali, nao ali dentro.

> ⛔ **O erro que mata a peca:** procurar a decisao do leilao no rol do caput, nao achar, e concluir que "nao cabe agravo". Conclui-se errado, perde-se o prazo, e o que sobra e uma via pior. 🟡 Confira a redacao vigente do 1.015 e do seu paragrafo unico antes de protocolar.

## As quatro decisoes que este dominio agrava

| # | Decisao | Fundamento do cabimento | Cuidado proprio |
|---|---|---|---|
| **1** | **Liminar indeferida** na anulatoria de arrematacao (judicial) ou de leilao extrajudicial | Tutela provisoria — hipotese **do proprio rol** do CPC 1.015 (processo de conhecimento) | No extrajudicial, a Lei 9.514/97, art. 30, §unico, comprime a defesa: consolidada ou arrematada, **so a exigencia de notificacao obsta** a reintegracao. O agravo ataca a **notificacao**, nao o preco |
| **2** | Decisao do juiz sobre **invalidacao · ineficacia · resolucao** nos proprios autos | **CPC 903, §1º**, decidida na forma do §2º = interlocutoria **na execucao** → 1.015, §unico | O prazo de **10 dias do §2º** e para **PROVOCAR**, contado do **aperfeicoamento** (assinatura do auto) — **nao** e prazo recursal e o agravo **nao o ressuscita** |
| **3** | **Imissao negada** ou condicionada | Interlocutoria na execucao → 1.015, §unico | O **CPC 901, §1º** so manda expedir o mandado **depois** de pagos preco, comissao e despesas; o **§2º** exige **prova de pagamento do ITBI** na carta. Agravar antes de pagar e agravar sem razao |
| **4** | **Comissao do leiloeiro** arbitrada, negada ou reduzida | Interlocutoria na execucao → 1.015, §unico | O **CPC 884, §unico nao fixa percentual**. 5% e **PISO, nao teto, e nao existe teto** (RMS 65.084/SP · REsp 680.140/RS — turma). **7% em leilao JUDICIAL e licito** |

## ⚖️ Legitimidade recursal — quem pode agravar aqui ✅ 🔴
- **Partes** e o **arrematante** (que e parte no incidente que o atinge).
- ⭐ **O LEILOEIRO** tem legitimidade para recorrer como **terceiro prejudicado**, na forma do **CPC 996** — reconhecido no **REsp 2.198.525** (3ª Turma, julho/2026), no mesmo julgado que assentou que a **remicao posterior ao lance e anterior a assinatura do auto nao afasta a comissao**. 🔴 **Turma, nao repetitivo** — escreva *"o STJ decidiu, em acordao de turma"*, nunca "tese firmada".
- **Terceiro titular de direito real nao intimado** — o **CPC 804** lhe da **ineficacia**, nao nulidade: a alienacao nao o alcanca, e o gravame **nao foi purgado** perante ele.

## 🟡 O percentual que este corpus NAO tem — nao invente
A multa do **agravo interno** (CPC 1.021) incide sobre o **VALOR DA CAUSA** — base **diferente** dos percentuais deste dominio: **20% da avaliacao** (**CPC 896, §2º**, arrependimento no imovel de incapaz) · **ate 20% do valor atualizado do bem** (**CPC 903, §6º**, vicio infundado) · **lance** (comissao).

⛔ **A faixa percentual dessa multa NAO foi localizada neste corpus** — `metodologia-leiloes.md` §7.1 registra a ausencia expressamente. **Nao escreva o numero.** Diga que a sancao existe, **nomeie a base (valor da causa)**, e confira o percentual na fonte antes da peca → `validador-leiloes`.

## Metodologia
1. **Pergunta em botoes: qual decisao voce vai atacar?** — liminar indeferida · decisao do 903 nos autos · imissao negada · comissao. A resposta define o fundamento do cabimento e o cuidado da linha 3 da tabela.
2. **Provar o cabimento na abertura**, em um paragrafo: e interlocutoria? esta na execucao (1.015, §unico) ou no conhecimento (rol do caput)? **Peca que nao abre provando o cabimento e peca que convida a nao-conhecimento.**
3. **Conferir a tempestividade** — prazo em **dias uteis**; confira o termo inicial da intimacao e eventual prazo em dobro antes de assinar. 🟡 Nao afirme numero de dias sem conferir na fonte.
4. **Montar a instrucao**: copia da decisao agravada, da certidao de intimacao e das pecas que provam o alegado (edital, matricula, auto, comprovantes). No leilao, **o documento e a tese** — alegacao sem documento nao se sustenta e ainda expoe ao **§6º do 903** (ato atentatorio, ate 20% do valor atualizado do bem).
5. **Delimitar o capitulo recorrido** — o que nao for impugnado **nao devolve**. Em decisao que resolve varios pontos (invalidacao + comissao + imissao), nomeie **cada** capitulo atacado.
6. **Pedir efeito suspensivo ou tutela recursal com fundamento proprio** — ele **nao e automatico**. Probabilidade + perigo + **reversibilidade**; sem os tres, o pedido enfraquece o recurso inteiro. Detalhe em `tutela-de-urgencia-leiloes`.
7. **Selar cada precedente** com a qualificacao (repetitivo · turma · **monocratica** · **pendente**) e fechar por `suprema-corte-leiloes` (R1-R4) + `validador-leiloes`.

## Regras de ouro
- ⛔ **Nao existe agravo que devolva prazo perdido.** Passados os 10 dias do **CPC 903, §2º** sem alegacao, expede-se a carta e a via nos autos **se fecha**: resta **acao autonoma** (§4º), com o arrematante como **litisconsorte necessario**. Prometer o contrario e vender derrota.
- ⛔ **Nunca "a arrematacao nunca cai"** nem **"cai como qualquer negocio"**. O caput do 903 a mantem **ainda que procedentes** os embargos ou a acao autonoma, resolvendo-se em reparacao — e o §1º ainda assim admite invalidacao.
- **Precedente sempre com a qualificacao.** 🚫 Nunca **REsp 2.165.101** como "tese firmada" (e **monocratica** — a redacao e *"o STJ vem anulando"*). 🚫 Nunca **REsp 2.171.564/SP** ou **Tema 1.266** como tese existente. 🚫 Nunca **"a materia esta em aberto no STJ"** no debito condominial.
- **Percentual so com a base colada ao numero** (`metodologia-leiloes.md` §7.1): 20% da **avaliacao** (**CPC 896, §2º**) ≠ ate 20% do **valor atualizado** (**CPC 903, §6º**) ≠ 20% do **lance**; comissao incide sobre o **valor da arrematacao**; multa de agravo interno sobre o **valor da causa** — **sem numero neste corpus**.
- **Nunca dar numero** de aliquota de ITBI, emolumento fora de SP ou custas — apenas a formula e a fonte a consultar.
- **A trilha muda a linguagem, nunca o corpus**: 💰 o investidor recebe o efeito pratico e o custo; 🎓 o advogado recebe a peca e a tese.

## Entrega obrigatoria final
Agravo completo com: (a) **paragrafo de cabimento** nomeando o fundamento (rol do caput **ou** 1.015, §unico na execucao); (b) tempestividade **conferida**; (c) lista das pecas que instruem; (d) **capitulos recorridos nomeados um a um**; (e) fundamentacao com cada precedente **selado e qualificado**; (f) pedido de efeito suspensivo ou tutela recursal **fundamentado nos tres requisitos**; (g) pedido final; (h) **ressalvas 🟡 nomeadas** — a faixa recursal nao capturada e o percentual do agravo interno — com o roteamento. Validado por `suprema-corte-leiloes` + `validador-leiloes`, com `memoria-de-caso-leilao` atualizada.

## Guard
Nenhuma citacao de artigo **fora** da faixa 876-908 do CPC entra entre aspas como verbatim conferido. Nenhum percentual sem a **base colada**, e **nenhum numero** para a multa do agravo interno. Nenhum precedente sem qualificacao. Nenhuma alegacao de vicio **sem documento** — o §6º do art. 903 pune com ate 20% do valor atualizado do bem. Nunca prometer resultado, nunca "leilao e seguro". Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
