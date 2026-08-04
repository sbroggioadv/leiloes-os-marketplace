---
name: risco-de-anulacao-do-certame
description: "⭐ O fosso do plugin: responde a pergunta que nenhum SaaS de leilao responde — este leilao pode CAIR depois de eu pagar? Cruza intimacao, avaliacao, publicidade, edital e legitimacao contra as teses vigentes, e separa o que anula de fato do que so parece. No judicial mostra que a falta de intimacao de titular de direito real gera INEFICACIA do art. 804, nao nulidade — o que para o arrematante e PIOR, porque ele fica com o imovel E com o gravame nao purgado. No extrajudicial aponta o eixo que restou: a intimacao eletronica imprescindivel do art. 26, §4º-B e o filtro do §15 do art. 9º da Lei 14.711, que mata metade dos casos de hipoteca. E o espelho defensivo da mesma municao que a camada de defesa do devedor usa no ataque. Use antes do lance e quando disserem esse leilao pode ser anulado, e seguro arrematar aqui, e se o devedor recorrer, posso perder o imovel depois de pagar, o leilao tem vicio."
---

# RISCO-DE-ANULACAO-DO-CERTAME ⭐

> Camada 2. **O fosso.** As outras skills do gate perguntam *quanto custa* e *o que vem junto*. Esta pergunta **se o negocio sobrevive** — e e a unica coisa que nenhum dos 8 SaaS concorrentes analisa. E o **espelho defensivo** da municao que a C6 usa no ataque: ler dos dois lados e o que da a resposta honesta.

## Anexos obrigatorios (context/)
- `context/cpc-leilao-879-903.md` — **889** (as 8 categorias) · **804** (ineficacia, 6 §§) · **887** (publicidade) · **890** (impedidos) · **891 §unico** (preco vil em cascata) · **903** (o relogio) — **grep o artigo e leia a faixa**.
- `context/lei-9514-consolidada.md` — **26 §§3º-A, 3º-B, 4º e 4º-B** (intimacao e edital) · **26-A §2º** (purga ate a averbacao) · **30 §unico** (so a notificacao obsta) — **grep + ler a faixa**.
- `context/lei-14711-2023.md` — **art. 9º, §15** (o filtro da clausula expressa) e o rito do §§1º-10 — **grep + ler a faixa**.
- `context/jurisprudencia-leiloes.md` — REsp 2.167.979/PB · REsp 2.165.101 🔴 · REsp 2.135.500 · Tema 982 · **REsp 2.171.564/SP** 🔴 pendente — **grep + ler a faixa**.
- `context/clausulas-armadilha-de-edital.md` — §3, a auditoria do art. 886 — **grep + ler a faixa**.

## Objetivo
Devolver um **grau de risco por vetor**, cada um com **o documento que o prova ou o afasta**, e traduzir isso em consequencia de lance: risco alto rebaixa o teto ou vira **NO-GO**; risco medio vira **GO-CONDICIONADO** com a condicao nomeada.

## Metodologia
1. **Fixar a via** — judicial x extrajudicial. Os vetores **nao sao os mesmos** e nao se transportam.
2. **Rodar os vetores** da via (tabelas abaixo), um a um, com o documento na mao.
3. **Cruzar [1]-[4]**: o que a matricula mostra e o edital nao menciona; quem consta como titular de direito real e nao aparece intimado; a avaliacao contra o lance minimo.
4. **Qualificar cada precedente** — repetitivo x turma x **monocratica** x **pendente**. Precedente sem qualificacao e municao que explode na mao.
5. **Fixar a posicao no relogio** do art. 903 e dizer o que ainda e possivel de cada lado.
6. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## Vetores do LEILAO JUDICIAL

| Vetor | O que checar | Consequencia correta |
|---|---|---|
| **Intimacao (889)** ⭐ | As **8 categorias fechadas**, com **≥ 5 dias**. ⚠️ O **conjuge NAO esta na lista** — esse mito derruba peca | 🔴 **INEFICACIA do art. 804, NAO nulidade** (903, §1º, II). Ver o bloco abaixo |
| **Edital (886)** | Inciso a inciso; o **VI** e o gatilho | Onus fora do edital ⇒ **903, §5º, I**: desiste e recebe o deposito de volta |
| **Descricao do bem** | Deve refletir a situacao **ATUAL** — **REsp 2.167.979/PB** (**turma, nao repetitivo**) | Divergencia grave e tese de nulidade |
| **Publicidade (887)** | Publicacao **≥ 5 dias** antes; abertura do sistema ≥ 5 dias (Res. CNJ 236, art. 11) | Vicio de publicidade atinge o certame |
| **Preco vil (891 §unico)** | **Cascata**: havendo preco minimo no edital, vil e o **abaixo dele**; **so na ausencia** valem os 50% | ⛔ Nao dizer "o CPC fixa 50%", nem "so na 1a praca", nem transportar os 50% ao extrajudicial |
| **Legitimacao (890)** | Impedidos de arrematar — **VI: advogado de qualquer das partes** | Arrematacao por impedido e vicio de origem |
| **Imovel de incapaz (896)** | Piso de **80%** | Abaixo disso o certame nao se sustenta |

### 🔴 Por que INEFICACIA e pior que nulidade para o arrematante
Falta de intimacao de titular de direito real **nao anula** o leilao: torna-o **ineficaz perante quem nao foi intimado** (CPC 804). O arrematante **fica com o imovel E com o gravame**, que nao foi purgado. **Nao e uma boa noticia disfarcada de tecnicidade** — e o cenario em que ele paga, mantem a aquisicao e ainda responde ao credor que ficou de fora. **Todo titular de direito real da matricula e um item de conferencia de intimacao.**

🟡 **`pas de nullite sans grief` no leilao judicial:** so ha snippets de busca, **nenhum acordao aberto**, e ha tensao real com a linha do extrajudicial — **nao presumir o recorte**. Reforco textual: o **804 fala em ineficacia**, que **nao depende de grief**. Marcar e **rotear ao `validador-leiloes`** antes de usar em peca.

## Vetores do LEILAO EXTRAJUDICIAL

| Vetor | O que checar | Peso |
|---|---|---|
| **Intimacao eletronica (26, §4º-B)** ⭐⭐ | Havendo contato eletronico no contrato, a intimacao por essa via e **IMPRESCINDIVEL**, com **15 dias** de antecedencia antes do edital | 🔴 **A tese de nulidade mais forte que restou** |
| **Intimacao pessoal e edital (26, §§3º-A, 3º-B, 4º)** | Diligencias, portaria, edital em 3 dias | Alto — a defesa se concentra aqui |
| **A compressao do art. 30, §unico** | Consolidada ou arrematada a propriedade, **nenhuma** discussao sobre clausulas ou requisitos obsta a reintegracao — **EXCETO a exigencia de notificacao** | 🔴 Define o campo: **atacar a intimacao, nao o preco** |
| **Purga (26-A, §2º)** | No residencial, a purga vai **ate a averbacao** da consolidacao — nao ate o leilao | Purga tempestiva desfaz tudo |
| **Registro do contrato** | **REsp 2.135.500** (3a Turma, **turma**): o registro e **requisito** para usar a via extrajudicial | Alto |
| **Filtro do §15 (14.711, art. 9º)** ⭐ | Na **hipoteca**, o rito novo so vale se o titulo trouxer, como **requisito de validade**, previsao expressa com mencao aos §§1º a 10 | 🔴 **Hipoteca anterior a 31/10/2023 tipicamente nao tem** — mata metade dos casos |
| **Preco vil no extrajudicial** | **REsp 2.165.101** | 🔴 **MONOCRATICA.** Escreva **"o STJ vem anulando"** — **NUNCA** "tese firmada em repetitivo" |

⚠️ **Tema 982/STF** valida o procedimento da Lei 9.514 **em abstrato** — **nao convalida vicio concreto**. Usar o Tema para dizer "logo este leilao e valido" e erro de leitura.

🔴 **REsp 2.171.564/SP** (ex-`AREsp 2.471.891`, 3a Turma, Rel. Min. Daniela Teixeira) esta **PENDENTE: sem julgamento, sem acordao, sem tese**. **NAO EXISTE tese do STJ estendendo o art. 886, VI ao edital extrajudicial** — quem alega nulidade de edital extrajudicial por omissao de onus funda-se no **dever de informacao e na boa-fe objetiva**, nao em precedente. ⚠️ **Rastrear pelo numero NOVO**; o antigo nao devolve andamento. **Se vier a ser julgado nesse sentido, abala editais ja realizados** — e por isso entra no gate de calendario do `validador-leiloes`.

## ⏰ O relogio decide o que ainda e possivel
- **Ate 10 dias do APERFEICOAMENTO** (assinatura do auto, **nao** da ciencia do vicio): as 3 hipoteses do **903, §1º** — invalidacao, ineficacia, resolucao — e as **3 portas de desistencia do §5º**, tudo **incidental nos autos**.
- **Depois da carta:** so **acao autonoma** (§4º), com o **arrematante como litisconsorte necessario**.
- ⚠️ **Freio do §6º:** vicio **infundado** e ato atentatorio, multa de ate **20%**. Risco se afirma **com documento**, nunca por suspeita.

## Regras de ouro
- **Risco alto nao e sinonimo de nao arrematar** — e teto rebaixado, condicao nomeada ou desistencia informada. O que o produto entrega e a **decisao consciente**, nao o medo.
- **Monocratica nunca vira repetitivo. Pendente nunca vira decidido. Afetado nao e tese.** Precedente sem selo ✅ no anexo exige **busca ao vivo** — o plugin nao inventa numero de REsp.
- **Vetor sem documento nao vira alegacao**: entra no relatorio como **pendencia de prova**, e pendencia de prova puxa o parecer para **NO-GO por insuficiencia de prova**.
- **O que anula no extrajudicial nao anula no judicial, e vice-versa.** Nao transportar vetor de uma via para a outra.
- ⭐ **ADIs 7600/7601/7608** (Pleno, 30/06/2025) validaram a Lei 14.711 **com balizas de conduta**: vedada perseguicao ao devedor e familiares, **apenas dados publicos**, proibida forca fisica ou psicologica. 🟡 Citar **as balizas**, que sao verificaveis — nao uma "tese literal".
- Cross-link soft: o ataque esta na C6 (`anulatoria-de-arrematacao-judicial`, `anulatoria-de-leilao-extrajudicial`, `nulidades-de-intimacao-e-notificacao`, `preco-vil-como-tese`); a lista fechada do 889, em `intimacoes-art-889-e-ineficacia`.

## Entrega obrigatoria final
Matriz **vetor · o que foi conferido · documento que prova · grau (alto / medio / baixo) · efeito no lance**, mais: a **posicao no relogio do 903**, os precedentes **com a qualificacao junto**, e a lista de **vetores nao verificados por falta de documento**. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Nunca afirmar vicio **sem documento** — o §6º pune com ate 20%. Nunca tratar a falta de intimacao do 889 como **nulidade**: e **ineficacia** do 804, e e pior. Nunca "o CPC fixa 50%". Nunca **REsp 2.165.101 como repetitivo**. Nunca **REsp 2.171.564/SP como tese existente**. Nunca **Tema 982 para convalidar vicio concreto**. Nunca transportar vetor entre as vias. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
