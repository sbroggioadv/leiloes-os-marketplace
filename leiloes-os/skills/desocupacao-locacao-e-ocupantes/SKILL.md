---
name: desocupacao-locacao-e-ocupantes
description: "Tira o ocupante do imovel arrematado pela rota que a lei realmente da, com calendario e CAIXA honestos. Trava a armadilha dos 90 dias: a denuncia da locacao corre do REGISTRO da venda ou do compromisso (Lei 8.245, art. 8º, §2º), nunca da alienacao — perdido o prazo, presume-se a concordancia com a manutencao do contrato. E diz o que quase ninguem diz: o despejo pela denuncia NAO tem liminar (o rol do art. 59, §1º tem nove incisos de fundamento exclusivo, e o art. 8º nao esta entre eles), e onde ha liminar ela exige CAUCAO de tres meses de aluguel. Abre a segunda porta do art. 40, VII — notificar, 30 dias sem nova garantia, despejo com liminar. Cobre a denuncia de 30/90 dias do art. 27, §7º da Lei 9.514 e a ineficacia do art. 37-B. Use quando disserem tem inquilino, quero denunciar a locacao, perdi os 90 dias, o ocupante nao sai, quanto tempo ate o imovel vazio."
---

> **🖱️ Escolhas = botoes:** nas perguntas de lista fechada use **AskUserQuestion** (max. 4 por pergunta).

# DESOCUPACAO-LOCACAO-E-OCUPANTES

> Camada 5. O folclore diz "90 dias". A lei diz **90 para denunciar + 90 para desocupar + processo + 30** — e, havendo liminar, **caucao de tres meses de aluguel adiantada**.

## Anexos obrigatorios (context/)
- `context/lei-8245-locacao.md` — ⭐ **o anexo-mae**: art. 8º (§1), **despejo** (§4), arts. 32-33 (§5), art. 35 (§6), ⭐ **art. 59, §1º — nove incisos e a caucao** (§7), 63-64 (§8), 46/47/57 (§9), 51 (§10), ⭐ **40, VII** (§11) — **grep o artigo e leia a faixa**.
- `context/lei-9514-consolidada.md` — **Lei 9.514, art. 27, §7º** (30/90 dias), **art. 37-B** (locacao acima de um ano **ineficaz**), **art. 30** — **grep + ler a faixa**.
- `context/clausulas-armadilha-de-edital.md` — **ARM-04** (ocupado por conta do adquirente), **ARM-07** (carrego desde a arrematacao) — **grep + ler a faixa**.

## Objetivo
Escolher a **rota**, cravar as **datas**, dizer **quanto custa em caixa**, entregar a peca — e declarar o que a lei **nao** da.

## Metodologia
1. **Pergunta 1 (botoes): quem ocupa?** — **locatario** · **devedor/fiduciante** · **invasor** · **terceiro com titulo**. Fora do locatario, a rota e de `imissao-na-posse-do-arrematante`.
2. **Pergunta 2 (botoes): a aquisicao foi por que via?** — **judicial** · **AF da Lei 9.514** · **hipoteca da Lei 14.711** · **nao sei**. Marco e prazos mudam por inteiro.
3. **Pergunta 3 (botoes): data do REGISTRO** da venda ou do compromisso? — **tenho a data** · **ainda nao registrei** · **em andamento** · **nao sei**. Sem ela **nao ha contagem**.
4. Quem ocupa e os **tres requisitos do "salvo"** do art. 8º vem de `situacao-possessoria` — **nao reapurar**. Rodar a arvore, devolver **calendario + caixa**, fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## ⭐ O marco: 90 dias do REGISTRO — e sao DOIS prazos

> **Lei 8.245, art. 8º, §2º:** a denuncia deve ser exercitada **no prazo de noventa dias contados do REGISTRO da venda ou do compromisso**, presumindo-se, apos esse prazo, a **concordancia na manutencao da locacao**.

🔴 **NUNCA "contados da alienacao"** — a expressao **nao existe** nesta lei. O registro e **posterior**: contar dali **declara morto um prazo que ainda corre**. Marco **registral** ⇒ **quem controla a data e o proprio arrematante**.

⚠️ **Sao DOIS prazos de 90 no mesmo artigo — nao os funda** (tabela abaixo). ⏰ **Dias CORRIDOS**: prazo material, exercido por notificacao fora do processo; o **CPC, art. 219** limita os dias uteis aos prazos **processuais**.

⚠️ **Grave as DUAS datas** em `memoria-de-caso-leilao`: **registro = o prazo** · **alienacao = referencia**. 🟡 A lei **nao** diz se a arrematacao e "alienacao" do art. 8º nem se o registro da carta e o "registro da venda" do §2º — leituras que o plugin adota, **nao literais e nao confirmadas nesta captura**. ⭐ **Sobrevive as duas: denuncie CEDO.**

## 🔴 O CALENDARIO HONESTO — ele nao termina no dia 90

| Etapa | Prazo | Base (Lei 8.245) |
|---|---|---|
| Denunciar | ate **90 dias** do **registro** | art. 8º, §2º |
| Locatario desocupar | **90 dias** da denuncia | art. 8º, caput |
| Nao saindo: **acao de despejo** | 🔴 **sem liminar** por este fundamento | arts. 5º e 59, §1º |
| Apos sentenca de procedencia | **+30 dias** de desocupacao voluntaria | art. 63 |
| ⭐ Reducao gratuita | **15 dias**, se passaram **mais de 4 meses** entre citacao e sentenca | art. 63, §1º, "a" |

**Horizonte: 90 + 90 + processo + 30.** ⚠️ **Execucao provisoria do despejo exige caucao de 6 a 12 meses de aluguel** (Lei 8.245, art. 64) — nunca "12 a 18", redacao vencida.

## 🔴 A LIMINAR DE DESPEJO — nove incisos, fundamento EXCLUSIVO, e ela CUSTA CAIXA

**Lei 8.245, art. 59, §1º:** liminar de desocupacao em **quinze dias**, sem ouvir a parte contraria, ⭐ **desde que prestada caucao no valor equivalente a tres meses de aluguel**, nas acoes de **fundamento exclusivo** ali listado.

🔴 **Sao NOVE incisos e a denuncia por alienacao do art. 8º NAO esta entre eles** — prova negativa feita no anexo (`context/lei-8245-locacao.md`, §7, verbatim). ⚠️ **Ao recontar por grep:** I-V usam hifen e VI-IX usam **travessao**; grep ingenuo devolve cinco. Os **seis** que nao servem ao arrematante (I acordo · II art. 47, II · III temporada · IV morte do locatario · V sublocatario · VI reparacoes urgentes) ficam no anexo — **grep se o caso encaixar**.

⭐ **Os tres que servem:** **VII** — prazo notificatorio do **art. 40, §unico** vencido **sem nova garantia** (bloco abaixo) · **VIII** — locacao **NAO residencial** com prazo terminado, acao em ate **30 dias** do termo ou da notificacao de retomada (janela curta) · **IX** — falta de pagamento com contrato **desprovido de garantia**, e aqui esta o veneno: 🔴 **o locatario ELIDE a liminar depositando o total devido dentro dos 15 dias** (art. 59, §3º). **Vender o IX como certeza e erro.**

🔴 **A caucao e caixa adiantado no PIOR momento** — depois de pagos preco, comissao, despesas e ITBI, e **antes** de ter carta e posse. Entra na linha de desocupacao de `custo-total-real-e-precificacao`; nunca fica fora da conta.

## ⭐⭐ A SEGUNDA PORTA — art. 40, VII: a rota mais rapida da lei

**Lei 8.245, art. 40, VII:** a **"desapropriacao ou alienacao do imovel"** e causa expressa para **exigir novo fiador ou substituir a garantia**. Pelo **§unico**: notificado o locatario e **nao apresentada nova garantia em 30 dias**, a sancao e o **desfazimento da locacao** — o que **destrava o inciso VII do art. 59, §1º**, hipotese de **liminar**.

```
notificar (art. 40, VII) -> 30 dias sem nova garantia -> despejo COM liminar (59, §1º, VII)
                                                        + caucao de 3 meses + 15 dias
```

⭐ **Depende de FATO OBJETIVO** — ausencia de garantia nova —, **nao de tese**. E a saida de quem perdeu os 90 dias. **Conferir a garantia do contrato antes de escolher a rota.**

## As outras rotas

| Situacao | Rota | Base |
|---|---|---|
| Prorrogada, prazo **abaixo de 30 meses** | **sem** denuncia vazia — so o rol do art. 47; o mais acessivel e o **inciso V** (5 anos ininterruptos). ⚠️ Nos incisos **III e IV**, quem concorda ganha **6 meses** da citacao (art. 61) | Lei 8.245, art. 47 |
| Prorrogada, **30 meses ou mais** | denuncia vazia **a qualquer tempo**, 30 dias | Lei 8.245, art. 46, §2º |
| Nao residencial, prazo **indeterminado** | denuncia escrita, **30 dias** | Lei 8.245, art. 57 |
| **Alienacao fiduciaria** | denuncia em **90 dias da CONSOLIDACAO**; desocupacao em ⚠️ **30 dias** | Lei 9.514, art. 27, §7º |
| Locacao **acima de um ano** sem anuencia escrita do fiduciario | **ineficaz** perante fiduciario **e sucessores** — ⚠️ mas ineficacia se **declara** | Lei 9.514, art. 37-B |

🔴 **Os dois erros que a tabela impede:** aplicar os **30 dias** da Lei 9.514 a arrematacao **judicial** (la sao **90**), e usar o marco **"consolidacao"** fora da alienacao fiduciaria.

⚠️ **Lote comercial:** locatario com **5 anos** de contrato e **3 anos** no mesmo ramo tem direito a **renovacao por igual prazo** (Lei 8.245, art. 51, requisitos **cumulativos**), decadencia estreita no **§5º**. 🟡 Como ela interage com a denuncia do art. 8º **nao esta na lei** — ressalva + rota.

## Regras de ouro
- ✅ **O locatario NAO tem preferencia no leilao.** O **art. 32, caput da Lei 8.245** exclui a "venda por **decisao judicial**": no judicial a blindagem e **limpa e incondicionada**. 🟡 No **extrajudicial de garantia** vale o **§unico**, que exige **clausula especifica com destaque grafico**, e **em qual contrato** ela deve estar **nao esta resolvido** — ressalva + rota. Sem o art. 32, o **art. 33** deixaria o locatario preterido **haver o imovel para si** em **6 meses do registro do ato**.
- ⚠️ **Benfeitorias podem terminar os 90 dias com o imovel AINDA OCUPADO.** **Necessarias** (mesmo **nao autorizadas**) e **uteis autorizadas** sao indenizaveis **e dao direito de RETENCAO** (Lei 8.245, art. 35) — defesa possessoria. ⭐ **Procure PRIMEIRO a clausula de renuncia**, admitida pelo caput. 🟡 Se o **arrematante** responde por benfeitorias anteriores a aquisicao **nao esta dito na lei** — marcar e rotear.
- ⛔ **Nunca prometer despejo liminar pela denuncia do art. 8º**, nem contar os 90 dias em dias uteis.
- 💰 **O carrego comeca na arrematacao, nao na posse** (ARM-07) → `custo-total-real-e-precificacao`.
- Cross-link soft: quem ocupa → `situacao-possessoria` · devedor e invasor → `imissao-na-posse-do-arrematante` · o outro lado → `defesa-contra-imissao-e-embargos-de-terceiro` · liminar → `tutela-de-urgencia-leiloes`.

## Entrega obrigatoria final
(a) **Rota** com fundamento; (b) **as duas datas** e a contagem; (c) **calendario** ate o imovel vazio, com cenario de resistencia; (d) **caixa**: caucao de 3 meses havendo liminar, 6 a 12 meses na execucao provisoria, honorarios e carrego; (e) a **notificacao** ou a **inicial**; (f) as ressalvas 🟡 escritas. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Nunca contar os **90 dias** da alienacao, da arrematacao, da carta ou da imissao — o **art. 8º, §2º da Lei 8.245** conta do **REGISTRO**. Nunca fundir os dois prazos de 90. Nunca prometer **liminar** pela denuncia do art. 8º: o rol do **art. 59, §1º** e de **fundamento exclusivo** e tem **nove** incisos. Nunca omitir a **caucao de tres meses de aluguel**, nem escrever "12 a 18 meses" no art. 64 (e **6 a 12**). Nunca vender o inciso IX como certeza — o §3º permite elidir em 15 dias. Nunca aplicar os **30 dias** da Lei 9.514 a leilao judicial. Nunca dizer que o locatario tem preferencia, nem prometer imovel vazio ignorando a **retencao do art. 35**. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
