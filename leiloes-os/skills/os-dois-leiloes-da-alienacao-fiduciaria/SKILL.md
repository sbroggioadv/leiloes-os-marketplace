---
name: os-dois-leiloes-da-alienacao-fiduciaria
description: "O art. 27 da Lei 9.514/97 completo — os dois leiloes do extrajudicial de alienacao fiduciaria: 60 dias para o primeiro e 15 para o segundo, o minimo de cada um, a comissao do leiloeiro como DESPESA dedutivel (regime oposto ao judicial), a sobra devolvida em 5 dias, o saldo remanescente do §5º-A que inverteu o conselho antigo, o direito de preferencia do §2º-B com a tabela purga x preferencia do Tema 1.288/STJ, e as constricoes dos §§11-12 que deixaram de travar o leilao. Carrega o alerta do homonimo mais perigoso do dominio: os 50% do segundo leilao sao FACULDADE do credor, a seu exclusivo criterio, e nao piso de preco vil nem direito do arrematante. Use em qualquer leilao de banco, e quando disserem quando sai o leilao, qual o valor minimo, o banco pode aceitar metade, sobrou dinheiro pra mim, ainda devo depois do leilao, tenho penhora na matricula."
---

# OS-DOIS-LEILOES-DA-ALIENACAO-FIDUCIARIA

> Camada 4. **O motor do extrajudicial.** Quatro das mudancas de 31/10/2023 estao dentro deste artigo, e tres delas **invertem** conselho que ainda circula como verdade.

## Anexos obrigatorios (context/)
- `context/lei-9514-consolidada.md` — §5 do anexo (art. 27 verbatim, **16 paragrafos**, um deles **revogado**), §5.1 (purga x preferencia), §5.2 e §5.3. ⚠️ **AVISO 2 antes de citar**: o caput ainda exibe "trinta dias" numa redacao superada — **o prazo vigente e 60 dias**. **Grep + ler a faixa**.
- `context/lei-14711-2023.md` — art. 9º, §§5º-8º: os **mesmos passos com numeros diferentes** no rito hipotecario — **grep + ler a faixa**.
- `context/jurisprudencia-leiloes.md` — Tema 1.288/STJ · REsp 2.165.101 🔴 monocratica · REsp 2.167.979/PB — **grep + ler a faixa**.
- `context/metodologia-leiloes.md` — **§7.1 (homonimo de criterio: os dois "50%")** e §10 (o relogio) — **grep + ler a faixa**.

## Objetivo
Devolver **as datas de cada leilao com o marco inicial**, **o valor minimo de cada um com a formula** e **o destino do dinheiro** — sobra, saldo remanescente ou nada — em vez de "o leilao vai sair por metade do valor".

## Metodologia
1. Confirmar a **averbacao da consolidacao** e a sua data — e dela que corre tudo (art. 26, §7º, da Lei 9.514).
2. Checar se o caso e **residencial do devedor** → `regime-do-imovel-residencial-26a` muda referencial e desfecho.
3. Montar os **dois minimos** com a formula, nao com percentual de ouvido.
4. Rodar a tabela dos paragrafos e apontar o que foi **cumprido / omitido**.
5. Fechar a conta: sobra (§4º), saldo remanescente (§5º-A + §6º-A) ou extincao (art. 26-A, §4º, da Lei 9.514).
6. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## O artigo, paragrafo a paragrafo — art. 27 da Lei 9.514

| § | O que decide |
|---|---|
| caput | 🔴 **1º leilao em 60 dias** contados do **registro da consolidacao**. A pagina do compilado ainda mostra "trinta dias" numa redacao superada |
| §1º | Lance do 1º leilao inferior ao valor do imovel (art. 24, VI, ou §unico, da Lei 9.514) ⇒ **2º leilao nos 15 dias seguintes** |
| §2º | 2º leilao: aceita-se o maior lance **>= divida + despesas + emolumentos + premios de seguro + encargos legais, inclusive tributos + contribuicoes condominiais**; **nao havendo**, o credor **pode**, a seu **exclusivo criterio**, aceitar lance de **pelo menos metade do valor de avaliacao** |
| §2º-A | Datas, horarios e locais **comunicados** ao devedor e ao terceiro fiduciante nos enderecos do contrato, **inclusive o eletronico** |
| §2º-B | **Preferencia** do fiduciante: da averbacao **ate a data do 2º leilao**, adquirir por divida + despesas + seguros + encargos + condominio + tributos + **ITBI e laudemio ja pagos pelo credor** + despesas de cobranca e leilao — **mais** os encargos e emolumentos da **nova aquisicao** |
| §3º | Definicoes: **I** divida (saldo na data do leilao) · **II** despesas — **inclui a comissao do leiloeiro** · **III** encargos do imovel |
| §4º | **Sobra devolvida em 5 dias**, incluida indenizacao de benfeitorias, com **reciproca quitacao**; afasta a parte final do art. 516 do Codigo Civil |
| §5º | 2º leilao sem lance no referencial: o fiduciario fica com a **livre disponibilidade** e **exonerado** do §4º |
| §5º-A | 🔴 **Produto insuficiente ⇒ o devedor CONTINUA obrigado pelo saldo**, cobravel por **execucao** e com **excussao das demais garantias** — ressalvado o art. 26-A, §4º, da Lei 9.514 |
| §6º | **REVOGADO** pela Lei 14.711/2023 (art. 18, V, "a") — acabou o termo de quitacao em 5 dias |
| §6º-A | Calculo do saldo: deduz-se **o referencial minimo do §2º** do valor **atualizado** da divida, incluidos encargos e despesas de cobranca |
| §7º | Locacao: denuncia com **30 dias** para desocupar, **desde que** denunciada em **90 dias da consolidacao** e havendo clausula especifica com **destaque grafico** |
| §8º | Encargos do imovel sao do **fiduciante ate a IMISSAO** do fiduciario na posse |
| §9º | Estende o §2º-B as consolidacoes de imoveis do **FAR** |
| §10 | Leiloes e editais **podem ser eletronicos** |
| §§11-12 | 🔴 Constricoes **sobre o direito real de aquisicao do fiduciante** — penhoras, arrestos, bloqueios, indisponibilidades — **nao obstam** consolidacao nem venda; os titulares **sub-rogam-se no saldo** |

## ⚠️⚠️ O HOMONIMO QUE MAIS CUSTA DINHEIRO — os dois "50%"

| "50%" | Base | O que realmente e |
|---|---|---|
| **50% da avaliacao** (judicial) | avaliacao | **preco vil** — regra **supletiva** do CPC, so quando o juiz nao fixou preco minimo no edital |
| **metade da avaliacao** no 2º leilao (§2º) | avaliacao | 🔴 **FACULDADE DO CREDOR, a seu exclusivo criterio.** **NAO e piso de vileza. NAO e direito do arrematante.** O credor pode simplesmente **nao aceitar** |

⛔ **Nunca transportar os 50% do CPC para o extrajudicial**, nem prometer ao investidor que "o segundo leilao sai por metade". E oferta que **depende do credor aceitar**. 🟡 A construcao judicial que anula abaixo de 50% no extrajudicial se apoia no **REsp 2.165.101**, decisao **MONOCRATICA** — a redacao honesta e ***"o STJ vem anulando"***, **nunca** "tese firmada em repetitivo" → `preco-vil-como-tese`.

## ⭐ Purga x preferencia — e a distincao virou tese
Depois da averbacao da consolidacao, **fora** do art. 26-A da Lei 9.514, o fiduciante **nao purga mais**: resta-lhe a **preferencia** do §2º-B, que custa **toda a divida** e ainda **paga tributos e emolumentos de nova aquisicao**. ✅ **Tema 1.288/STJ**: "resta ao fiduciante **tao somente** o exercicio do direito de preferencia". ⚠️ Citar com a qualificacao — **precedente vivo sobre texto morto**: versava o art. 39, II, da Lei 9.514, hoje revogado. Chamar o §2º-B de "purga tardia" e **erro material com impacto no calculo**.

## 🔴 As inversoes de 31/10/2023 (conselho antigo que virou errado)
1. **Prazo do 1º leilao: 30 ⇒ 60 dias.**
2. **O credor PODE aceitar metade da avaliacao no 2º leilao** — faculdade, jamais direito do arrematante.
3. **Leilao negativo deixou de quitar a divida como regra** (§5º-A). O §6º foi revogado coerentemente.
4. **Penhora nao trava mais o leilao** (§11). ⚠️ **Limite literal:** o §11 fala do direito **do fiduciante**. Constricao sobre a **propriedade**, ou vinda de outra relacao, **nao esta coberta** pela literalidade — e constricao averbada **antes** da alienacao fiduciaria e lacuna real (🟡) → `leitura-de-matricula`.

## ⚠️ Nao transportar regime entre as vias
- **Comissao:** aqui e **despesa dedutivel** (§3º, II) e sai do produto do leilao. No judicial, o arrematante paga **por fora** (CPC 901, §1º). **Regimes opostos** → `custo-total-real-e-precificacao`.
- **Sobra:** **5 dias** aqui (§4º) x **15 dias** no rito hipotecario (art. 9º, §8º, da Lei 14.711/2023).
- **Descricao do imovel:** ✅ **REsp 2.167.979/PB** (turma, nao repetitivo) — o edital deve refletir a situacao **atual**, e nao se vincula a descricao do contrato fiduciario.

## Regras de ouro
- **Todo prazo com o marco colado:** 60 dias do **registro da consolidacao**; 15 dias do **1º leilao**; preferencia ate a **data do 2º leilao**; 5 dias da **venda**.
- **Percentual sempre com a base junto.** Antes de comparar dois percentuais, confirmar que incidem sobre a **mesma base** (`context/metodologia-leiloes.md`, §7.1).
- **Nunca prometer desconto.** A media provada de desagio do mercado e **37,3%**, nao 70%.
- Cross-link soft: intimacao → `consolidacao-da-propriedade-e-intimacao` · residencial → `regime-do-imovel-residencial-26a` · varios imoveis → `excussao-multipla-e-concurso-de-credores` · saldo → `saldo-remanescente-e-quitacao` · vicios → `vicios-do-procedimento-extrajudicial`.

## Entrega obrigatoria final
Cronograma com **data de cada leilao e o marco de onde saiu**; os **dois minimos com a formula aberta**; a conta do **destino do dinheiro** (sobra, saldo ou extincao); a posicao da **preferencia do §2º-B** com prazo; e o efeito das **constricoes da matricula** com o limite literal do §11 declarado. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Nunca tratar a **metade da avaliacao do §2º** como piso de vileza ou direito do arrematante — e **faculdade do credor**. Nunca dizer que **leilao negativo quita** fora do art. 26-A da Lei 9.514. Nunca chamar a preferencia de **purga**. Nunca citar **REsp 2.165.101** como repetitivo. Nunca transportar a comissao do judicial para ca. Nunca estender o §11 a constricao sobre a **propriedade**. Sempre nomear o diploma junto do numero do artigo — **"art. 27" sozinho e citacao quebrada** (o numero designa varios diplomas no corpus). Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
