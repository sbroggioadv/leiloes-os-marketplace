---
name: imissao-na-posse-do-arrematante
description: "Entrega a posse ao arrematante pela via CERTA — e a via muda conforme o titulo e conforme QUEM esta dentro do imovel. Judicial: mandado de imissao nos proprios autos da execucao, sem acao autonoma, e so depois de pagos preco, comissao, despesas e ITBI (CPC, art. 901, §§1º e 2º). Extrajudicial: acao propria de reintegracao, com liminar EXPRESSA por lei e 60 dias (Lei 9.514, art. 30), assegurada tambem ao adquirente em leilao — e so a exigencia de notificacao obsta. Trava a armadilha da camada: contra LOCATARIO a via nao e imissao nem reintegracao, e DESPEJO (Lei 8.245, art. 5º), e esse despejo nao tem liminar no rol de nove incisos do art. 59, §1º da mesma lei. Use depois de arrematado e quando disserem quero a posse, como tiro o ocupante, pedi a imissao e negaram, o devedor nao sai, quanto tempo ate entrar no imovel, tem inquilino dentro."
---

> **🖱️ Escolhas = botoes:** nas perguntas de lista fechada use **AskUserQuestion** (max. 4 por pergunta).

# IMISSAO-NA-POSSE-DO-ARREMATANTE

> Camada 5. Arrematar nao e ter a posse. **Duas perguntas decidem a via** — qual o titulo e **quem esta dentro** —, e errar a segunda entrega a peca errada para o juiz certo.

## Anexos obrigatorios (context/)
- `context/cpc-leilao-879-903.md` — **CPC, art. 901, §§1º e 2º** (o que o mandado exige **antes**) e **CPC, art. 903, §3º** (carta e mandado so saem passados os 10 dias) — **grep + ler a faixa**.
- `context/lei-9514-consolidada.md` — **Lei 9.514, art. 30** caput e §unico (liminar + 60 dias; o eixo unico que ainda obsta) e **Lei 9.514, art. 37-A** — **grep + ler a faixa**.
- `context/lei-8245-locacao.md` — **Lei 8.245, art. 5º** (a via e o despejo) e **art. 59, §1º** da mesma lei (os **nove** incisos e a **caucao**) — **grep + ler a faixa**.
- `context/lei-14711-2023.md` — **Lei 14.711, art. 9º, §12** (a hipoteca importa o regime da 9.514, com a **ata notarial equiparada a consolidacao**) — **grep + ler a faixa**.
- `context/jurisprudencia-leiloes.md` — §11 item 9 (os REsp de **fonte secundaria**, inteiro teor nao aberto) — **grep + ler a faixa**.

## Objetivo
Dizer **qual instrumento**, **em que juizo**, **com que pre-requisito pago** e **em quanto tempo** — e recusar o atalho quando quem esta dentro exige outra via.

## Metodologia
1. **Pergunta 1 (botoes, lista fechada): qual e o titulo?** — **carta de arrematacao judicial** · **leilao de alienacao fiduciaria (Lei 9.514)** · **hipoteca do art. 9º da Lei 14.711** · **ainda nao tenho titulo**. A ultima opcao **para o fluxo**: sem titulo nao ha imissao.
2. **Pergunta 2 (botoes, lista fechada): quem esta dentro?** — **devedor/executado ou fiduciante** · **locatario** · **invasor** · **terceiro com titulo**. ⚠️ **Esta resposta pode trocar a via inteira** (bloco 🔴 abaixo). "Nao sei" e **documento faltante** → `situacao-possessoria`.
3. **Conferir os pre-requisitos de pagamento** — no judicial eles sao condicao textual da carta e do mandado.
4. **Emitir o pedido** com o fundamento da via correta, o prazo que a lei da e o que **nao** da.
5. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## ⭐⭐ AS TRES VIAS — e a assimetria a favor do extrajudicial

| | **Judicial (carta de arrematacao)** | **AF extrajudicial (Lei 9.514)** | **Hipoteca (Lei 14.711, art. 9º)** |
|---|---|---|---|
| Instrumento | **mandado de imissao nos PROPRIOS AUTOS** — sem acao autonoma | **acao propria** de reintegracao de posse | idem AF, **por remissao do §12** |
| Fundamento | **CPC, art. 901, §1º** | **Lei 9.514, art. 30** | **Lei 14.711, art. 9º, §12** |
| Liminar | 🔴 **nao ha** qualificacao liminar no texto | ✅ **liminar por lei**, expressa | ✅ mesma, por remissao |
| Prazo de desocupacao | 🔴 **o texto nao fixa prazo** | **60 dias** da liminar | **60 dias** |
| Pre-requisito | **preco + comissao + despesas + ITBI**, mais os **10 dias** do art. 903, §2º do CPC vencidos | **consolidacao** comprovada | **ata notarial de arrematacao** — o §12 a **equipara** a consolidacao |

🔴 **A assimetria e real e favorece o extrajudicial.** Quem compara judicial x extrajudicial sem esta linha compara errado: no judicial o arrematante desembolsa **tudo** antes de ter titulo **e** antes de ter posse, e nao tem prazo legal a exigir.

⭐ **A trava do art. 30, §unico da Lei 9.514 e ouro do lado do arrematante.** Arrematado o imovel, discussoes sobre **clausulas contratuais ou requisitos procedimentais** de cobranca e leilao **nao obstam** a reintegracao — resolvem-se em **perdas e danos**. Sobra **um unico eixo** capaz de obstar: a **exigencia de notificacao** do devedor e, se for o caso, do terceiro fiduciante. 🔴 **A Lei 14.711/2023 tirou o recorte antigo:** a trava valia so para financiamento habitacional na redacao da Lei 13.465/2017 — hoje vale para **qualquer** caso arrematado ou definitivamente consolidado. Material que diga o contrario esta desatualizado.

## 🔴🔴 A ARMADILHA DESTA SKILL — contra LOCATARIO a via NAO e imissao

**Lei 8.245, art. 5º:** *"Seja qual for o fundamento do termino da locacao, a acao do locador para reaver o imovel e a de despejo."* E categorico. **Denunciada a locacao e nao saindo o inquilino, o caminho e ACAO DE DESPEJO** — nao e peticao nos autos da execucao, nao e mandado de imissao contra o locatario.

🔴 **E esse despejo nao tem liminar pela denuncia.** O rol do **art. 59, §1º da Lei 8.245** e de **fundamento exclusivo**, tem **nove** incisos, e **nenhum deles e a denuncia por alienacao do art. 8º** da mesma lei — conferido por **prova negativa** no anexo. Quem prometer "imissao liminar contra o inquilino" esta prometendo o que a lei nao da.

⭐ **Onde ha liminar, ela custa caixa:** as hipoteses do art. 59, §1º da Lei 8.245 exigem **caucao equivalente a tres meses de aluguel** e dao **15 dias** para desocupar. Rota completa, incisos aproveitaveis e a segunda porta do **art. 40, VII** da mesma lei estao em `desocupacao-locacao-e-ocupantes` — **nao duplicar aqui**.

🟡 **Se cabe tutela de urgencia generica ou imissao contra o locatario NAO esta resolvido.** O art. 5º da Lei 8.245 nao abre excecao e o rol do art. 59, §1º nao contempla a hipotese — mas isso e **leitura de texto, nao jurisprudencia confirmada nesta captura**. Marcar a ressalva e rotear ao `validador-leiloes` antes de protocolar.

## Quem esta dentro decide o instrumento

| Ocupante | Via correta | Observacao |
|---|---|---|
| **Devedor / executado / fiduciante** | imissao (judicial) ou reintegracao (extrajudicial) | o caso-padrao das duas colunas acima |
| **Locatario** | 🔴 **DESPEJO** (Lei 8.245, art. 5º) | ver `desocupacao-locacao-e-ocupantes` |
| **Invasor** | reintegracao com **prova de esbulho** | sem contrato e sem prazo de lei; custo e **tempo** |
| **Terceiro com titulo** (usufruto, comodato, promessa) | depende do titulo — consta da **matricula** | pode ser **titular a intimar** (CPC, arts. 804 e 889) → `risco-de-anulacao-do-certame` |

## Regras de ouro
- ⛔ **Nao pedir imissao sem os pre-requisitos pagos.** No judicial o **CPC, art. 901, §1º** condiciona carta **e** mandado ao deposito de preco, comissao e despesas, e o **§2º** exige **prova de pagamento do ITBI na carta**. Pedido prematuro so gera indeferimento e perda de tempo.
- ⏰ **O mandado so sai depois dos 10 dias do CPC, art. 903, §2º**, contados do **aperfeicoamento** (assinatura do auto), nao da ciencia de vicio. Vencidos sem alegacao, o **§3º** manda expedir carta e mandado.
- ✅ **A carta deve indicar onus real ou gravame remanescente** (CPC, art. 901, §2º). Carta que silencia sobre gravame conhecido e documento defeituoso — apontar antes de receber.
- ⚠️ **Liminar concedida nao e imovel vazio.** 🟡 A estatistica de cumprimento real **nao foi pesquisada** neste corpus: orcar oficial de justica, forca policial e prazo de cumprimento como **cenario**, nunca como certeza.
- 💰 **No extrajudicial, o relogio do art. 37-A da Lei 9.514 (redacao da Lei 14.711/2023) corre a favor do arrematante:** **1% ao mes sobre o valor do art. 24, VI da Lei 9.514**, desde a **CONSOLIDACAO** ate a **imissao** — e **CREDITO**. 🟡 A **legitimidade do arrematante terceiro** para cobra-la **nao foi pesquisada**: lancar como credito **eventual** → `debitos-e-creditos-pos-arrematacao`.
- 🟡 **Nao citar com numero em peca** `AgInt no REsp 1.898.518/PE` nem `REsp 1.909.196/SP`: vieram de **fonte secundaria** e **nenhum inteiro teor foi aberto** (`jurisprudencia-leiloes.md` §11, item 9). Usar o **texto de lei**, que e ✅, e rotear ao `validador-leiloes`.
- Cross-link soft: quem esta dentro → `situacao-possessoria` · o inquilino → `desocupacao-locacao-e-ocupantes` · carrego ate a posse → `custo-total-real-e-precificacao` · titulo e registro → `registro-regularizacao-e-itbi` · o outro lado do balcao → `defesa-contra-imissao-e-embargos-de-terceiro`.

## Entrega obrigatoria final
Pedido pronto com: (a) **via e fundamento** corretos para o titulo; (b) **quem ocupa** e o documento que prova; (c) **checklist de pre-requisitos** pagos, com o comprovante de cada um; (d) **prazo que a lei da** — e a declaracao expressa quando **nao ha** prazo nem liminar; (e) **horizonte realista** ate o imovel vazio; (f) as ressalvas 🟡 escritas no corpo. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Nunca prometer **liminar** de imissao no **judicial** — o CPC, art. 901, §1º nao a qualifica nem fixa prazo. Nunca pedir imissao **contra locatario**: a via e o **despejo** (Lei 8.245, art. 5º), e a denuncia do art. 8º da mesma lei **nao esta** entre os **nove** incisos do art. 59, §1º. Nunca omitir a **caucao de tres meses de aluguel** quando houver liminar de despejo. Nunca pedir carta ou mandado sem preco, comissao, despesas e **ITBI**. Nunca dizer que a trava do art. 30, §unico da Lei 9.514 vale so no financiamento habitacional. Nunca citar `AgInt no REsp 1.898.518/PE` ou `REsp 1.909.196/SP` com numero em peca. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
