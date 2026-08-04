---
name: base-legal-leilao-judicial
description: "Fundacao legal do leilao judicial brasileiro como UM corpo so: CPC arts. 876-903 (adjudicacao, alienacao particular, edital, intimacoes, preco vil, parcelamento, auto e carta, e o relogio do art. 903) + art. 804 (ineficacia relativa) + art. 908 §1º (creditos propter rem sub-rogam-se no preco) + a Resolucao CNJ 236/2016, que nao e anexo opcional e sim o regulamento do art. 882, §1º. Devolve o dispositivo pela faixa lida no anexo, com prazo e MARCO INICIAL nomeados, nunca de memoria. Use ao montar qualquer peca, parecer ou impugnacao do lado judicial, quando o leiloes-master rodar o passo de fundacao, ou quando disserem qual artigo, onde esta na lei, base legal, fundamento do leilao judicial, o CPC diz o que, preco vil, prorrogacao de 3 minutos, comissao no judicial, intimacao do art. 889, prazo de 10 dias."
---

# BASE-LEGAL-LEILAO-JUDICIAL

> Camada 1. Fundacao. Nao redige peca: entrega o dispositivo **vigente**, pela faixa lida, para as camadas C2-C7 usarem. CPC e Res. CNJ 236 sao **um corpo so** — a Resolucao regulamenta o art. 882, §1º.

## Anexos obrigatorios (context/)
- `context/cpc-leilao-879-903.md` — arts. 876-903 + 804 + 826 + 908 §1º verbatim; a faixa **nao tem nota de alteracao** (conferido) — **grep o artigo e leia a faixa**, nunca despeje o anexo inteiro.
- `context/resolucao-cnj-236-2016.md` — os 36 artigos + a ficha oficial (Situacao **Vigente**, campo Alteracao **vazio**) — **grep + ler a faixa**.
- `context/jurisprudencia-leiloes.md` — quando o dispositivo tiver precedente atrelado (804/889, 891, 901) — **grep + ler a faixa**.

## Objetivo
Entregar a base legal exata do leilao judicial — artigo, paragrafo, inciso, prazo e **marco inicial** — para que nenhuma skill de C2 a C7 cite de memoria. Toda resposta sai nomeando a faixa do anexo que foi lida.

## Metodologia
1. Identificar o instituto: expropriacao, edital, intimacao, lance, pagamento, auto, carta, invalidacao.
2. Grep do artigo no anexo e **leitura da faixa inteira** — caput, incisos e paragrafos. Inciso lido pela metade e erro de peca.
3. Havendo precedente atrelado, trazer de `jurisprudencia-leiloes.md` **com a qualificacao** (repetitivo x turma x monocratica x pendente).
4. Devolver dispositivo + prazo com marco + efeito pratico + a skill de destino.
5. Fechar por `validador-leiloes` e `suprema-corte-leiloes`.

## O mapa da expropriacao (a ordem importa)
Adjudicacao (876-878 — e o **878 reabre a janela, com direito a nova avaliacao**) → alienacao por iniciativa particular (880, que gera **carta de alienacao**, nao de arrematacao) → leilao judicial, eletronico como regra (879, 881-903).

## Os dispositivos que decidem (contagens conferidas no anexo)

| Dispositivo | O que trava |
|---|---|
| **884 §unico** | O CPC **nao fixa percentual** de comissao: "estabelecida em lei ou arbitrada pelo juiz". Deposito em **1 dia**, contas em **2** |
| **885** | Preco minimo e **decisao judicial** — e alimenta a cascata do 891 |
| **886** | Edital com **6 incisos**; o **VI** (onus, recurso ou processo pendente) e o gatilho da desistencia do 903 §5º, I |
| **887 / 888** | Publicacao com **5 dias** de antecedencia; adiamento |
| **889** | **8 categorias fechadas**, cientificadas com **5 dias**. ⚠️ O **conjuge NAO esta na lista** — a intimacao dele tem sede na **penhora de imovel** |
| **804** | **6 paragrafos**: falta de intimacao gera **INEFICACIA relativa, nao nulidade**. Para o arrematante e **pior** — fica com o bem **e com o gravame**, que nao foi purgado perante quem nao foi intimado |
| **890** | Impedidos de arrematar; **inciso VI: advogado de qualquer das partes** |
| **891 §unico** | **Preco vil em cascata**: fixado preco minimo no edital, vil e o que fica **abaixo dele**; **so na ausencia** valem os 50% da avaliacao |
| **892 a 894** | Pagamento imediato; preferencia de familia **so em igualdade de oferta**; lance global; alienacao parcial |
| **895** | Parcelada: **25% a vista + 30 meses**. §7º **lance a vista sempre prevalece** · §6º a proposta **nao suspende o leilao** · §4º multa sobre a parcela inadimplida **somada as vincendas** |
| **896** | Imovel de incapaz: piso de **80%** |
| **897-900** | Arrematante remisso perde a caucao **e fica banido daquele leilao** |
| **901** | Auto lavrado de imediato; **carta e mandado so apos preco + comissao + despesas**; §2º exige **prova de pagamento do ITBI** na carta e indicacao dos onus |
| **902 + 826 + 877 §3º** | As **tres remicoes** — marcos e valores distintos. Nunca tratar como uma so |
| **903** | O relogio: assinado o auto, a arrematacao e perfeita, acabada e irretratavel; as 3 hipoteses do §1º so em **10 dias contados do APERFEICOAMENTO**; §4º acao autonoma com o arrematante como **litisconsorte necessario**; §5º, I desistencia por onus fora do edital; **§6º freio de ate 20% do valor atualizado do bem** |
| **908 §1º** | Creditos propter rem **sub-rogam-se no preco**, observada a preferencia |

## Resolucao CNJ 236/2016 — regulamento, nao apendice
Ficha oficial: **Vigente**, campo **Alteracao vazio**; em vigor desde 13/10/2016.
- **1º e 2º** — credencia-se o **leiloeiro pessoa fisica**, nao a plataforma; 3 anos de exercicio; §1º, V veda relacao societaria com outro credenciado.
- **7º** — comissao **no minimo 5%** a cargo do arrematante; §1º nao devida em desistencia, anulacao ou leilao negativo; **§3º devida em acordo ou remicao POSTERIORES a alienacao**; §4º deducao do produto.
- **11** — abertura do sistema com **5 dias**; o simultaneo ocorre no ultimo dia.
- **18** ⭐ — bens vendidos "no estado de conservacao em que se encontram, **sem garantia**, constituindo onus do interessado verificar". **E a base normativa do gate de due diligence**: a clausula "sem garantia" do edital **nao e abusiva em si**, e dizer que e seria erro.
- **21** — prorrogacao automatica de **3 minutos** no exclusivamente eletronico e **15 segundos** no presencial/simultaneo. Nao existe lance-surpresa no estalar do prazo.
- **22 §unico** proibe lance por e-mail ou intervencao humana · **27** o juiz pode determinar rastreamento de IP · **29** remocao e transferencia **por conta do arrematante** · **34** gravacao integral.

## Regras de ouro
- **Prazo sem marco nomeado nao sai daqui.** "10 dias" e incompleto: sao 10 dias **do aperfeicoamento (assinatura do auto)**, jamais da ciencia do vicio — o erro mais caro do dominio, e a razao textual do gate DUE-DILIGENCE-FIRST.
- **Comissao e despesas nao estao dentro do lance** (901 §1º): sao pagamento adicional e **condicao para a carta**. Um lance de R$ 1.000.000 custa **R$ 1.050.000** so de lance + comissao, antes de ITBI, emolumentos, carrego e desocupacao.
- **Nao transportar os 50% do CPC para o extrajudicial** — la a regua e propria (`base-legal-alienacao-fiduciaria`). E a regua do 891 **nao separa 1ª de 2ª praca**.
- **Nunca dar numero de aliquota de ITBI, emolumento fora de SP ou custas** — so a formula e a fonte a consultar.
- Cross-link soft: a execucao **ate a penhora** e do `execucao-adv-os`; daqui em diante e deste plugin. Leilao publico administrativo (Lei 14.133) e **gap declarado** — encaminhar, nunca improvisar.

## Entrega obrigatoria final
Dispositivo com artigo, paragrafo e inciso + faixa do anexo lida + prazo com **marco inicial** + efeito pratico + a skill de destino. Nunca "conforme o CPC" solto.

## Guard
Artigo que nao foi lido na faixa do anexo **nao entra**. Prazo, percentual ou piso sem ancora **nao entra**. Fecha por `validador-leiloes` e `suprema-corte-leiloes` (R1-R4). A tabela das **11 correcoes travadas** e a **lista 🟡 integral** vivem no `validador-leiloes`; as 21 verdades duras e o gate de due diligence, no `anti-alucinacao-leiloes` — apontar, nunca duplicar.
