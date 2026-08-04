---
name: outras-garantias-e-bens-extrajudiciais
description: "O que sobra fora do imovel: penhor, alienacao fiduciaria de bem MOVEL e veiculo apreendido. No penhor a regra e VENDA, nunca apropriacao — o art. 1.433, IV, do Codigo Civil da ao credor pignoraticio execucao judicial ou venda amigavel apenas se o contrato permitir ou o devedor autorizar por procuracao, e o art. 1.428 do Codigo Civil fulmina a clausula previa de ficar com o bem (pacto comissorio), ressalvada a dacao apos o vencimento. No bem movel o regime e OUTRO e ha decisao de 24/08/2025 dispensando a intimacao — aplicar a regra do imovel ao movel derruba a peca. O leilao de veiculo do art. 328 do CTB entra como PONTEIRO, com a desvinculacao automatica dos debitos e o alerta de que sucata nao volta a circular. Use quando a garantia nao for imovel, e quando disserem arrematei um carro de leilao, penhoraram minha joia, o banco ficou com o bem."
---

> **🖱️ Escolhas = botoes:** nas perguntas de lista fechada use **AskUserQuestion** (max. 4 por pergunta).

# OUTRAS-GARANTIAS-E-BENS-EXTRAJUDICIAIS

> Camada 4. **A borda do dominio.** Aqui o risco nao e errar a tese: e **importar a regra do imovel** para um bem que tem regime proprio. Esta skill existe para marcar as fronteiras e apontar para fora quando for o caso.

## Metodologia — primeira pergunta, em botoes
**Qual e a garantia ou o bem?** (penhor · alienacao fiduciaria de bem **movel** · **veiculo** apreendido pelo poder publico · leilao publico **administrativo** de bem da Administracao)

A ultima opcao e **gap declarado**: leilao publico administrativo esta **fora do escopo** deste plugin — reconhecer e encaminhar ao `licitacoes-adv-os`, **nunca improvisar**.

## Anexos obrigatorios (context/)
- `context/lei-14711-2023.md` — §5 do anexo (**Codigo Civil**: arts. 1.428, 1.430, 1.433 e 1.435 verbatim) e §6 (**art. 328 do CTB**, com o escopo declarado) — **grep + ler a faixa**.
- `context/lei-9514-consolidada.md` — art. 27, §5º-A, da Lei 9.514 (o saldo remanescente que replica a regra geral) — **grep + ler a faixa**.
- `context/jurisprudencia-leiloes.md` — §8, o recorte **imovel x movel** na intimacao — **grep + ler a faixa**.

## 1. PENHOR — venda, NUNCA apropriacao

| Dispositivo | O que trava |
|---|---|
| **Art. 1.433, IV, do Codigo Civil** ⭐ | O credor pignoraticio tem direito **"a promover a execucao judicial, ou a venda amigavel, se lhe permitir expressamente o contrato, ou lhe autorizar o devedor mediante procuracao"**. **Nao existe leilao extrajudicial de penhor por forca de lei geral** |
| **Art. 1.428 do Codigo Civil** ⭐ | E **NULA** a clausula que autoriza o credor **pignoraticio, anticretico ou hipotecario** a **ficar com** o objeto da garantia se a divida nao for paga no vencimento — o **pacto comissorio**. ⚠️ **Contrapeso do §unico:** **apos o vencimento**, o devedor **pode** dar a coisa em pagamento. Proibe-se a clausula **previa**, nao o acordo posterior |
| **Art. 1.435, V, do Codigo Civil** | O credor e obrigado **a entregar o que sobejar** do preco na hipoteca do art. 1.433, IV — trava adicional contra a apropriacao disfarcada |
| **Art. 1.430 do Codigo Civil** | Regra geral do saldo: excutido o penhor ou executada a hipoteca, **o devedor continua obrigado pessoalmente pelo restante** |

⭐ **O art. 1.430 do Codigo Civil e o eixo que o plugin cruza o tempo todo:**
- **afastado** no financiamento de imovel **residencial** pelo art. 9º, §10, da Lei 14.711/2023;
- **replicado** para a alienacao fiduciaria de imovel fora do regime residencial pelo art. 27, §5º-A, da Lei 9.514.

⚠️ **Nao confundir com apropriacao legal.** O art. 9º, §9º, I, da Lei 14.711/2023 permite ao credor hipotecario **apropriar-se do imovel apos dois leiloes negativos**, pelo minimo atualizado. **Isso nao e pacto comissorio** — e apropriacao **legal, posterior ao vencimento e a excussao**. Confundir os dois e erro **nos dois sentidos**: tanto validar clausula previa quanto atacar apropriacao licita.

## 2. ALIENACAO FIDUCIARIA DE BEM MOVEL — regime OUTRO
- ⚠️ **A exigencia de intimacao que sustenta metade da defesa do extrajudicial e de IMOVEL** (Lei 9.514). Ha **decisao de 24/08/2025 dispensando** a intimacao em leilao de bem **movel** com alienacao fiduciaria. 🟡 **Inteiro teor nao aberto** — afirmar a existencia da decisao, **nao** generalizar o alcance, e rotear ao `validador-leiloes` antes de peca.
- **Aplicar o regime do imovel ao movel derruba a causa**, e o inverso tambem: nao usar o afastamento da intimacao no movel para relativizar a exigencia no imovel.
- **A Lei 14.711/2023 tambem mexeu aqui:** o art. 18, III, revogou o art. 8º-A do Decreto-Lei 911/69. As **ADIs 7600/7601/7608** (Pleno, 30/06/2025) validaram os procedimentos extrajudiciais criados pela Lei 14.711/2023, **inclusive a consolidacao em alienacao fiduciaria de moveis e a busca e apreensao extrajudicial** — **com as balizas de conduta** (vedada perseguicao ao devedor e a familiares, **apenas dados publicos**, proibida forca fisica ou psicologica). 🟡 Citar **as balizas**, verificaveis — nao a "tese literal", que nao foi lida no acordao.
- **Fronteira:** o **contrato** de financiamento de veiculo (revisional, busca e apreensao judicial) e do `bancario-adv-os`; aqui so a **mecanica do leilao**.

## 3. VEICULO APREENDIDO — art. 328 do CTB, como PONTEIRO
⚠️ **Escopo declarado:** o leilao do art. 328 do CTB (Lei 9.503/97, redacao da Lei 13.160/2015) e **administrativo** — leilao publico administrativo esta **OUT** neste plugin. Entra como ponteiro por dois motivos: a fronteira com o arrematante de veiculo e real, e a regra de debitos e o paralelo veicular do que os tributos fazem no imovel.

**Os quatro pontos, e so estes:**
1. ✅ **60 dias** sem reclamacao pelo proprietario, contados do recolhimento ⇒ avaliacao e leilao, **preferencialmente eletronico** (caput).
2. ✅ **2º leilao: minimo de 50% do avaliado** (§2º) — **regua propria**, que **nao** se confunde com a cascata do preco vil do CPC nem com o referencial do art. 27, §2º, da Lei 9.514. Mais um "50%" com base diferente: **anote a base junto do numero**.
3. ✅ **Classificacao em conservado ou sucata** (§1º, I e II), e o veiculo levado **duas vezes** a leilao sem arrematacao **e releiloado como sucata** (§3º). 🔴 **Comprar sucata achando que vai regularizar e o erro mais caro do leilao de veiculos.**
4. 🟡 **Desvinculacao dos debitos anteriores — NAO CONFERIDA NO LITERAL.** O anexo afirma, em resumo, que o art. 328 do CTB desvincula automaticamente os debitos anteriores (§9º), **inclusive tributarios** (§10), com **reata** se o antigo proprietario reaver o veiculo (§11), e que a sucata nao volta a circular (§4º). **Esses paragrafos NAO estao capturados verbatim no corpus** — so o caput e os §§1º a 3º estao. Tratar como **resumo de segunda mao**: **conferir o texto do art. 328 do CTB na fonte antes de qualquer peca ou parecer de compra**, e rotear ao `validador-leiloes`.

**Fronteira:** o `transito-adv-os` e dono da defesa do **proprietario** contra remocao e leilao; `leiloes-os` atende o **arrematante**. Cross-link soft, sem duplicar.

## Regras de ouro
- **Identificar o bem antes da tese.** Imovel, movel, veiculo apreendido e bem da Administracao tem **quatro regimes**; a resposta certa no regime errado e resposta errada.
- **Percentual sempre com a base colada** — os "50%" deste dominio nao se comparam entre si (`context/metodologia-leiloes.md`, §7.1).
- **Nunca afirmar situacao do bem sem documento lido** — no veiculo isso significa laudo de classificacao, avaliacao e a consulta de debitos e restricoes.
- 🟡 **O que este plugin nao cobre, ele declara:** leilao publico administrativo e **gap**; a extensao da decisao de 24/08/2025 sobre bem movel **nao foi lida**; os paragrafos de debitos do art. 328 do CTB **nao estao no corpus**.
- Cross-link soft: `licitacoes-adv-os` (leilao administrativo) · `transito-adv-os` (defesa do proprietario do veiculo) · `bancario-adv-os` (o contrato) · `hipoteca-extrajudicial-14711` (a apropriacao legal do art. 9º, §9º, I) · `saldo-remanescente-e-quitacao` (o art. 1.430 do Codigo Civil no caso concreto).

## Entrega obrigatoria final
Identificacao do **regime aplicavel** com o dispositivo; no penhor, a resposta **venda x apropriacao** com o artigo do Codigo Civil; no bem movel, a distincao declarada e o item 🟡; no veiculo, os quatro pontos com o **aviso de que os paragrafos de debitos nao foram conferidos no literal**; e o **encaminhamento** quando o caso for de outro plugin. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Nunca admitir **apropriacao** do bem empenhado por clausula previa — art. 1.428 do Codigo Civil e nulidade. Nunca dizer que existe **leilao extrajudicial de penhor** por lei geral: o art. 1.433, IV, do Codigo Civil da **execucao judicial ou venda amigavel autorizada**. Nunca chamar de pacto comissorio a apropriacao do art. 9º, §9º, I, da Lei 14.711/2023. Nunca aplicar a exigencia de intimacao do **imovel** ao bem **movel**, nem o contrario. Nunca afirmar a desvinculacao de debitos do art. 328 do CTB **sem conferir o literal** — o corpus so tem caput e §§1º a 3º. Nunca improvisar em **leilao publico administrativo** — e gap declarado. Sempre nomear o diploma junto do numero do artigo. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
