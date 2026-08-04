---
name: leitura-de-matricula
description: "Leitura tecnica da matricula do imovel de leilao, registro a registro e averbacao a averbacao: cadeia dominial, onus reais, hipoteca, alienacao fiduciaria, penhoras, indisponibilidade, usufruto, enfiteuse e terreno de marinha (laudemio), construcao averbada e habite-se. E a prova [2] do gate de due diligence e a UNICA fonte que confirma ou desmente o edital — quem cruza matricula com edital acha o onus nao mencionado, que e a violacao do art. 886, VI e abre a porta do art. 903, §5º, I. Aplica o §11 do art. 27 da Lei 9.514 (constricao sobre o direito do fiduciante nao trava mais o leilao) e o seu limite literal, e o art. 804 do CPC (falta de intimacao de titular de direito real gera INEFICACIA, nao nulidade: o arrematante fica com o imovel E com o gravame). Use antes de qualquer lance, e quando disserem le a matricula, tem onus nesse imovel, o que significa essa averbacao, esse imovel esta livre, tem hipoteca, e terreno de marinha, a area bate."
---

# LEITURA-DE-MATRICULA

> Camada 2. **Prova [2] do gate.** A matricula e a **unica fonte que confirma ou desmente o edital**. Onde os dois divergem, nasce a tese — e nasce o direito de desistir.

## Anexos obrigatorios (context/)
- `context/cpc-leilao-879-903.md` — **804** (os 6 §§ da ineficacia relativa), **886 I e VI**, **903 §§2º e 5º, I** — **grep o artigo e leia a faixa**.
- `context/lei-9514-consolidada.md` — **27 §§11-12** (constricoes e sub-rogacao no saldo), 26 §7º (averbacao da consolidacao), **37-B** (locacao > 1 ano sem anuencia = ineficaz) — **grep + ler a faixa**.
- `context/lei-8245-locacao.md` — **art. 8º, caput**: os tres requisitos do "salvo", dos quais **dois se leem na matricula**; e o art. 33 (averbacao da locacao) — **grep + ler a faixa**.
- `context/clausulas-armadilha-de-edital.md` — ARM-03 (*ad corpus*), ARM-05 (catch-all), ARM-08 (laudemio) — **grep + ler a faixa**.
- `context/custo-total-do-arrematante.md` — §5, o emolumento pela **MAIOR base** — **grep + ler a faixa**.

## Objetivo
Devolver o **estado dominial e de onus** do imovel pela leitura de **cada** registro e **cada** averbacao, com a data e o numero de cada ato — e a lista do que **esta na matricula e nao esta no edital**, que e o achado de maior valor do gate.

## Metodologia
1. **Certidao atualizada.** Matricula vencida ou parcial nao serve — e o que o guard chama de documento nao lido.
2. **Cadeia dominial**: quem e o proprietario **hoje**, por qual titulo, e se a cadeia tem salto ou titulo precario.
3. **Varrer R e Av na ordem cronologica**, um a um. Ato lido pela metade e erro de peca; averbacao de cancelamento **so vale se estiver la**.
4. **Cruzar com o edital** (`analise-de-edital`): todo onus que esta aqui e **nao** esta no edital e violacao do **886, VI**.
5. **Ler os tres itens de custo zero** que so a matricula responde (bloco abaixo).
6. **Confrontar area e descricao** com IPTU e planta (ARM-03) e checar **construcao averbada** e **habite-se**.
7. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## O que procurar, e o que cada achado significa

| Achado | O que decide |
|---|---|
| **Hipoteca** | Sobrevive se o credor **nao foi intimado** (804). Baixa possivel com o credor intimado — o proprio edital costuma remeter ao **CC 1.499** |
| **Alienacao fiduciaria** | O imovel **nao e do devedor**: e propriedade resoluvel do credor. Muda o rito inteiro → `base-legal-alienacao-fiduciaria` |
| **Penhoras de outros processos** | Cada uma tem titular a intimar (889). Cruzar com ARM-13 (penhora no rosto dos autos) e com a ordem de preferencia do **908** |
| **Indisponibilidade** | Trava o **registro** da carta, mesmo com arrematacao valida. Achado de **prazo**, nao so de preco |
| **Usufruto / uso / habitacao** | Direito real de terceiro: **titular a intimar** e **ocupacao legitima** — cruzar com `situacao-possessoria` |
| **Enfiteuse / aforamento / terreno de marinha** | ⭐ **Laudemio** na transferencia — pode somar dezenas de milhares. So a matricula responde |
| **Construcao NAO averbada / sem habite-se** | Area real diverge (ARM-03); **trava financiamento e revenda**. Custo proprio: projeto + INSS + averbacao |
| **Locacao averbada** | ⭐ Ver o bloco de custo zero abaixo — decide se o inquilino fica |
| **Avaliacao x IPTU x base do ITBI** | 🚨 O **emolumento** e enquadrado pela **MAIOR** das bases (SP, Lei estadual 11.331/2002, art. 7º — **regra ESTADUAL**). Arrematar com 50% de desconto **nao corta o emolumento pela metade**. 🟡 **Fora de SP nao foi pesquisado: dar a formula e mandar consultar a tabela da corregedoria local — nunca o numero** |

## ⭐ O art. 804 CPC — por que ineficacia e PIOR que nulidade para o arrematante
Falta de intimacao de titular de direito real gera **INEFICACIA relativa** (CPC 804, **6 paragrafos**), **nao nulidade** — e o **903, §1º, II** e expresso. O leilao **fica de pe**, mas **nao produz efeito perante quem nao foi intimado**: o arrematante fica **com o imovel E com o gravame**, que nao foi purgado. **Todo titular de direito real que aparece na matricula e um item de conferencia de intimacao** — a lista fechada esta em `intimacoes-art-889-e-ineficacia`, e a leitura de risco, em `risco-de-anulacao-do-certame`.

## 🔴 O §11 do art. 27 mudou a leitura da matricula em 31/10/2023 — e tem limite literal
Penhoras, arrestos, bloqueios e indisponibilidades **sobre o direito real de aquisicao do FIDUCIANTE** **nao obstam** a consolidacao nem a venda; os titulares **se sub-rogam no saldo** (§12). Uma matricula "suja" de penhoras contra o devedor **nao trava mais** o leilao de alienacao fiduciaria — conselho anterior a 2023 esta invertido.

⚠️ **O limite e literal:** o §11 fala do direito **do fiduciante**. Constricao sobre a **propriedade** ou vinda de **outra relacao juridica** **nao esta coberta** — nesses casos a leitura antiga continua valendo. Nao estender.

## ⭐⭐ Os tres itens de custo zero que so a matricula responde
1. **A locacao resiste ao leilao?** O "salvo" do **art. 8º, caput, da Lei 8.245** sao **TRES requisitos CUMULATIVOS**: (a) locacao **por tempo determinado**; (b) contrato com **clausula de vigencia em caso de alienacao**; (c) **averbada na matricula**. ⭐ **Falhando UM dos tres, o adquirente pode denunciar** — e os itens (b) e (c) se leem **aqui**. **Locacao nao averbada nao blinda o inquilino**, por melhor que seja a clausula do contrato dele; **contrato averbado com clausula de vigencia e bandeira vermelha de precificacao** (imovel ocupado ate o fim do prazo). Prazos e rota: `situacao-possessoria`.
2. **O imovel e foreiro?** Enfiteuse na matricula = **laudemio** na transferencia (ARM-08).
3. **A construcao esta averbada e ha habite-se?** Sem isso, area divergente, financiamento travado e revenda presa a comprador a vista.

## Regras de ouro
- ⛔ **"Nao identifiquei onus" so pode ser escrito depois de ler a matricula inteira.** Sem certidao atualizada, o veredito e **NO-GO por insuficiencia de prova** — nunca "aparentemente livre".
- **Onus que esta na matricula e nao esta no edital e o achado que vale dinheiro:** viola o **886, VI** e abre o **903, §5º, I** (desiste e recebe o deposito de volta). ⏰ **Caduca em 10 dias do APERFEICOAMENTO**, nao da ciencia. ⚠️ Freio do **§6º**: vicio infundado = ato atentatorio, multa de ate **20% do valor atualizado do bem** — alegar so com o documento na mao.
- **Cancelamento nao se presume:** gravame sem averbacao de baixa **continua vivo** na leitura.
- **A descricao do edital deve refletir a situacao ATUAL**, nao a do contrato antigo (REsp 2.167.979/PB — **turma, nao repetitivo**).
- **Locacao maior que 1 ano sem anuencia escrita do fiduciario e ineficaz** perante ele e seus sucessores (9.514, **art. 37-B**) — rota exclusiva do extrajudicial.
- Cross-link soft: usucapiao, retificacao de area, duvida registral e REURB sao do `direito-imobiliario-adv-os`; aqui a matricula e lida **na otica do arrematante**. O registro da carta e o ITBI ficam em `registro-regularizacao-e-itbi`.

## Entrega obrigatoria final
Quadro com: (a) **cadeia dominial** e proprietario atual; (b) **cada R e Av** com numero, data e efeito; (c) **onus vivos x baixados**; (d) ⭐ **a lista do que esta na matricula e NAO esta no edital**, com o artigo violado; (e) os **tres itens de custo zero**; (f) o que **falta de documento**. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Sem **certidao atualizada** nao ha leitura — ha suposicao, e suposicao e bloqueada. Nao afirmar area, onus, ocupacao ou regularidade sem o ato lido. Nao estender o **§11** alem do **direito do fiduciante**. Nao tratar ineficacia do 804 como nulidade. **Nunca dar numero de emolumento fora de SP** — formula e fonte. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
