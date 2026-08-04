---
name: situacao-possessoria
description: "Apura QUEM ocupa o imovel do leilao — devedor, locatario, invasor ou terceiro com titulo — e precifica prazo e custo de tira-lo de la. E a prova [3] do gate de due diligence e a linha que mais destroi margem, porque o relogio de condominio e IPTU vira na arrematacao e nao na posse. Traz o marco correto dos 90 dias do locatario: a Lei 8.245, art. 8º, §2º conta do REGISTRO da venda ou do compromisso, NUNCA da alienacao — contar da alienacao declara morto um prazo que ainda corre. Distingue as tres rotas que nao se misturam (arrematacao judicial, alienacao fiduciaria e locacao longa sem anuencia), mostra a assimetria de desocupacao entre judicial e extrajudicial, e avisa que a denuncia do art. 8º NAO da despejo liminar. Use antes de qualquer lance em imovel ocupado, e quando disserem tem gente morando, o imovel esta ocupado, tem inquilino, como tiro o ocupante, quanto tempo ate a posse, posso denunciar a locacao."
---

> **🖱️ Escolhas = botoes:** nas perguntas de lista fechada use **AskUserQuestion** (max. 4 por pergunta).

# SITUACAO-POSSESSORIA

> Camada 2. **Prova [3] do gate.** "Imovel ocupado" nao e um dado — sao **quatro** situacoes juridicas, com prazos, vias e custos diferentes. Quem nao apura **quem** ocupa esta chutando o item mais caro da conta.

## Anexos obrigatorios (context/)
- `context/lei-8245-locacao.md` — ⭐ **o anexo-eixo**: art. 8º verbatim, as **tres rotas** (§3), a **via do despejo sem liminar** (§4), a **blindagem do art. 32** (§5), as **benfeitorias** (§6), a **segunda porta do art. 40, VII** (§11) — **grep o artigo e leia a faixa**.
- `context/lei-9514-consolidada.md` (Lei 9.514) — **art. 30** (reintegracao liminar em 60 dias, assegurada **tambem ao arrematante**), 27 §7º, **37-B**, 37-A — **grep + ler a faixa**.
- `context/cpc-leilao-879-903.md` — **901 §1º** (o que o mandado de imissao exige antes) — **grep + ler a faixa**.
- `context/clausulas-armadilha-de-edital.md` — ARM-04 (ocupado por conta do adquirente) e ARM-07 (encargos desde a arrematacao) — **grep + ler a faixa**.

## Objetivo
Nomear **quem** ocupa, **com que titulo**, **por qual rota** se retira e **em quanto tempo e a que custo** — dando o carrego a `custo-total-real-e-precificacao` e o prazo real ate a posse ao `parecer-go-nogo-lote`.

## Metodologia
1. **Pergunta em botoes (lista fechada): quem ocupa?** — **devedor/executado** · **locatario** · **invasor** · **terceiro com titulo**. "Nao sei" nao e resposta: e **documento faltante**.
2. **Provar com documento ou diligencia** — certidao do oficial, constatacao, vistoria, contrato, matricula. **Boato de sindico ou anuncio nao e prova.**
3. **Fixar a ROTA** (tabela abaixo): ela decide marco, prazo e via.
4. **Ler na matricula** os dois requisitos registrais do "salvo" do art. 8º.
5. Devolver o **horizonte em meses** com cenario de resistencia. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## ⭐⭐ O marco dos 90 dias — o erro mais caro do dominio

> **Lei 8.245, art. 8º, §2º:** a denuncia deve ser exercitada **no prazo de noventa dias contados do REGISTRO da venda ou do compromisso**, presumindo-se, apos esse prazo, a **concordancia na manutencao da locacao**.

🔴 **NUNCA contar da alienacao.** A expressao "contados da alienacao" **nao existe** nesta lei. O **registro e sempre posterior** ao ato de alienacao — contar dali **declara morto um prazo que ainda corre**. E o marco e **registral**: **quem controla a data do registro e o proprio arrematante**.

⭐ **Sao DOIS prazos de 90 dias no mesmo artigo — nao os funda:**

| | **Para DENUNCIAR** | **Para DESOCUPAR** |
|---|---|---|
| Onde | **art. 8º, §2º** | **art. 8º, caput** |
| Contado de | ⭐ **do REGISTRO** da venda ou do compromisso | da **denuncia** |
| Se estourar | **presume-se a concordancia** com a manutencao | o adquirente ajuiza **despejo** (art. 5º) |

**Horizonte literal ate o imovel vazio: 90 + 90 = ate 180 dias do registro** — e isso **antes** de qualquer despejo. Planejar 90 dias e subestimar pela metade.

⚠️ **Grave as DUAS datas** em `memoria-de-caso-leilao`: **registro = o prazo** · **alienacao = referencia**. 🟡 Dois pontos que a lei **nao** resolve: (a) **a arrematacao e "alienacao" do art. 8º?** — o caput nao menciona hasta publica; (b) **o registro da carta e o "registro da venda" do §2º?**. Sao as leituras que este plugin adota, **nao sao literais** e **nao foram confirmadas em jurisprudencia nesta captura**. ⭐ **Postura que sobrevive aos dois: denuncie CEDO** — denuncia logo apos a aquisicao e boa sob qualquer leitura; a tardia depende de vencer os dois ao mesmo tempo. Antes de protocolar, **rotear ao `validador-leiloes`**.

⏰ **Dias CORRIDOS.** Sao prazos de **direito material**, exercidos por notificacao fora do processo; o **CPC 219** limita a contagem em dias uteis aos **prazos processuais**.

## ⭐ A defesa forte do locatario — e ela se le na matricula
A locacao **so resiste** a alienacao se, **ao mesmo tempo** (art. 8º, caput): (a) for por **tempo determinado**; (b) o contrato tiver **clausula de vigencia em caso de alienacao**; **e** (c) estiver **averbado na matricula**. **Falhando UM dos tres, o adquirente pode denunciar** — e (b) e (c) se leem em `leitura-de-matricula`, a custo zero. **Locacao nao averbada nao blinda o inquilino**; **contrato averbado com clausula de vigencia afasta a denuncia inteira** e e **bandeira vermelha de precificacao**.

## ⭐⭐ AS TRES ROTAS NAO SE MISTURAM

| | **Arrematacao judicial** | **AF extrajudicial** | **Locacao longa sem anuencia** |
|---|---|---|---|
| Fundamento | **8.245, art. 8º** | **9.514, art. 27, §7º** | **9.514, art. 37-B** |
| Quem denuncia | o **adquirente** | o **fiduciario** e sucessores | — (locacao **ineficaz**) |
| ⭐ **Marco** | **REGISTRO** da venda | **CONSOLIDACAO** | — |
| Denunciar / desocupar | 90 dias / **90 dias** | 90 dias / ⚠️ **30 dias** | — |
| Nao se aplica se | prazo determinado **+** clausula de vigencia **+** averbada | houve **aquiescencia escrita** do fiduciario | locacao de **ate 1 ano** ou com anuencia escrita |

🔴 **Os dois erros que a tabela impede:** aplicar os **30 dias** da 9.514 a **arrematacao judicial** (la sao **90**); e usar o marco **"consolidacao"** fora da alienacao fiduciaria — **consolidacao nao existe em leilao judicial**, onde o marco e **registral**.

## 🔴 A assimetria de desocupacao — e a pior noticia honesta

| | **Judicial (CPC 901, §1º)** | **Extrajudicial (9.514, art. 30)** |
|---|---|---|
| Instrumento | mandado de imissao **nos autos** | **acao propria** de reintegracao |
| Liminar / prazo | **nao ha** qualificacao liminar nem prazo no texto | **liminar EXPRESSA** + **60 dias** |
| Pre-requisito | so apos **preco + comissao + despesas + ITBI** | comprovada a **consolidacao** |

🔴🔴 **Contra o LOCATARIO a via e o DESPEJO (art. 5º) — e esse despejo NAO tem liminar.** O rol do **art. 59, §1º** e de **fundamento exclusivo**, tem **nove incisos**, e **nenhum e a denuncia por alienacao do art. 8º**. Apos a sentenca ainda ha **30 dias** (art. 63 Lei 8.245). **Lote judicial com locacao viva e caro em tempo, e o edital nao mostra isso.** 🟡 Se cabe **tutela de urgencia generica** ou imissao contra o locatario **nao esta resolvido** — e leitura de texto, nao jurisprudencia: marcar e **rotear ao `validador-leiloes`**.

⭐ **A segunda porta, para quem perdeu os 90 dias — e ela TEM liminar.** O **art. 40, VII** poe a **alienacao** como causa expressa para **exigir novo fiador**; pelo **§unico**, notificado o locatario e **nao apresentada nova garantia em 30 dias**, a sancao e o **desfazimento da locacao** — hipotese que **destrava o inciso VII do art. 59, §1º**, caso de **liminar**. Caminho: **notificar → 30 dias sem garantia → despejo com liminar**. Depende de **fato objetivo**, nao de tese.

## Regras de ouro
- ⛔ **Nao afirmar ocupacao sem documento.** "Parece desocupado" e "aparentemente livre" sao bloqueados; sem apuracao o parecer sai **NO-GO por insuficiencia de prova**.
- ✅ **O locatario NAO tem preferencia no leilao.** O **art. 32, caput** exclui a "venda por **decisao judicial**" — no judicial a blindagem e **limpa e incondicionada**. 🟡 No **extrajudicial de garantia** vale o **§unico**, que exige **clausula especifica com destaque grafico**, e **em qual contrato** ela deve estar **nao esta resolvido** — ressalva + `validador-leiloes`. Sem o art. 32, o **art. 33** deixaria o locatario preterido **tomar o imovel para si** em **6 meses do registro**.
- ⚠️ **Benfeitorias seguram o imovel.** Necessarias (**mesmo nao autorizadas**) e uteis **autorizadas** sao indenizaveis **e dao direito de RETENCAO** (art. 35) — defesa possessoria que faz os 90 dias **nao terminarem em imovel vazio**. **Procurar primeiro a clausula de renuncia**, admitida pelo caput. 🟡 Se o **arrematante** responde por benfeitorias anteriores a aquisicao **nao esta dito na lei** — marcar e rotear.
- **Invasor** nao tem contrato nem prazo de lei: reintegracao com prova de esbulho, custo de **tempo**. **Terceiro com titulo** (usufruto, comodato, promessa) consta da **matricula** e pode ser **titular a intimar** (804/889) → `risco-de-anulacao-do-certame`.
- **O carrego comeca na arrematacao, nao na posse** (ARM-07). No extrajudicial, a **taxa de ocupacao de 1%/mes desde a CONSOLIDACAO** (37-A) e **credito**; 🟡 a legitimidade do **terceiro** para cobra-la nao foi pesquisada — lancar como credito **eventual**, nunca como receita certa.

## Entrega obrigatoria final
Quadro com: (a) **quem ocupa** e o documento que prova; (b) o **titulo** do ocupante; (c) **rota** e **marco** corretos; (d) **as duas datas** (registro e alienacao); (e) **horizonte em meses** ate o imovel vazio, com cenario de resistencia; (f) **custo estimado** (honorarios + carrego); (g) o que falta de documento. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Ocupacao **nao se presume**. Nunca contar os 90 dias **da alienacao, da arrematacao, da carta ou da imissao** — o art. 8º, §2º conta do **REGISTRO**. Nunca fundir os dois prazos (horizonte **ate 180**). Nunca aplicar os **30 dias** da 9.514 a leilao judicial. Nunca prometer **despejo liminar** com base na denuncia do art. 8º. Nunca dizer que o locatario tem preferencia no leilao. Nunca contar prazo material em **dias uteis**. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
