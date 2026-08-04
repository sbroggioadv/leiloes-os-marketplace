---
name: anulatoria-de-arrematacao-judicial
description: "Redige a acao autonoma do art. 903, §4º do CPC contra arrematacao judicial ja consumada, com o arrematante como LITISCONSORTE NECESSARIO — e antes disso faz a escolha que decide a peca: invalidacao, ineficacia ou resolucao. Sao tres pedidos distintos no §1º, e pedir nulidade onde o art. 804 do CPC da INEFICACIA e pedir a coisa errada: o leilao fica de pe e o efeito e relativo apenas a quem nao foi intimado. Fixa a posicao no relogio (10 dias do aperfeicoamento para a via incidental nos autos; depois da carta, so acao autonoma) e carrega o freio do §6º: suscitacao infundada de vicio e ato atentatorio, com multa de ate 20% do valor atualizado do bem. Use quando o executado, o coproprietario ou o titular de direito real quiser desfazer arrematacao judicial, e quando disserem quero anular o leilao, perdi meu imovel no leilao, nao fui intimado, arremataram por preco vil, ja saiu a carta e agora, o leilao foi irregular."
---

> **🖱️ Escolhas = botoes:** nas perguntas de lista fechada use **AskUserQuestion** (max. 4 por pergunta).

# ANULATORIA-DE-ARREMATACAO-JUDICIAL

> Camada 6. **Defesa do executado.** O produto desta skill **nao e a peca — e a escolha do pedido.** Tres destinos convivem no art. 903, §1º do CPC e **nao sao sinonimos**: pedir o errado entrega vitoria formal com resultado zero.

## Anexos obrigatorios (context/)
- `context/cpc-leilao-879-903.md` — **903 integral** (§1º I-III · §2º · §4º · §5º · §6º) · **804** (os **6 §§**, quem tem legitimidade) · **889** (as 8 categorias) · **891 §unico** · **890** — **grep o artigo e leia a faixa**.
- `context/jurisprudencia-leiloes.md` — §8 (a consequencia correta da falta de intimacao) · §6 (preco vil) · §11 (o bloco 🟡, inclusive **REsp 1.862.902/SP**) — **grep + ler a faixa**.
- `context/metodologia-leiloes.md` — **§7.1** (homonimo de criterio: os tres "20%" tem **bases diferentes**) — **grep + ler a faixa**.

## Objetivo
Devolver a **peca certa**: pedido nomeado (invalidacao / ineficacia / resolucao), causa de pedir ancorada em **documento lido**, polo passivo completo com o **arrematante como litisconsorte necessario**, e a via correta para a **fase em que o caso esta**.

## Metodologia
1. **Fixar a fase (botoes):** *dentro dos 10 dias do aperfeicoamento* · *carta ja expedida* · *nao sei a data do auto*. "Nao sei" nao e resposta — e **documento faltante**, e a peca para ate ter a data.
2. **Escolher o pedido** pela tabela abaixo. **Este passo e o produto.**
3. **Provar cada vicio com documento** — auto, edital, matricula, certidao de intimacao, laudo de avaliacao.
4. **Montar o polo passivo:** exequente, executado e, na acao autonoma, **o arrematante (§4º)**.
5. **Medir o freio do §6º** antes de assinar (bloco abaixo).
6. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## ⭐⭐ AS TRES SAIDAS DO §1º — pedir a errada e perder ganhando

| Pedido | Hipotese legal | O que acontece com o leilao | Quem tem legitimidade |
|---|---|---|---|
| **Invalidacao** (I) | **preco vil ou outro vicio** | O leilao **cai** — desfaz-se a aquisicao | executado e quem sofreu o vicio |
| **Ineficacia** (II) | inobservancia do **art. 804 do CPC** | 🔴 O leilao **FICA DE PE**; e ineficaz **so perante quem nao foi intimado** | **os 6 §§ do art. 804** — bloco abaixo |
| **Resolucao** (III) | **preco nao pago** ou caucao nao prestada | Desfaz-se por **inadimplemento do arrematante** | exequente e executado |

### 🔴 INEFICACIA ≠ NULIDADE — o erro que mais custa nesta camada
Peca que pede **"nulidade"** onde o **art. 804 do CPC** da **"ineficacia"** **pede a coisa errada**. O efeito e **relativo**: o bem **continua arrematado** e o **gravame nao foi purgado** perante o titular nao intimado. Para o credor com garantia registrada isso costuma ser **melhor** que anular — ele mantem o gravame sobre imovel agora nas maos de um terceiro solvente. Para o **executado**, ao contrario, a ineficacia **nao devolve o imovel**: se o objetivo e recuperar o bem, o pedido e **invalidacao (I)**, nao ineficacia.

⭐ **Os 6 §§ do art. 804 do CPC sao o MAPA DA LEGITIMIDADE** — cada um nomeia quem pode alegar: caput credor pignoraticio, hipotecario ou anticretico · **§1º** promitente comprador ou cessionario de cessao registrada · **§2º** concedente ou concessionario de **direito de superficie** · **§3º** promitente vendedor, promitente cedente ou **proprietario fiduciario** · **§4º** enfiteuta ou concessionario (CUEM/CDRU) · **§5º** proprietario do imovel quando alienado o direito do enfiteuta ou concessionario · **§6º** titular de **usufruto, uso ou habitacao**. **Ler os 6 antes de definir o autor** — errar o §  e errar a parte.

⚠️ A ineficacia do 804 **nao depende de demonstracao de prejuizo**. 🟡 Se vale ou nao *pas de nullite sans grief* no leilao judicial **nao esta resolvido**: ha so snippets de busca, **nenhum acordao aberto**, e tensao real com a linha do extrajudicial. **Nao presumir o recorte** — marcar e rotear ao `validador-leiloes`.

## ⏰ O relogio decide a VIA, e ele e irreversivel
- **Ate 10 dias do APERFEICOAMENTO** (assinatura do auto, **nunca** da ciencia do vicio — CPC 903, §2º): tudo **incidental nos autos**.
- **Passados os 10 dias sem alegacao:** expede-se carta + mandado de imissao (§3º) e **a via nos autos se fecha**.
- **Depois da carta:** **so acao autonoma** (§4º), e nela **o arrematante e litisconsorte necessario** — peca que nao o inclui e **inepta por defeito de polo**.
- ⚠️ **O caput e forte:** a arrematacao segue **perfeita, acabada e irretratavel** *ainda que julgados procedentes* os embargos ou a acao autonoma, resolvendo-se em **reparacao**. **Nao prometer devolucao do imovel como resultado natural.**

## 🔴 O FREIO DO §6º — a regra de ouro desta camada inteira
Suscitacao **infundada** de vicio para ensejar a desistencia do arrematante e **ato atentatorio a dignidade da justica**: multa de **ate 20% do VALOR ATUALIZADO DO BEM** (base colada — nao e sobre o lance, e nao e a caucao de 20% do edital). **Achado sem documento nao vira alegacao.** Vicio suspeitado entra na peca como **pedido de exibicao ou diligencia**, nunca como afirmacao.

## Regras de ouro
- **Um pedido por vicio, nomeado.** Cumular invalidacao e ineficacia sem separar causa de pedir confunde o juizo e derruba os dois.
- **Preco vil no judicial e cascata do CPC 891, §unico** — havendo preco minimo no edital, vil e o **abaixo dele**; **so na falta** valem os **50% da avaliacao**. ⛔ Nunca "o CPC fixa 50%". Regime completo em `preco-vil-como-tese`.
- **O art. 889 do CPC tem 8 categorias fechadas e o conjuge NAO e uma delas.** Alegar nulidade por falta de intimacao do conjuge cita o dispositivo errado. Detalhe em `nulidades-de-intimacao-e-notificacao`.
- 🟡 **REsp 1.862.902/SP veio de fonte secundaria, sem inteiro teor aberto** — **conferir antes de citar em peca**.
- **Nao transportar vetor do extrajudicial para ca.** O art. 30, §unico da **Lei 9.514** nao rege leilao judicial; a compressao da defesa e de la, nao daqui.
- Cross-link soft: espelho de risco em `risco-de-anulacao-do-certame` · via incidental em `invalidacao-embargos-e-desistencia-903` · o extrajudicial em `anulatoria-de-leilao-extrajudicial` · danos em `reparacao-por-leilao-irregular`.

## Entrega obrigatoria final
Peca com: (a) **fase e data do auto** declaradas logo no inicio; (b) **pedido nomeado** entre invalidacao, ineficacia e resolucao, com o dispositivo colado; (c) causa de pedir com **o documento que prova cada vicio**; (d) polo passivo completo, com o **arrematante nomeado litisconsorte necessario** quando §4º; (e) na ineficacia, **o § do art. 804 do CPC** que da a legitimidade; (f) o que ficou **pendente de documento**. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Nunca chamar de **nulidade** a falta de intimacao de titular de direito real — e **ineficacia do art. 804 do CPC**, e o leilao fica de pe. Nunca ajuizar a acao do §4º **sem o arrematante no polo passivo**. Nunca contar os 10 dias da **ciencia do vicio**. Nunca alegar vicio **sem documento** — §6º, ate **20% do valor atualizado do bem**. Nunca "o CPC fixa 50%". Nunca prometer que a arrematacao cai. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
