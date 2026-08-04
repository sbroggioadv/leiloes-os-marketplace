---
name: mecanica-do-leilao-judicial
description: "O mapa completo da expropriacao judicial: adjudicacao (CPC 876-878), alienacao por iniciativa particular (CPC 880) e, so depois delas, o leilao (CPC 881-903) — com 1a e 2a praca, publicidade, adiamento, licitacao entre pretendentes, lance global, alienacao parcial e a regua do preco vil em CASCATA (CPC 885 x 891), que nao e 50% e pronto: havendo preco minimo no edital, vil e o que fica abaixo DELE, e os 50% da avaliacao so entram na ausencia de minimo. Carrega o piso proprio de 80% da avaliacao no imovel de incapaz (CPC 896) e o eletronico como via ordinaria (CPC 882). Use para entender como o leilao funciona por dentro, e quando disserem como funciona leilao judicial, o que e primeira e segunda praca, esse lance e preco vil, por que ninguem adjudicou antes, o leilao foi adiado, da pra arrematar so parte do imovel, quem pode dar lance, o leilao tem que ser eletronico."
---

# MECANICA-DO-LEILAO-JUDICIAL

> Camada 3. O mapa de **como o bem chegou ao leilao** e de **como o leilao funciona por dentro**. Quem quer saber *se compra* roda o gate da camada 2; aqui se aprende *o que esta acontecendo* e onde cada trava mora.

## Anexos obrigatorios (context/)
- `context/cpc-leilao-879-903.md` — §0 (o mapa) · **876-878** · **880** · 879/882/883 · **884** · **885** · 887-888 · **890** · **891 §unico** · 892-894 · **896** · 897-900 — **grep o artigo e leia a faixa**.
- `context/resolucao-cnj-236-2016.md` — arts. **11** (abertura do sistema), **21** (prorrogacao), **22 §unico** e **7º** (comissao) — **grep + ler a faixa**.
- `context/metodologia-leiloes.md` — **§7.1** (homonimo de criterio: percentual so vale com a base colada) e §10 (o relogio) — **grep + ler a faixa**.

## Objetivo
Dizer, para o caso concreto, **em que etapa da expropriacao o bem esta**, **qual regra rege aquela etapa** e **onde estao as travas** — na linguagem da trilha escolhida (advogado ou investidor), sobre o mesmo corpus.

## Metodologia
1. **Situar a etapa** no mapa das tres vias. Leilao e a **terceira**, nao a primeira.
2. **Ler o edital** por `analise-de-edital` — etapa se prova por documento, nunca por suposicao.
3. **Aplicar a regua do preco vil em cascata** e checar se ha **piso especial** (incapaz).
4. **Rodar as travas da etapa** e fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## O mapa das tres vias — e a pergunta que ele obriga

| # | Via | Base | O que decide |
|---|---|---|---|
| 1 | **Adjudicacao** | CPC 876-878 | Exequente e legitimados ficam com o bem por preco **nao inferior a avaliacao** |
| 2 | **Alienacao por iniciativa particular** | CPC 880 | Venda direta por corretor ou leiloeiro credenciado; o **juiz** fixa prazo, publicidade, **preco minimo**, condicoes, garantias e a comissao de corretagem |
| 3 | **Leilao judicial** | CPC 881-903 | **So se nao efetivadas** as duas anteriores (CPC 881) |

⭐ **Primeira pergunta da due diligence:** o bem passou por **duas janelas** em que o credor podia te-lo tomado e **nao tomou**. Isso e **sinal, nao garantia** — obriga perguntar *por que ninguem adjudicou?* Regime completo em `adjudicacao-e-as-tres-remicoes`.

🔴 **Distincao que muda a peca:** quem compra pela via 2 recebe **carta de ALIENACAO** (CPC 880, §2º, I), e o negocio se aperfeicoa por **termo nos autos**. 🟡 A mecanica do **CPC 903** (10 dias, invalidacao, desistencia) esta redigida para a **arrematacao** — **nao transportar automaticamente** para a alienacao particular. Ponto em aberto: marcar *"conferir antes de protocolar"* e rotear ao `validador-leiloes`.

## ⭐⭐ Preco vil — a regua e em CASCATA (CPC 885 x CPC 891)

| Cenario | Piso do preco vil |
|---|---|
| Juiz **fixou** preco minimo no edital (**CPC 885**) | **O minimo do edital** — vil e o que fica abaixo dele |
| Juiz **nao fixou** preco minimo | **50% da avaliacao** — **CPC 891, §unico**, regra **supletiva** |
| **Imovel de INCAPAZ** | **80% da avaliacao** — **CPC 896**, regua propria, nao os 50% |

**Tres erros que o guard bloqueia:**
1. *"O CPC fixa 50%"* como regra geral — **nao fixa**; os 50% sao **supletivos**.
2. *"O piso de 50% vale so para a 1a praca"* — **o CPC nao separa pracas** na regua do preco vil. O que muda entre elas e o **preco de aceitacao da proposta parcelada** (CPC 895, I e II).
3. **Transportar os 50% do CPC para o extrajudicial** — la a regua e propria (**Lei 9.514, art. 27, §2º** e **Lei 14.711, art. 9º, §6º**) e o "50%" e **faculdade do credor**, jamais piso de vileza nem direito do arrematante.

⚠️ **Homonimo de criterio — o percentual so entra no texto com a BASE colada.** O **20% do CPC 896, §2º** (arrependimento do pretendente que havia caucionado no adiamento) incide **sobre a AVALIACAO**, em beneficio do incapaz, e a decisao vale como **titulo executivo**. Nao e o 20% do **lance** de clausula de edital, nem os 20% de **caucao**, que sao **deposito e nao multa**. Bases diferentes **nao se somam nem se comparam** — `context/metodologia-leiloes.md` §7.1.

## As travas de cada etapa

| Etapa | Regra | A trava |
|---|---|---|
| **Modalidade** | **CPC 882**: nao sendo possivel o eletronico, o leilao sera **presencial** | O eletronico e a via **ordinaria** e o presencial a **subsidiaria justificada**. ⛔ Nao afirmar que a lei "obriga" o eletronico em termos absolutos. O **§1º do CPC 882** e o gancho legal da Res. CNJ 236/2016 |
| **Quem conduz** | **CPC 883**: designacao do leiloeiro cabe ao **juiz**, podendo ser indicado pelo exequente | Due diligence do leiloeiro por **nome + matricula** em `estrategia-de-lance-e-habilitacao` |
| **Deveres e comissao** | **CPC 884**: publicar, realizar, expor, **depositar em 1 dia**, **prestar contas em 2 dias** | 🔴 O **CPC nao fixa percentual** (884, §unico: "estabelecida em lei ou arbitrada pelo juiz"). Os 5% vem do **Decreto 21.981/1932, art. 24, §unico** e da **Res. CNJ 236, art. 7º** ("**no minimo** 5%"), e sao **do arrematante** |
| **Publicidade** | **CPC 887, §1º**: publicacao **≥ 5 dias** antes | 🔴 **Tres "5 dias" distintos:** publicacao do edital (**CPC 887, §1º**) · cientificacao das 8 categorias (**CPC 889**) · abertura do sistema para lances (**Res. CNJ 236, art. 11**). Mesmo numero, funcoes diferentes |
| **Adiamento** | **CPC 888**: nao realizado o leilao, publica-se a transferencia | O §unico responsabiliza pelas despesas quem **culposamente** der causa, com suspensao de **5 dias a 3 meses** |
| **Pregao eletronico** | **Res. CNJ 236, art. 21** | Prorrogacao automatica de **3 minutos** no exclusivamente eletronico e **15 segundos** no presencial/simultaneo — **nao existe lance-surpresa no estalar do prazo**. **Art. 22, §unico**: lance por e-mail e proibido |
| **Pagamento** | **CPC 892**: de imediato, por deposito judicial ou meio eletronico | **§1º**: exequente unico credor nao exibe o preco, mas deposita a diferenca em **3 dias**, sob pena de a arrematacao ficar sem efeito e o novo leilao correr **as custas dele** |
| **Licitacao e preferencias** | **CPC 892, §§2º-3º** | 🔴 A preferencia do conjuge, companheiro, descendente ou ascendente **so incide em IGUALDADE DE OFERTA** — **nao e direito de cobrir** o lance vencedor. ⛔ Nao confundir com o **direito de preferencia do fiduciante da Lei 9.514, art. 27, §2º-B**, instituto distinto em procedimento distinto. Em bem tombado preferem Uniao, Estados e Municipios, nessa ordem |
| **Lance global** | **CPC 893** | Varios bens e varios lancadores: prefere quem arremata **todos em conjunto**, pagando avaliacao pelos sem lance e o maior lance pelos demais |
| **Alienacao parcial** | **CPC 894** | Tese de **reducao de dano** pouco usada pelo executado: vender so a parte suficiente. Exige **planta e memorial descritivo** e tem de ser requerida **a tempo de entrar no edital** |
| **Quem NAO pode lancar** | **CPC 890** | Seis incisos. ⭐ **VI: advogado de QUALQUER das partes** — do exequente e do executado. O **V** (leiloeiro e prepostos) espelha o art. 3º da Res. CNJ 236 |
| **Arrematante remisso** | **CPC 897-900** | ⭐ Nao pagar **nao e "perder o sinal": e EXCLUSAO** — perde a caucao **e fica banido daquele novo leilao**, com o fiador remisso. O fiador que paga lance e multa pode pedir a transferencia (898); suspende-se a arrematacao quando o produto ja basta ao credor e as despesas (899); ultrapassado o expediente, prossegue no **dia util imediato, na mesma hora, sem novo edital** (900) |

## Regras de ouro
- ⛔ **Etapa nao se deduz do calendario nem do site da plataforma** — prova-se no edital e nos autos. Sem documento, a resposta e *"nao verificado"*, nunca uma etapa presumida.
- **1a e 2a praca nao mudam a regua do preco vil.** Mudam o **preco de aceitacao da proposta parcelada** (CPC 895, I e II) e a expectativa de desagio. Desagio medio provado do mercado: **37,3%** — nunca prometer 70%.
- **A comissao nao esta dentro do lance.** Prova textual no **CPC 901, §1º**: sem deposito **+ comissao + despesas** nao ha carta nem mandado de imissao. Conta em `custo-total-real-e-precificacao`.
- **Explicar mecanica nao autoriza opinar sobre lance.** Opiniao de lance so depois do **gate due-diligence-first** completo (4 provas), pelo `parecer-go-nogo-lote` — os 10 dias do **CPC 903, §2º** correm do **aperfeicoamento**.
- Cross-link soft, sem duplicar: intimacoes em `intimacoes-art-889-e-ineficacia` · auto e carta em `arrematacao-auto-e-carta` · parcelamento em `arrematacao-parcelada-895` · adjudicacao e remicoes em `adjudicacao-e-as-tres-remicoes` · relogio de 10 dias em `invalidacao-embargos-e-desistencia-903` · preco vil como tese na camada de defesa.

## Entrega obrigatoria final
Mapa do caso com: (a) **etapa atual** e o documento que a prova; (b) **regra que rege a etapa**, com artigo e diploma nomeados; (c) **travas ativas** naquela etapa; (d) a **regua de preco vil aplicavel** com a base colada; (e) o que **nao foi possivel verificar** por falta de documento. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Nunca *"o CPC fixa 50% de preco vil"* · nunca *"o CPC fixa 5% de comissao"* · nunca *"o piso vale so na 1a praca"* · nunca transportar a regua de preco vil ao extrajudicial · nunca confundir a preferencia do **CPC 892, §2º** (igualdade de oferta) com a preferencia do fiduciante da **Lei 9.514, art. 27, §2º-B** · nunca estender o **CPC 903** a alienacao particular sem ressalva · nunca opinar sobre lance sem o gate completo. Percentual sem base colada nao entra no texto. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
