---
name: base-legal-alienacao-fiduciaria
description: "Fundacao legal do leilao EXTRAJUDICIAL de imovel: Lei 9.514/97 consolidada pos-Lei 14.711/2023, artigo a artigo, marcando o que mudou em 31/10/2023 e invertendo conselho antigo. Cobre o encargo do fiduciante do art. 23 §2º (IPTU e taxas condominiais — o endereco vigente, nunca o art. 24 §2º), a intimacao da mora e a intimacao eletronica imprescindivel do art. 26 §4º-B, o regime do imovel residencial do art. 26-A (purga ate a averbacao, divida extinta, condicao resolutiva que alcanca a via judicial), os dois leiloes do art. 27 com o saldo remanescente do §5º-A e as constricoes dos §§11-12, a excussao multipla do 27-A, a reintegracao liminar do art. 30 e a taxa de ocupacao do 37-A. Use em qualquer caso de alienacao fiduciaria, consolidacao, purga, leilao de banco ou defesa do fiduciante, e quando disserem base legal do extrajudicial, a 9.514 diz o que, artigo da alienacao fiduciaria, consolidacao da propriedade."
---

# BASE-LEGAL-ALIENACAO-FIDUCIARIA

> Camada 1. Fundacao do lado extrajudicial. Entrega a Lei 9.514/97 **como ela esta hoje**, com o marco de 31/10/2023 visivel: quem opera essa lei pela memoria anterior a 2023 da conselho invertido.

## Anexos obrigatorios (context/)
- `context/lei-9514-consolidada.md` — arts. 23 a 39 consolidados. **Ler o AVISO 2 (pegadinha de Planalto: redacoes sucessivas na mesma tela) e o AVISO 3 (art. 23, §2º x art. 24, §2º) antes de citar qualquer coisa** — **grep o artigo e leia a faixa**.
- `context/lei-14711-2023.md` — o que a 14.711 revogou e alterou aqui (art. 18, V) — **grep + ler a faixa**.
- `context/jurisprudencia-leiloes.md` — Tema 1.288, REsp 2.135.500, REsp 1.949.182, REsp 2.167.979/PB — **grep + ler a faixa**.
- `context/lei-8245-locacao.md` — art. 8º, §2º verbatim: os **90 dias do locatario correm do REGISTRO** da venda ou do compromisso — **grep + ler a faixa**.

## Objetivo
Devolver o dispositivo vigente do rito extrajudicial da alienacao fiduciaria, com o prazo e o **marco inicial** nomeados, e sinalizar quando o dispositivo mudou de sentido em 2023. Alimenta C4 (rito), C5 (pos-arrematacao) e C6 (defesa do fiduciante).

## Metodologia
1. Localizar a fase: mora e intimacao · consolidacao · 1º leilao · 2º leilao · sobra ou saldo · reintegracao.
2. Grep do artigo no anexo e **leitura da faixa inteira**. ⚠️ Nesta lei o compilado exibe **redacoes sucessivas sem tachado** — conferir sempre a **atribuicao** de cada paragrafo antes de citar.
3. Marcar o que mudou em **31/10/2023** e o que virou direito intertemporal.
4. Devolver dispositivo + prazo com marco + efeito pratico + skill de destino.
5. Fechar por `validador-leiloes` e `suprema-corte-leiloes`.

## Artigo a artigo — o que decide

| Dispositivo | O que trava |
|---|---|
| **23, §2º** 🔴⭐ | **O endereco VIGENTE do encargo do fiduciante** por **IPTU e taxas condominiais** (incluido pela Lei 14.620/2023, art. 28). ⚠️ **Nao cite o art. 24, §2º** — ver o bloco abaixo |
| **24** | Requisitos do contrato; inciso VI o valor para leilao; **§unico: a base do ITBI prevalece se maior** |
| **26** | Mora e **intimacao pessoal, 15 dias**; §1º-A multiplas circunscricoes; §2º-A carencia supletiva de 15 dias; §3º-A/3º-B diligencias e portaria; §4º edital em 3 dias; **§4º-B intimacao eletronica IMPRESCINDIVEL havendo contato no contrato, 15 dias antes do edital** ⭐; §7º averbacao da consolidacao |
| **26-A** 🔴 | Regime do **imovel residencial do devedor** (exceto consorcio): §1º averbacao 30 dias depois; **§2º purga ate a AVERBACAO**; §3º referencial do 2º leilao; **§4º divida EXTINTA**; **§5º condicao resolutiva inerente a divida, que alcanca tambem a via judicial** — o credor nao escapa migrando de via |
| **27** 🔴 | Os dois leiloes: **60 + 15 dias**; **§2º no 2º leilao o credor PODE aceitar 50% da avaliacao, a seu exclusivo criterio** — faculdade do credor, **jamais direito do arrematante**; §2º-B **preferencia**; §3º, II inclui a comissao do leiloeiro nas despesas; §4º sobra em 5 dias; **§5º-A saldo remanescente**; **§6º REVOGADO**; §6º-A calculo; §7º denuncia da locacao 30/90; §10 leilao eletronico; **§§11-12 constricoes nao obstam + sub-rogacao no saldo** |
| **27-A** 🔴 | Excussao **simultanea ou sucessiva** de varios imoveis; §1º a ordem e escolhida pelo credor **salvo clausula em contrario** — alavanca de quem redige do lado do devedor; **§3º prazo de 30 dias**, nao 60 |
| **30** ⭐ | Reintegracao de posse **liminar, em 60 dias**, assegurada **tambem ao arrematante**. **§unico: consolidada ou arrematada, NENHUMA discussao sobre clausulas ou requisitos obsta a reintegracao — EXCETO a exigencia de notificacao** |
| **37-A** | Taxa de ocupacao de **1% ao mes sobre o valor do art. 24, VI** desde a CONSOLIDACAO ate a imissao — para o arrematante e **credito, nao custo** |
| **37-B** | Locacao maior que 1 ano sem anuencia escrita e **ineficaz** perante o fiduciario e sucessores |
| **39** | Incisos I e II **REVOGADOS** pela 14.711 (art. 18, V, "b") — o II era o que mandava aplicar os arts. 29 a 41 do DL 70/66 |

## 🔴 A trava do IPTU e do condominio — por que o art. 24, §2º nao serve
A MP 1.162/2023 **FOI convertida** (Lei 14.620/2023) — 🚫 **e proibido escrever que "nao vingou"**, porque a parte contraria refuta em dois cliques no cabecalho do Planalto. **Morreu o ENDERECO, nao a regra:** a MP inseriu no **art. 24, §2º**; a lei de conversao promulgou no **art. 23, §2º**, em vigor.
⚠️ **Por que o erro nasce, e por que explicar isso importa:** o compilado exibe **os dois dispositivos na tela, sem tachado** — quem faz grep de "IPTU" acha os dois. O que desqualifica o art. 24, §2º e a **atribuicao apenas a MP**, ou seja, **sem eficacia**. Sem essa explicacao o leitor abre o Planalto, ve o artigo la e desconfia da regra inteira.
⚠️ **Limite honesto, na mesma frase:** o art. 23, §2º rege **fiduciante x fiduciario** e **nao resolve sozinho a divida do ARREMATANTE** — para ele valem o condominio (edital informando) e o Tema 1.134. Ancora: `lei-9514-consolidada.md` **AVISO 3**.

## As inversoes de 31/10/2023 (conselho antigo que virou errado)
1. **Leilao negativo deixou de quitar a divida como regra** (§5º-A): o devedor **continua obrigado pelo saldo**, cobravel por execucao e com excussao das demais garantias. **Excecao:** imovel residencial do devedor (26-A, §4º).
2. **Penhora nao trava mais o leilao** (§11): constricoes **sobre o direito real de aquisicao do fiduciante** nao obstam consolidacao nem venda; os titulares se sub-rogam no **saldo** (§12). ⚠️ **Limite literal:** o §11 fala do direito **do fiduciante** — constricao sobre a **propriedade** ou vinda de outra relacao **nao esta coberta**.
3. **A defesa do fiduciante foi comprimida a um eixo unico** (30, §unico): **atacar a intimacao, nao o preco**.
4. **A intimacao eletronica virou pre-requisito** (26, §4º-B) — somada ao item 3, e a tese de nulidade mais forte que restou.

## Regras de ouro
- **A purga tem marco proprio:** no residencial, **ate a averbacao** da consolidacao (26-A, §2º) — nao ate o leilao.
- **Tema 1.288 e precedente vivo sobre texto morto:** versava o art. 39, II, hoje revogado. Citar assim.
- ✅ **Denuncia da locacao pelo arrematante — o marco esta ancorado.** Sao **dois** prazos distintos: os **90 dias** da Lei 8.245, art. 8º, **§2º, contados do REGISTRO da venda ou do compromisso** (perdido, presume-se concordancia com a manutencao do contrato), e a denuncia de **30/90 dias** do art. 27, §7º. ⛔ **Nunca contar da alienacao:** o registro e posterior, e o marco errado declara morto um prazo que ainda corre → `context/lei-8245-locacao.md`, **grep o artigo e leia a faixa**.
- 🟡 **Direito intertemporal** de contratos e procedimentos anteriores a 31/10/2023: a 14.711 **nao traz regra de transicao** — conferir antes de protocolar.
- Cross-link soft: o **contrato** de AF (revisao, superendividamento) e do `bancario-adv-os`; a **relacao** de AF e o registral, do `direito-imobiliario-adv-os`; aqui e a **mecanica do leilao**.

## Entrega obrigatoria final
Dispositivo com artigo, paragrafo e inciso + faixa lida + prazo com **marco inicial** + o que mudou em 2023 + skill de destino.

## Guard
Nao citar art. 24, §2º como fonte do encargo do fiduciante. Nao apresentar leilao negativo como quitacao fora do 26-A. Nao estender o §11 alem do **direito do fiduciante**. Nao contar os 90 dias do locatario da alienacao — o art. 8º, §2º conta do **REGISTRO**. Fecha por `validador-leiloes` e `suprema-corte-leiloes` — a tabela das 11 correcoes e a lista 🟡 integral ficam la, nao aqui.
