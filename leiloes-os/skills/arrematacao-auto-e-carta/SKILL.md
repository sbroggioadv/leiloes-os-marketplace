---
name: arrematacao-auto-e-carta
description: "A sequencia obrigatoria entre o lance e o titulo, pelo art. 901 do CPC: o auto e lavrado de IMEDIATO, mas a carta de arrematacao e o mandado de imissao so saem depois de depositado o preco (ou prestadas as garantias) MAIS a comissao do leiloeiro MAIS as demais despesas da execucao — e a carta ainda exige prova de pagamento do ITBI e a indicacao de eventual onus real ou gravame remanescente. Somada a trava do art. 903, §3º do CPC (a carta so e expedida passados os 10 dias sem alegacao), e a sequencia que drena o caixa do arrematante: ele paga TUDO antes de ter titulo e antes de ter posse. Separa os tres titulos que o mercado confunde — carta de arrematacao, carta de adjudicacao e carta de alienacao. Use quando disserem ja arrematei e agora, quando sai a carta, por que a carta nao foi expedida, tenho que pagar ITBI antes do registro, quando eu pego a chave, o que vem no auto de arrematacao."
---

> **🖱️ Escolhas = botoes:** nas perguntas de lista fechada use **AskUserQuestion** (max. 4 por pergunta).

# ARREMATACAO-AUTO-E-CARTA

> Camada 3. Entre o martelo e o titulo ha uma **sequencia com ordem fixa**. Quem a ignora nao perde o bem — trava o proprio caixa e descobre tarde que a chave vem por ultimo.

## Anexos obrigatorios (context/)
- `context/cpc-leilao-879-903.md` — **901** (caput e §§1º-2º) · **903, §3º** · **877, §§1º-2º** (carta de adjudicacao) · **880, §2º** (carta de alienacao) · **884** · **897** — **grep o artigo e leia a faixa**.
- `context/custo-total-do-arrematante.md` — §4 (ITBI e a **armadilha de sequencia**) e §5 (emolumentos pela **maior base**) — **grep + ler a faixa**.
- `context/resolucao-cnj-236-2016.md` — **art. 7º, §4º** (deducao da comissao do produto) e **art. 29** (remocao e transferencia por conta do arrematante) — **grep + ler a faixa**.
- `context/clausulas-armadilha-de-edital.md` — ARM-12 (pagamento em 24 h com caucao) e ARM-09/10 (comissao por fora) — **grep + ler a faixa**.

## Pergunta de abertura (botoes)
**Em que ponto da sequencia voce esta?** ⟶ *auto assinado, nada pago* · *preco depositado, faltam comissao/despesas* · *tudo pago, aguardando a carta* · *carta expedida, sem posse*. Cada ponto tem um proximo passo diferente — e um deles nao depende de voce.

## Objetivo
Dizer **o que falta para a carta sair**, **quanto ainda tem de ser desembolsado antes dela**, e **quando a posse entra** — separando o que depende do arrematante do que depende do juizo e do decurso do prazo.

## Metodologia
1. **Ler o auto**: data da assinatura, condicoes da alienacao e se abrange bens de mais de uma execucao.
2. **Montar a fila de pagamentos** na ordem do **CPC 901, §1º** e conferir cada comprovante.
3. **Checar a dupla condicao da carta** (pagamentos **e** decurso dos 10 dias do **CPC 903, §3º**).
4. **Conferir o conteudo obrigatorio da carta** (**CPC 901, §2º**) antes de aceita-la.
5. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## ⭐ A sequencia do art. 901 do CPC — ordem fixa, sem atalho

```
auto lavrado de IMEDIATO (caput)
   |
   +-- deposito do preco  OU  garantias prestadas
   +-- comissao do leiloeiro          <- por fora do lance
   +-- demais despesas da execucao
   |
   +-- prova de pagamento do ITBI     <- exigida pelo §2º na propria carta
          |
      CARTA de arrematacao (imovel)  ou  ORDEM DE ENTREGA (movel)
          |
      MANDADO de imissao na posse
```

⭐ **O §1º e a prova textual de que comissao e despesas NAO estao dentro do lance:** sao pagamento **adicional** e **condicao para a carta sair**. Um lance de R$ 1.000.000 custa **R$ 1.050.000** so de lance + comissao a 5%, antes de ITBI, emolumentos, carrego e desocupacao. Conta completa em `custo-total-real-e-precificacao`.

⭐ **O §2º inverte a sequencia tributaria:** a carta **contem** a prova de pagamento do imposto de transmissao — ou seja, **o ITBI e pago ANTES do titulo**, nao depois do registro. Quem planejou pagar o ITBI "depois, com o aluguel do imovel" **trava a propria carta**. Esta denuncia ja e feita na camada de due diligence: aqui ela e **herdada, nao reescrita**.

🟡 **Aliquota de ITBI varia por municipio e nao foi pesquisada. NUNCA dar o numero** — dar a **formula** (aliquota municipal x base da arrematacao) e mandar consultar a legislacao do municipio do imovel. Mesma disciplina para **emolumentos fora de SP** e **custas judiciais**.

## A trava que nao depende do arrematante — art. 903, §3º do CPC
Ainda que tudo esteja pago, **a carta so e expedida passado o prazo do §2º sem alegacao** de invalidacao, ineficacia ou resolucao. **Sao duas condicoes cumulativas**, e a segunda e o **decurso do tempo**. Relogio completo em `invalidacao-embargos-e-desistencia-903`.

⚠️ **E o §5º, II do art. 903 do CPC vive nessa janela:** se, **antes de expedida a carta**, o executado alegar alguma das situacoes do §1º, o arrematante **pode desistir** e receber o deposito de volta. A janela fecha com a carta.

## O que a carta OBRIGATORIAMENTE contem (art. 901, §2º do CPC)

| Item | Como conferir |
|---|---|
| **Descricao do imovel**, com remissao a **matricula ou individuacao** e aos **registros** | Confrontar com a matricula atualizada (`leitura-de-matricula`) — divergencia aqui reaparece no registro |
| **Copia do auto de arrematacao** | Conferir se as **condicoes da alienacao** descritas batem com o edital |
| **Prova de pagamento do imposto de transmissao** | Guia quitada; a base e o **valor alcancado em hasta** — 🟡 **turma, nao repetitivo**, e o **Tema 1.113 NAO e sobre arrematacao** |
| ⭐ **Indicacao da existencia de eventual onus real ou gravame** | **Carta que silencia sobre gravame conhecido e documento defeituoso.** Cruzar com a conferencia de intimacoes (`intimacoes-art-889-e-ineficacia`): gravame de credor **nao intimado** nao foi purgado perante ele — **ineficacia do art. 804 do CPC**, nao nulidade |

## Os TRES titulos que o mercado confunde

| Titulo | Base | Como se aperfeicoa |
|---|---|---|
| **Carta de arrematacao** | **CPC 901** | Auto de arrematacao assinado por juiz, arrematante e leiloeiro |
| **Carta de adjudicacao** | **CPC 877, §§1º-2º** | Auto de adjudicacao; a carta traz a **prova de quitacao do imposto de transmissao**. Regime em `adjudicacao-e-as-tres-remicoes` |
| **Carta de alienacao** | **CPC 880, §2º** | **Termo nos autos** na alienacao por iniciativa particular. 🟡 A mecanica do CPC 903 **nao se transporta** automaticamente para ela — marcar e rotear |

## Regras de ouro
- **A ordem nao se negocia.** Nao ha carta antes de preco + comissao + despesas, e nao ha mandado de imissao antes da carta. Pedir a chave antes disso e pedir fora da lei.
- **O prazo do edital e mais curto que a sequencia.** Editais reais exigem pagamento em **24 horas**, as vezes com **caucao de 20% do lance no ato** — e **financiamento bancario nao roda em 24 horas**. Recurso liquido confirmado **antes de habilitar** (ARM-11/ARM-12).
- **Nao pagar nao e "perder o sinal": e EXCLUSAO.** O **CPC 897** impoe a perda da caucao em favor do exequente **e bane o arrematante e o fiador remissos do novo leilao daquele bem**.
- **Comissao deduzida do produto e excecao, nao regra.** So quando o valor da arrematacao **supera o credito do exequente** (**Res. CNJ 236/2016, art. 7º, §4º**) — e a deducao e do **produto**, nao dispensa do arrematante.
- **Remocao, transferencia e guarda correm por conta do arrematante** (**Res. CNJ 236/2016, art. 29**) — entram na conta antes do lance, nao depois.
- 🔴 **Assimetria de desocupacao, contra o judicial:** o **CPC 901, §1º** **nao tem prazo nem qualificacao liminar**, e o mandado so sai ao fim da fila. No extrajudicial, a **Lei 9.514, art. 30** da **liminar expressa + 60 dias**. Detalhe em `imissao-na-posse-do-arrematante` — aqui e **ponteiro, nao duplicacao**.
- **Emolumentos de registro podem ser enquadrados por valor MAIOR que o lance.** Arrematar com 50% de desconto **nao corta o emolumento pela metade** — ver `custo-total-real-e-precificacao`.

## Entrega obrigatoria final
(a) **Posicao na sequencia**, com a data do auto; (b) **fila de pagamentos** com o que ja foi comprovado e o que falta; (c) **estado da dupla condicao** da carta (pagamentos e decurso dos 10 dias); (d) **conferencia dos 4 itens** obrigatorios da carta, com os defeitos apontados; (e) **previsao de posse** e a via da imissao; (f) o que ficou **pendente de documento**. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Nunca dizer que a comissao esta **dentro** do lance — o **CPC 901, §1º** prova o contrario. Nunca prometer carta ou posse **em data certa**: a expedicao depende tambem do **decurso** do prazo do **CPC 903, §3º**. Nunca **numero** de aliquota de ITBI, emolumento fora de SP ou custas — so a formula e a fonte. Nunca tratar a **base do ITBI** como tese repetitiva, nem citar o **Tema 1.113** como se fosse de arrematacao. Nunca confundir carta de **arrematacao**, de **adjudicacao** e de **alienacao**. Nunca aceitar carta que **omita gravame conhecido**. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
