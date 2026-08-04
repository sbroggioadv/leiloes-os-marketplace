---
name: adjudicacao-e-as-tres-remicoes
description: "A adjudicacao pelo exequente e pelos demais legitimados (arts. 876 a 878 do CPC), incluindo a SEGUNDA JANELA do art. 878 — frustrado o leilao, reabre-se a oportunidade de adjudicar, e com direito a pleitear NOVA AVALIACAO, dispositivo de alto valor e baixissimo uso — e as TRES REMICOES que nao podem ser confundidas: a da execucao (art. 826 do CPC), a do bem hipotecado no leilao (art. 902 do CPC) e a do bem hipotecado na adjudicacao (art. 877, §3º do CPC), cada uma com marco temporal e valor de resgate DIFERENTES. Carrega a armadilha do executado que acorda depois do pregao: acordo ou remicao posteriores a alienacao NAO afastam a comissao do leiloeiro. Use quando disserem quero adjudicar o bem, o leilao deu negativo e agora, posso pedir nova avaliacao, ainda da pra pagar e ficar com o imovel, ate quando o devedor pode remir, o acordo depois do leilao livra da comissao."
---

> **🖱️ Escolhas = botoes:** nas perguntas de lista fechada use **AskUserQuestion** (max. 4 por pergunta).

# ADJUDICACAO-E-AS-TRES-REMICOES

> Camada 3. Dois institutos que o mercado trata como um so — e nao sao. **Adjudicar e ficar com o bem; remir e pagar para que ele nao saia.** Confundi-los erra o marco temporal, o valor e a via.

## Anexos obrigatorios (context/)
- `context/cpc-leilao-879-903.md` — **876** (caput e §§1º-7º) · **877** (caput e §§1º-4º) · **878** (a segunda janela) · **902** · **826** · §16 (a tabela das tres remicoes) — **grep o artigo e leia a faixa**.
- `context/resolucao-cnj-236-2016.md` — **art. 7º**, com atencao ao **§3º** (acordo ou remicao **apos** a alienacao) e ao **§1º** (quando a comissao **nao** e devida) — **grep + ler a faixa**.
- `context/jurisprudencia-leiloes.md` — **REsp 2.198.525** (remicao posterior ao lance e comissao) — **grep + ler a faixa**.

## Pergunta de abertura (botoes)
**O que voce quer fazer?** ⟶ *adjudicar o bem* · *remir a execucao (pagar a divida)* · *remir o bem hipotecado* · *entender se ainda da tempo*. As quatro respostas levam a marcos e valores diferentes — e a escolha errada perde a janela.

## Objetivo
Dizer **qual instituto cabe**, **ate quando** e **por qual valor**, com o dispositivo nomeado — e, no caso da adjudicacao, se a **segunda janela do art. 878 do CPC** esta aberta.

## Metodologia
1. **Separar adjudicacao de remicao.** Sao finalidades opostas: uma **adquire**, a outra **impede a aquisicao**.
2. **Localizar o marco temporal** do instituto escolhido — todos sao preclusivos.
3. **Calcular o valor de resgate** pela regra propria daquele instituto, nunca pela de outro.
4. **Conferir a legitimidade** (a lista do CPC 876, §5º e §§6º-7º) e as intimacoes do CPC 876, §1º.
5. **Checar o impacto na comissao** do leiloeiro. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## Adjudicacao — arts. 876 a 878 do CPC

| Ponto | Regra |
|---|---|
| **Quem** | O **exequente**, oferecendo preco **nao inferior ao da avaliacao** (876, caput) |
| **Quem mais** | **§5º**: os indicados no **art. 889, incisos II a VIII** · os **credores concorrentes que penhoraram o mesmo bem** · **conjuge, companheiro, descendentes e ascendentes** do executado |
| **Intimacao do executado** | **§1º**: pelo Diario da Justica na pessoa do advogado (I) · **carta com AR** quando representado pela Defensoria ou sem procurador (II) · **meio eletronico** no caso do §1º do art. 246, sem procurador (III). **§2º**: mudou de endereco sem comunicar ao juizo, considera-se intimado. **§3º**: citado por edital e sem procurador, a intimacao e **dispensavel** |
| **Diferenca de valores** | **§4º**: credito **menor** que os bens ⟶ o requerente **deposita de imediato a diferenca**, a disposicao do executado; credito **maior** ⟶ a execucao **prossegue pelo saldo** |
| **Mais de um pretendente** | **§6º**: **licitacao** entre eles; em **igualdade de oferta**, preferem conjuge, companheiro, descendente e ascendente, **nessa ordem** |
| **Quota social / S.A. fechada** | **§7º**: penhora em favor de exequente **alheio a sociedade** ⟶ a sociedade e intimada e fica **responsavel por informar aos socios**, assegurada a estes a preferencia |
| **Aperfeicoamento** | **877**: transcorridos **5 dias da ultima intimacao** e decididas as questoes, o juiz ordena a lavratura do auto. **§1º**: perfeita e acabada com a **lavratura e assinatura**, expedindo-se **carta de adjudicacao + mandado de imissao** (imovel) ou **ordem de entrega** (movel) |
| **Conteudo da carta** | **§2º**: descricao do imovel, remissao a **matricula e registros**, copia do auto e **prova de quitacao do imposto de transmissao** |

⭐⭐ **A segunda janela — art. 878 do CPC.** *Frustradas as tentativas de alienacao*, **reabre-se** a oportunidade de requerer a adjudicacao — **e nela tambem se pode pleitear NOVA AVALIACAO**. E o dispositivo de maior valor e menor uso do capitulo: o credor que nao adjudicou por achar o bem caro tem, apos o leilao negativo, **uma segunda chance com laudo novo**.

🟡 **A adjudicacao NAO tem a mecanica de invalidacao do art. 903 do CPC**, que esta redigida para a **arrematacao**. **Nao transportar os 10 dias** para ela sem fundamentar — marcar *"conferir antes de protocolar"* e rotear ao `validador-leiloes`.

## ⭐ AS TRES REMICOES — marcos e valores DIFERENTES

| Remicao | Dispositivo | Ate quando | Quanto se paga |
|---|---|---|---|
| **Da EXECUCAO** | **CPC 826** | **A todo tempo**, antes de **adjudicados ou alienados** os bens | A **divida atualizada** + **juros, custas e honorarios advocaticios** |
| **Do BEM HIPOTECADO no leilao** | **CPC 902** | Ate a **assinatura do AUTO DE ARREMATACAO** | Preco **igual ao MAIOR LANCE** oferecido |
| **Do BEM HIPOTECADO na adjudicacao** | **CPC 877, §3º** | Ate a **assinatura do AUTO DE ADJUDICACAO** | **AVALIACAO**, se **nao houve licitantes**; havendo, o **maior lance** |

🔴 **Misturar os tres erra o calculo e a via.** Quem remir "a execucao" pensando que basta cobrir o maior lance paga menos do que deve e nao remi nada; quem for remir o bem hipotecado calculando a divida inteira paga a mais.

⚠️ **Quem remi o bem hipotecado e o EXECUTADO** (arts. 902 e 877, §3º do CPC). Em **falencia ou insolvencia do devedor hipotecario**, o direito passa **a massa ou aos credores em concurso**, e o **exequente nao pode recusar o preco da avaliacao** (CPC 902, §unico e 877, §4º).

⛔ **Remicao nao e purga.** A **purga da mora do extrajudicial** (**Lei 9.514, art. 26-A, §2º** — vai **ate a averbacao** da consolidacao) e instituto **diverso**, em procedimento diverso. Ponteiro para a camada extrajudicial — **nao duplicar aqui**.

## ⚠️ A armadilha do executado que "acordou depois do leilao"
**Acordo ou remicao POSTERIORES a realizacao da alienacao NAO afastam a comissao do leiloeiro** — **Res. CNJ 236/2016, art. 7º, §3º**, literal. O **§1º** so afasta a comissao na desistencia do art. 775 do CPC, na **anulacao** e no **resultado negativo**.

✅🔴 **Reforco jurisprudencial, com a qualificacao junto:** **REsp 2.198.525**, **3a Turma, unanime**, Rel. Min. Ricardo Villas Boas Cueva, noticia institucional do STJ de **17/07/2026** — a arrematacao **ja existe** com a aceitacao do lance e o deposito do preco, e a remicao feita **antes da assinatura do auto** nao retira a comissao, *"desde que seu trabalho tenha sido concluido com resultado util"*. Reconheceu tambem a **legitimidade do leiloeiro para recorrer como terceiro prejudicado** (CPC 996).
🟡 **Ressalvas obrigatorias:** e **acordao de turma, nao repetitivo** — nao vincula; a fonte e a **noticia institucional** e o **inteiro teor nao foi aberto**; o criterio e "trabalho concluido com **resultado util**", que **nao alcanca leilao negativo nem acordo ANTERIOR ao pregao**; e **nao foi localizada** decisao que declare a comissao indevida em acordo celebrado **antes** do leilao. Conferir antes de protocolar ⟶ `validador-leiloes`.

## Regras de ouro
- **Marco temporal e preclusivo e nao se estica por equidade.** Passada a assinatura do auto, a remicao daquele bem acabou.
- **O art. 876, §5º nao inclui qualquer terceiro.** A lista e fechada e remete ao **art. 889, incisos II a VIII** — o **inciso I (o executado)** ficou de fora dela.
- ⛔ **Nao confundir a preferencia do CPC 876, §6º e do CPC 892, §2º (so em IGUALDADE DE OFERTA) com o direito de preferencia do fiduciante da Lei 9.514, art. 27, §2º-B** — institutos distintos, procedimentos distintos.
- **A carta de adjudicacao tambem exige o imposto de transmissao quitado** (CPC 877, §2º) — mesma inversao de sequencia da arrematacao. Ver `arrematacao-auto-e-carta`.
- ⭐ **Para o arrematante, a segunda janela do art. 878 e informacao de risco:** um leilao negativo **nao significa** que o bem esta livre para a proxima praca — pode ser adjudicado antes, e com nova avaliacao.
- **Precedente entra com a qualificacao junto:** turma nao e repetitivo, noticia institucional nao e inteiro teor.
- Cross-link soft: mecanica geral em `mecanica-do-leilao-judicial` · relogio da arrematacao em `invalidacao-embargos-e-desistencia-903` · purga e defesa do fiduciante na camada extrajudicial · comissao e prestacao de contas na camada do leiloeiro.

## Entrega obrigatoria final
(a) **Instituto aplicavel** nomeado por artigo e diploma; (b) **marco temporal** com a data-limite calculada e o documento que a fixa; (c) **valor de resgate** pela regra propria, memoria de calculo aberta; (d) **legitimidade** conferida e intimacoes do CPC 876, §1º checadas; (e) estado da **segunda janela do art. 878**, se houve leilao frustrado; (f) **impacto na comissao**, com a ressalva 🟡 do precedente; (g) o que ficou **pendente de documento**. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Nunca tratar as **tres remicoes** como uma so — marcos e valores sao **diferentes**. Nunca chamar de **purga** a remicao judicial. Nunca aplicar o prazo de **10 dias do art. 903 do CPC** a adjudicacao sem ressalva. Nunca afirmar que acordo ou remicao **posteriores** a alienacao dispensam a comissao — a **Res. CNJ 236/2016, art. 7º, §3º** diz o oposto. Nunca citar o **REsp 2.198.525** como repetitivo ou como tese vinculante. Nunca ampliar a lista de legitimados do **CPC 876, §5º**. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
