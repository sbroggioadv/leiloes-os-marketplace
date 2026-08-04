---
name: arrematacao-parcelada-895
description: "A via alavancada do investidor pelo art. 895 do CPC — proposta escrita de aquisicao em prestacoes, com no minimo 25% do lance a vista e o saldo em ate 30 meses, garantido por hipoteca do proprio imovel — e os seus TRES VENENOS, que quase nenhum material de mercado conta: qualquer lance a VISTA sempre prevalece sobre a proposta parcelada (§7º), a proposta NAO suspende o leilao e portanto nao reserva o bem (§6º), e a multa de 10% por atraso incide sobre a parcela inadimplida SOMADA AS VINCENDAS (§4º), nao sobre a parcela isolada. Roda so depois do gate de due diligence, e recusa operar sem ele. Use quando disserem quero parcelar a arrematacao, posso comprar em leilao financiado, como funciona a proposta parcelada, minha proposta segura o imovel, e se eu atrasar uma parcela, quanto preciso de entrada, ate quando posso apresentar a proposta."
---

> **🖱️ Escolhas = botoes:** nas perguntas de lista fechada use **AskUserQuestion** (max. 4 por pergunta).

# ARREMATACAO-PARCELADA-895

> Camada 3. A unica via de alavancagem que o CPC oferece ao arrematante — e a que mais gera frustracao, porque **nao reserva nada**. Quem entende os tres venenos antes de montar a operacao economiza o preco de aprender depois.

## ⛔ Esta skill depende do GATE — e recusa operar sem ele
Skill de **lance e aquisicao** nao roda sem as **4 provas documentais**: **[1] edital lido** (`analise-de-edital`) · **[2] matricula lida** (`leitura-de-matricula`) · **[3] ocupacao apurada** (`situacao-possessoria`) · **[4] debitos levantados** (`debitos-propter-rem`), mais `risco-de-anulacao-do-certame` e `custo-total-real-e-precificacao`. Faltando qualquer uma, o caminho e **NO-GO por insuficiencia de prova** pelo `parecer-go-nogo-lote` — **nunca** "provavelmente esta ok". O motivo e textual e nao pedagogico: os **10 dias do art. 903, §2º do CPC** correm do **aperfeicoamento**, entao due diligence feita depois do lance chega tarde **por construcao da lei**.

## Anexos obrigatorios (context/)
- `context/cpc-leilao-879-903.md` — **895 integral** (caput, incisos I-II e §§1º-9º) · **891 §unico** (o que e vil) · **885** · **901, §1º** · **897** — **grep o artigo e leia a faixa**.
- `context/custo-total-do-arrematante.md` — §1 (formula do teto de lance) e §2 (comissao por fora) — **grep + ler a faixa**.
- `context/metodologia-leiloes.md` — **§7.1** (os percentuais e suas bases de calculo) — **grep + ler a faixa**.
- `context/clausulas-armadilha-de-edital.md` — ARM-12 (pagamento em 24 h) e ARM-11 (multa de desistencia) — **grep + ler a faixa**.

## Pergunta de abertura (botoes)
**Em que momento voce esta?** ⟶ *antes do 1º leilao* · *entre o 1º e o 2º leilao* · *proposta ja apresentada* · *ja arrematei parcelado e atrasei*. O momento define **o valor minimo da proposta** e o que ainda e possivel.

## Objetivo
Montar a **proposta escrita** com os elementos que a lei exige, dizer **qual e o piso de valor** naquele momento, e — antes de tudo — **declarar em voz alta os tres venenos**, para que a decisao seja consciente.

## Metodologia
1. **Confirmar o gate completo.** Sem as 4 provas, parar.
2. **Fixar o momento** e, com ele, o **piso do valor** (tabela abaixo).
3. **Montar a proposta** com os 5 elementos obrigatorios do §2º e do §1º.
4. **Simular o pior cenario**: lance a vista aparece · atraso de uma parcela · concorrencia de outra proposta parcelada.
5. **Cruzar com o teto de lance** do `custo-total-real-e-precificacao` — parcelar **nao reduz** comissao, ITBI, emolumentos nem carrego.
6. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## O piso do valor muda com o momento (art. 895, I e II do CPC)

| Momento | Ate quando | Valor minimo da proposta |
|---|---|---|
| **1º leilao** | **Ate o inicio** do primeiro leilao | **Nao inferior ao da AVALIACAO** |
| **2º leilao** | **Ate o inicio** do segundo leilao | Valor que **nao seja considerado vil** |

⭐ **E aqui — e so aqui — que a diferenca entre pracas aparece na lei.** A regua do **preco vil** (CPC 891, §unico) **nao separa pracas**; o que muda entre elas e este **preco de aceitacao da proposta parcelada**. O que e "vil" segue a **cascata**: havendo preco minimo no edital (**CPC 885**), vil e o que fica abaixo dele; so na ausencia valem os **50% da avaliacao**.

## A estrutura obrigatoria da proposta

| Elemento | Exigencia | Base |
|---|---|---|
| **Forma** | **Por escrito** | caput |
| **Entrada** | **No minimo 25% do valor do LANCE, a vista** | §1º |
| **Saldo** | Parcelado em **ate 30 meses** | §1º |
| **Garantia** | **Hipoteca do proprio bem** (imoveis) · **caucao idonea** (moveis) | §1º |
| **Conteudo** | **Prazo · modalidade · indexador de correcao monetaria · condicoes de pagamento do saldo** | §2º |

⚠️ **O §3º foi VETADO** — nao existe conteudo a citar ali. Material que "cita o §3º do art. 895" esta inventando dispositivo.

## 🔴 OS TRES VENENOS — dizer antes, sempre

| § | O veneno | O que isso significa na pratica |
|---|---|---|
| **§7º** ⭐ | **A proposta de pagamento do lance a vista SEMPRE prevalece** sobre as propostas de pagamento parcelado | Por menor que seja a diferenca. Voce pode fazer toda a due diligence, montar a operacao e **perder para um lance a vista de valor igual ou proximo** |
| **§6º** | **A apresentacao da proposta NAO suspende o leilao** | Ela **nao reserva o bem** e nao segura o pregao. Nao ha "prioridade" por ter protocolado antes |
| **§4º** | Atraso em qualquer prestacao: **multa de 10% sobre a SOMA da parcela inadimplida COM AS PARCELAS VINCENDAS** | ⛔ **Nao e 10% da parcela.** A base e a parcela atrasada **mais tudo o que ainda vai vencer** — no inicio do contrato, a diferenca entre as duas leituras e de ordens de grandeza |

⚠️ **Homonimo de criterio — cada percentual sobre a SUA base, e elas nao se somam nem se comparam:** os **10%** incidem sobre **parcela inadimplida + vincendas** (§4º) · os **25%** sobre o **valor do LANCE** (§1º) · a **comissao do leiloeiro** sobre o **valor da ARREMATACAO** (**Res. CNJ 236/2016, art. 7º** — piso de 5%, sem teto) · a **caucao de 20%** de clausula de edital e **deposito, nao multa** (ARM-12). Num bem arrematado a 50% da avaliacao, um percentual "sobre a avaliacao" e o **dobro** do mesmo percentual "sobre o lance". **Percentual so entra no texto com a base colada** — `context/metodologia-leiloes.md` §7.1.

## Concorrencia e inadimplemento

- **Mais de uma proposta parcelada** (§8º): em **condicoes diferentes**, o juiz decide pela **mais vantajosa, assim compreendida SEMPRE a de MAIOR VALOR**; em **condicoes iguais**, pela **formulada em primeiro lugar**.
- **Inadimplemento** (§5º): autoriza o **exequente** a pedir a **resolucao da arrematacao** **ou** promover, contra o arrematante, a **execucao do valor devido** — ambos **nos autos da propria execucao** em que se deu a arrematacao. Nao ha acao nova, e nao ha foro diferente.
- **Destino dos pagamentos** (§9º): pertencem ao **exequente ate o limite do seu credito**; os subsequentes, ao **executado**.

## Regras de ouro
- **Parcelar nao barateia a aquisicao.** Comissao, ITBI, emolumentos, carrego e desocupacao continuam iguais — e a maioria vence **antes** da carta (**CPC 901, §§1º-2º**). Ver `arrematacao-auto-e-carta`.
- 🟡 **Ponto sem resposta na lei:** se a comissao do leiloeiro incide sobre o **lance total** ou sobre a **parcela a vista** — o **CPC nao diz**. Precificar com as **duas hipoteses**, escrever *"conferir antes de protocolar"* e rotear ao `validador-leiloes`.
- **Se a operacao depende de credito bancario, a proposta do art. 895 tem de ser protocolada ANTES** — editais reais exigem pagamento em **24 horas**, prazo em que financiamento nao roda.
- **A hipoteca e do proprio bem arrematado.** O imovel nasce gravado em favor da execucao: isso limita revenda e refinanciamento no prazo do parcelamento. Entra no plano de saida, nao como surpresa.
- **Nao pagar nao e "perder o sinal": e EXCLUSAO** (**CPC 897**) — perda da caucao e banimento daquele novo leilao.
- **Nunca prometer desconto.** O desagio medio provado do mercado e **37,3%**, nao 70%.
- Cross-link soft: teto de lance em `custo-total-real-e-precificacao` · habilitacao, prazos de cadastro e prorrogacao de 3 min / 15 s em `estrategia-de-lance-e-habilitacao` · veredito final em `parecer-go-nogo-lote`.

## Entrega obrigatoria final
(a) **Confirmacao do gate** com as 4 provas nomeadas — ou o **NO-GO por insuficiencia de prova**; (b) **momento e piso de valor** aplicavel; (c) **proposta escrita** com os 5 elementos do §1º e do §2º; (d) os **tres venenos declarados** no corpo, sem eufemismo; (e) **simulacao do §4º** com a base correta (parcela + vincendas); (f) o **custo total** que nao muda por parcelar; (g) o que ficou **pendente** (inclusive a 🟡 da comissao). Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Nunca dizer que a proposta **reserva** o bem ou **suspende** o leilao — o **§6º** diz o contrario. Nunca omitir que **lance a vista sempre prevalece** (**§7º**). Nunca calcular a multa do **§4º** sobre a parcela isolada: a base sao **parcela inadimplida + vincendas**. Nunca citar o **§3º** (VETADO). Nunca operar sem o **gate completo** — o motivo e o **CPC 903, §2º**. Nunca afirmar sobre qual base incide a comissao no parcelamento sem a ressalva 🟡. Percentual sem base colada nao entra no texto. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
