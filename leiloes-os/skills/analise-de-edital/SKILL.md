---
name: analise-de-edital
description: "Auditoria clausula a clausula do edital de leilao contra as 16 armadilhas lidas em editais REAIS, somada a conferencia do art. 886 do CPC inciso a inciso — porque o inciso VI (onus, recurso ou processo pendente nao mencionado) e o gatilho do art. 903, §5º, I: provado o gravame fora do edital, o arrematante desiste e recebe o deposito de volta, e isso caduca em 10 dias contados do aperfeicoamento. E a prova [1] do gate de due diligence, e grita a clausula de debitos condominiais, porque le-la ANTES do lance decide quem responde pela divida. Use ao receber qualquer edital, antes de habilitar ou lancar, e quando disserem le esse edital, o que tem de armadilha aqui, posso confiar nesse leilao, a clausula sem garantia e abusiva, quanto vou pagar de comissao, o edital nao fala de onus."
---

# ANALISE-DE-EDITAL

> Camada 2. **Prova [1] do gate.** Le o edital com duas lentes ao mesmo tempo: o que ele **poe** (as 16 armadilhas) e o que ele **deveria conter e nao contem** (o art. 886). A segunda lente e a que vira dinheiro.

## Anexos obrigatorios (context/)
- `context/clausulas-armadilha-de-edital.md` — as 16 armadilhas com citacao literal de edital real (§2) e a **auditoria do art. 886 inciso a inciso** (§3) — **grep pela armadilha (`ARM-06`) ou pelo tema e leia a faixa**.
- `context/cpc-leilao-879-903.md` — arts. **886**, 887, 889, 890, 891 §unico e **903 §§2º, 5º e 6º** — **grep o artigo e leia a faixa**.
- `context/resolucao-cnj-236-2016.md` — arts. **18** (sem garantia), 11, 21, 22 §unico e 29 — **grep + ler a faixa**.
- `context/custo-total-do-arrematante.md` — §2 o percentual de comissao e §6 o debito condominial — **grep + ler a faixa**.
- `context/jurisprudencia-leiloes.md` — REsp 2.167.979/PB (descricao atual) e o condominio (§4) — **grep + ler a faixa**.

## Objetivo
Devolver um dossie com **cada clausula citada literalmente**, o risco concreto de cada uma e **o que checar** — mais a lista do que o art. 886 exige e o edital **omitiu**. Alimenta `risco-de-anulacao-do-certame`, `custo-total-real-e-precificacao` e o `parecer-go-nogo-lote`.

## Metodologia
1. **Auditar o art. 886 inciso a inciso** (tabela abaixo). O que faltar entra como achado nomeado, nunca como impressao.
2. **Varrer as 16 armadilhas**; para cada uma encontrada, transcrever a clausula **do edital em maos** — nao a do edital-ancora.
3. **Cruzar edital x matricula** (`leitura-de-matricula`): divergencia de descricao, area ou onus e o achado de maior valor.
4. **Extrair os numeros da conta**: percentual da comissao, debito condominial informado, encargos de plataforma, prazo de pagamento, multa de desistencia.
5. **Classificar cada achado**: risco de preco · risco de prazo · **municao de nulidade** · **porta de desistencia (886, VI)**. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## ⭐ A auditoria do art. 886 — e a ponte que transforma leitura em dinheiro

| Inciso | O que o edital deve trazer | Como auditar |
|---|---|---|
| I | Descricao do bem; em imovel, situacao e divisas | Confrontar com a **matricula**. Divergencia e ARM-03 e pode ser tese — a descricao deve refletir a situacao **ATUAL** (REsp 2.167.979/PB, **turma**) |
| II | Avaliacao, **preco minimo**, condicoes de pagamento e, se houver, a comissao | ⭐ **Havendo preco minimo fixado, e ele que define preco vil** (891 §unico) — nao os 50% |
| III | Lugar dos moveis, veiculos e semoventes | — |
| IV | Sitio na internet e periodo do leilao | Cruzar com a abertura **≥ 5 dias** (Res. CNJ 236, art. 11) |
| V | Local, dia e hora do 2º leilao presencial | — |
| **VI** ⭐ | **Mencao da existencia de onus, recurso ou processo pendente sobre o bem** | **E O GATILHO.** Onus real ou gravame **nao mencionado** viola o VI |

> ⭐ **A ponte:** provado onus real ou gravame **fora do edital**, o arrematante **desiste e recebe o deposito de volta imediatamente** — **CPC 903, §5º, I**. E a saida mais forte que ele tem.
>
> ⏰ **E caduca em 10 dias contados do APERFEICOAMENTO** (§2º) — a assinatura do auto —, **nunca da ciencia do vicio**. Por isso esta skill roda **antes** do lance.
>
> ⚠️ **O freio do §6º:** suscitar vicio **infundado** para forcar a desistencia e **ato atentatorio a dignidade da justica**, com multa de ate **20%** do valor atualizado do bem. **A auditoria e documental, nunca especulativa** — achado sem documento nao vira alegacao.

**Conferencia rapida do resto:** 887 (publicacao ≥ 5 dias) · **889** (as **8 categorias**, ≥ 5 dias — o **conjuge NAO esta na lista**) · 890 (impedidos; **VI: advogado de qualquer das partes nao arremata**) · Res. CNJ 236 arts. 11, **21** (prorrogacao 3 min / 15 s), 22 §unico (proibido lance por e-mail) e 29 (remocao por conta do arrematante) · IN DREI 52 art. 74, XXIII (**nome e matricula do leiloeiro no edital**).

## As 16 armadilhas — as que decidem o negocio

| # | Armadilha | O que checar |
|---|---|---|
| **ARM-06** ⭐ | **Debito condominial quantificado** | **A de maior impacto** — bloco abaixo |
| ARM-01/02 | "Sem garantia" · renuncia a vicio oculto | Vistoria; **acesso negado se registra por escrito ANTES do lance** |
| ARM-03 | **Ad corpus** | Matricula x IPTU x planta; construcao averbada e habite-se; **orcar a regularizacao** |
| ARM-04 / 07 | Ocupado por conta do adquirente · encargos **desde a arrematacao**, nao da posse | **QUEM** ocupa (`situacao-possessoria`) e o carrego: meses ate a posse x (cota + IPTU) |
| ARM-05 | Catch-all de onus | Ler a **ressalva ao lado** e listar o que ficou de fora — o risco mora ali |
| ARM-08 | Laudemio, emolumentos, escritura | Matricula: e **foreiro**? Emolumento pela **MAIOR base** |
| ARM-09/10 | Comissao **por fora** e irreversivel · **7%** | **Ler o percentual em CADA edital** — nao assumir 5% |
| ARM-11/12 | Desistencia **10% a 25% do lance** + banimento · pagamento em **24 h** com caucao de **20% do lance** | Recurso liquido **confirmado** antes de habilitar |
| ARM-13/14 | Penhora no rosto dos autos · zoneamento e convencao vinculam | **Ler o processo indicado** (credores e preferencia do 908); convencao mata tese de investimento **depois** do lance |
| ARM-15 | O leiloeiro se exime do pos-arrematacao | Orcar honorarios do pos **como custo de aquisicao** |
| ARM-16 | Edital de 2026 fundado na **IN DNRC 113/2010** | 🟡 **O ato revogatorio nao foi aberto**: e **desatualizacao de fundamentacao, nao nulidade provada**. Nao sustentar nulidade por isso isolado — usar como **gatilho para auditar o edital inteiro** → `validador-leiloes` |

## ⭐⭐ ARM-06 — a clausula que decide quem paga o condominio
**Ler a clausula de debitos condominiais ANTES do lance decide a responsabilidade.** Em edital real: **R$ 53.374,15** de debito + **R$ 5.337,41** de honorarios sobre avaliacao de **R$ 136.142,37** — **39% da avaliacao**.
- **Edital que INFORMA a divida ⇒ o arrematante RESPONDE** (*propter rem*) **+ sucessao processual**. Orientacao **CONSOLIDADA** (REsp 2.042.756/SP mantido pelo AgInt nos EREsp, **2a Secao, UNANIME, 13/05/2026**). 🚫 **PROIBIDO escrever "a materia esta em aberto no STJ".**
- **Edital OMISSO** ⇒ leitura *a contrario* do **CPC 908, §1º**, com lastro de 2º grau: **tese de defesa bem fundamentada, JAMAIS regra pacifica** — ha **REsp 1.299.081/SP** em sentido contrario (falimentar, inteiro teor nao aberto). 🟡 **Marcar como tese, dizer que o inteiro teor nao foi aberto e rotear ao `validador-leiloes` antes de protocolar.**
- ⚠️ **A clausula de sub-rogacao no edital nao e garantia:** a protecao do 908, §1º depende de o credito estar **comprovado e habilitado**. Nao habilitado o condominio, a natureza *propter rem* puxa a divida para o imovel.
- ⚠️ **Tema 1.266 e materia DIVERSA** — nao citar como saida. Regime completo em `debitos-propter-rem`.

## Regras de ouro
- ⛔ **A clausula "sem garantia" NAO e abusiva em si** — reproduz o **art. 18 da Res. CNJ 236/2016**, que poe o onus de verificar **no interessado**. Ataca-la e **tese perdida** e queima a peca. **Ataca-se o edital que descumpre o 886, nao o que avisa.**
- **Comissao: 5% e PISO, nao teto, e nao existe teto** — **7% em leilao JUDICIAL e licito**. ⭐ O eixo de ataque e **TEMPORAL**: impugnar **ANTES do lance**; nao impugnado e pago, **consolida-se**. 🟡 No **extrajudicial** o raciocinio **nao se transporta** (nenhum julgado localizado) — marcar e rotear ao `validador-leiloes`.
- ✅ **Achado positivo do mercado:** nenhum dos tres editais-ancora joga **tributo anterior** no arrematante. Encontrar hoje um que jogue e **anomalia** e clausula **invalida** (Tema 1.134).
- ⛔ **Nao afirmar situacao do imovel a partir do edital** — ele e a versao do vendedor. Onus, ocupacao e area se provam na **matricula** e na apuracao: edital lido **nao** substitui as provas [2], [3] e [4].
- **Nunca dar numero** de aliquota de ITBI, emolumento fora de SP ou custas — so a formula e a fonte.

## Entrega obrigatoria final
Dossie com: (a) **tabela do art. 886** marcando **atendido / omisso**; (b) cada armadilha com a **clausula literal do edital em maos** + risco + o que checar; (c) os **numeros que vao para a conta**; (d) os achados que viram **municao de nulidade** ou **porta do 903, §5º, I**, com o prazo de 10 dias nomeado; (e) o que ficou **pendente de documento**. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Nenhuma afirmacao sobre o imovel sai daqui **sem documento lido**. Clausula so entra citada **literalmente**. Achado especulativo **nao vira alegacao** — o §6º pune com ate 20%. Nunca "sem garantia e abusiva" · nunca "a materia esta em aberto no STJ" · nunca assumir 5% de comissao sem ler o edital · nunca nulidade fundada apenas na IN DNRC 113/2010. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
