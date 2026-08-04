---
name: saldo-remanescente-e-quitacao
description: "Responde a pergunta que decide a vida financeira do devedor depois do leilao: perdi o imovel E continuo devendo? A resposta virou de lado em 31/10/2023 e o mercado repete a antiga. Fora do art. 26-A da Lei 9.514, o §5º-A do art. 27 da mesma lei manteve o devedor OBRIGADO pelo saldo, cobravel por execucao e com excussao das demais garantias — e o §6º, que dava termo de quitacao, foi REVOGADO. Dentro do art. 26-A (financiamento para aquisicao ou construcao de imovel residencial do devedor, exceto consorcio) a divida e EXTINTA com reciproca quitacao pelo §4º, e o §5º qualifica isso como condicao resolutiva inerente a divida, que alcanca tambem a via JUDICIAL: o credor nao escapa migrando de via. Traz o calculo do §6º-A, a exoneracao do art. 9º, §10 da Lei 14.711 (afasta o art. 1.430 do Codigo Civil) e o intertemporal 🟡 dos contratos anteriores a 31/10/2023. Use quando cobrarem saldo apos leilao, e quando disserem perdi o imovel e ainda me cobram, sobrou divida, leilao negativo quita tudo."
---

> **🖱️ Escolhas = botoes:** nas perguntas de lista fechada use **AskUserQuestion** (max. 4 por pergunta).

# SALDO-REMANESCENTE-E-QUITACAO

> Camada 6. **A inversao de 2023.** "Leilao negativo quita a divida" era verdade e **deixou de ser regra**. Hoje a resposta depende de **um enquadramento** — e errar esse enquadramento e a diferenca entre encerrar o caso e responder a uma execucao.

## Anexos obrigatorios (context/)
- `context/lei-9514-consolidada.md` — **art. 27** (§§2º, 3º I-III, **4º**, **5º**, **5º-A**, **6º REVOGADO**, **6º-A**, 8º) · **art. 26-A** (§§3º, **4º**, **5º**) — **grep o artigo e leia a faixa**.
- `context/lei-14711-2023.md` — **art. 9º, §§7º, 8º, 9º e §10** (exoneracao no residencial, afastando o art. 1.430 do CC) · **§5.2** (o **art. 1.430 do Codigo Civil** verbatim) · **art. 18** (revogacoes) — **grep + ler a faixa**.
- `context/metodologia-leiloes.md` — §6 verdade 4 (a inversao) e §10 (o relogio) — **grep + ler a faixa**.

## Objetivo
Dizer, com o dispositivo colado, **se ainda ha divida**, **de quanto** e **por que via** — e, quando houver quitacao, entregar a **defesa pronta contra a cobranca**, inclusive se o credor migrar para a execucao judicial.

## Metodologia
1. **Enquadramento (botoes):** *financiamento para aquisicao ou construcao de imovel RESIDENCIAL do devedor* · *outra alienacao fiduciaria de imovel* · *consorcio* · *hipoteca pelo art. 9º da Lei 14.711*. **Consorcio esta excluido** do art. 26-A por texto expresso.
2. **Datar o contrato** — anterior ou posterior a **31/10/2023**. E o eixo do intertemporal.
3. **Ler o resultado do 2º leilao:** houve lance no referencial minimo, houve lance abaixo aceito pelo credor, ou o leilao foi **negativo**?
4. **Aplicar a tabela** e, havendo saldo, **conferir o calculo do §6º-A** linha a linha.
5. **Se ha quitacao, escrever a defesa** — e antecipar a migracao para a via judicial (art. 26-A, §5º Lei 9.514).
6. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## ⭐⭐ A TABELA QUE DECIDE — enquadramento antes de qualquer conta

| Cenario | Regra | Resultado |
|---|---|---|
| **Fora** do art. 26-A da Lei 9.514, produto do leilao insuficiente | **art. 27, §5º-A** da Lei 9.514 | 🔴 **Devedor continua obrigado** pelo saldo, cobravel por **acao de execucao** e com **excussao das demais garantias** |
| **Dentro** do art. 26-A da Lei 9.514, 2º leilao sem lance no referencial do §3º | **art. 26-A, §4º** da Lei 9.514 | ⭐ **Divida EXTINTA, com reciproca quitacao**; o credor fica com a **livre disponibilidade** do imovel |
| Dentro do art. 26-A, e o credor tenta cobrar **na Justica** | **art. 26-A, §5º** da Lei 9.514 | ⭐⭐ A extincao e **condicao resolutiva inerente a divida** e **estende-se as hipoteses em que o credor preferiu a via JUDICIAL** |
| **Hipoteca** residencial pelo rito novo, produto insuficiente | **art. 9º, §10 da Lei 14.711** | ⭐ Devedor **exonerado** do saldo, e **nao se aplica o art. 1.430 do Codigo Civil** |
| Leilao com sobra | **art. 27, §4º** da Lei 9.514 (**5 dias**) · na hipoteca, **art. 9º, §8º da Lei 14.711** (**15 dias**) | A entrega da sobra **importa reciproca quitacao** |

⚠️ **O §6º do art. 27 da Lei 9.514 — o termo de quitacao em 5 dias — foi REVOGADO** pela Lei 14.711/2023, coerentemente com o §5º-A. **Peca que invoca o §6º cita texto morto.**

## 🔴 A REGRA GERAL, e onde cada lei a afasta
> **Codigo Civil, art. 1.430.** Quando, excutido o penhor, ou executada a hipoteca, o produto nao bastar para pagamento da divida e despesas judiciais, **continuara o devedor obrigado pessoalmente pelo restante**.

- **Replicada** para a alienacao fiduciaria **fora** do art. 26-A pelo **art. 27, §5º-A da Lei 9.514**.
- **Afastada** na hipoteca de **imovel residencial do devedor** (exceto consorcio) pelo **art. 9º, §10 da Lei 14.711**, que exonera o devedor **expressamente**.
- **Afastada** na alienacao fiduciaria residencial pelo **art. 26-A, §4º da Lei 9.514**.

⭐ **A simetria e o argumento:** duas leis diferentes, no mesmo ano, exoneram o devedor **residencial** e mantem o devedor **nao residencial**. **Enquadrar o imovel como residencial do devedor e o trabalho de maior valor desta skill** — e prova-se com documento: contrato, finalidade do credito, matricula, comprovante de residencia.

## ⭐ O CALCULO DO §6º-A — e ele reduz o saldo
> Na hipotese do §5º (2º leilao sem lance no referencial), **para efeito de calculo do saldo remanescente do §5º-A, deduz-se do valor atualizado da divida o valor correspondente ao REFERENCIAL MINIMO PARA ARREMATACAO do §2º**, incluidos encargos e despesas de cobranca.

**Consequencia pratica:** o credor que fica com o imovel **nao pode cobrar a divida inteira**. Ele deduz **o referencial minimo**, nao o valor que julgar do bem. **Conferir a memoria de calculo do credor contra o §6º-A e a defesa mais rapida desta skill** — e o item mais comum de cobranca a maior.

⚠️ **Ler o §3º do art. 27 da Lei 9.514 antes de aceitar qualquer conta:** o que e "divida" (I), "despesas" (II — **inclusive a comissao do leiloeiro**) e "encargos do imovel" (III) esta **definido em lei**. Item fora dessas tres definicoes **nao entra**.

## 🟡 O INTERTEMPORAL — declarado, nao resolvido
A **Lei 14.711/2023 nao traz regra de transicao** para o §5º-A. Contratos firmados **antes de 31/10/2023**, executados depois, ficam num vacuo: aplica-se a regra da data do contrato ou a da data do leilao? 🟡 **Nao ha resposta ancorada nesta captura.** O plugin **declara a questao** e sustenta, como **tese**, que a obrigacao pelo saldo e regra de **direito material do contrato** — e **nao afirma isso como certeza**. **Marcar, argumentar e rotear ao `validador-leiloes` antes de protocolar.** ⚠️ Nao dizer ao cliente que "a lei nova nao alcanca contrato antigo" como se fosse pacifico.

## Regras de ouro
- ⛔ **Nunca "leilao negativo sempre quita a divida".** Fora do art. 26-A da Lei 9.514 o §5º-A mantem o devedor obrigado. E hoje um problema de **direito intertemporal**, nao uma regra estavel.
- ⭐ **O art. 26-A, §5º Lei 9.514 e a peca de defesa mais subestimada do dominio:** o credor **nao escapa** do efeito extintivo migrando para a execucao judicial. Alegar na contestacao **com o dispositivo colado**.
- **A comissao do leiloeiro e DESPESA dedutivel no extrajudicial** (art. 27, §3º, II da Lei 9.514) — regime **oposto** ao judicial, onde o arrematante paga por fora (CPC, art. 901, §1º). **Nao transportar um regime para o outro.**
- ⚠️ **Nomear o diploma sempre:** os §§5º-A e 6º-A sao do **art. 27 da Lei 9.514**; o §10 e do **art. 9º da Lei 14.711**; o art. 1.430 e do **Codigo Civil**. Tres diplomas, tres numeracoes que colidem.
- **Encargos do imovel correm contra o fiduciante ate a IMISSAO** do fiduciario na posse (art. 27, §8º da Lei 9.514) — item recorrente de cobranca a maior.
- Cross-link soft: `defesa-fiduciante-consolidacao-e-purga` · `regime-do-imovel-residencial-26a` · `os-dois-leiloes-da-alienacao-fiduciaria` · `hipoteca-extrajudicial-14711` · `reparacao-por-leilao-irregular`.

## Entrega obrigatoria final
Parecer com: (a) **o enquadramento** e o documento que o prova; (b) a **data do contrato** e a consequencia intertemporal, com a ressalva 🟡; (c) o **resultado do 2º leilao**; (d) **ha ou nao saldo**, com o dispositivo colado; (e) havendo saldo, a **conferencia do calculo pelo §6º-A**, item a item, contra as definicoes do §3º; (f) havendo quitacao, a **defesa pronta**, inclusive contra a migracao para a via judicial (art. 26-A, §5º Lei 9.514); (g) o que falta de documento. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Nunca afirmar que **leilao negativo quita a divida** sem enquadrar o caso no art. 26-A da **Lei 9.514**. Nunca invocar o **§6º do art. 27 da Lei 9.514** — esta **REVOGADO**. Nunca aceitar conta de saldo sem aplicar o **§6º-A** e as definicoes do **§3º**. Nunca afirmar o intertemporal como pacifico — e 🟡. Nunca confundir o **art. 9º, §10 da Lei 14.711** com o **art. 27, §5º-A da Lei 9.514** nem com o **art. 1.430 do Codigo Civil**. Nunca transportar o regime da comissao entre judicial e extrajudicial. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
