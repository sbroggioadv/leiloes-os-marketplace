---
name: estrategia-de-lance-e-habilitacao
description: "Operacao do lance, e SO roda depois do parecer GO — nenhuma estrategia de lance existe sem as 4 provas do gate de due diligence. Cobre a due diligence do LEILOEIRO por nome e matricula (credencia-se a pessoa fisica, nunca a plataforma, e a Junta publica a situacao regular, licenciado ou suspenso), os prazos reais de cadastro e habilitacao que fazem quem descobre o lote na vespera nao conseguir lancar, a prorrogacao automatica de 3 minutos no eletronico e 15 segundos no presencial (que mata a estrategia de sniping), os meios de pagamento e o prazo de 24 horas, a multa de desistencia com banimento do cadastro, e o que fazer quando o incremento minimo nao e publicado — nenhuma das 5 plataformas publica. Use depois do GO e quando disserem como dou o lance, vou me habilitar, quanto lanco, e melhor lancar no fim, o leiloeiro e confiavel, posso parcelar, aceita PIX."
---

> **🖱️ Escolhas = botoes:** nas perguntas de lista fechada use **AskUserQuestion** (max. 4 por pergunta).

# ESTRATEGIA-DE-LANCE-E-HABILITACAO

> Camada 2. Publico 💰. **Esta skill e a ULTIMA do gate, nunca a primeira.**

## ⛔ DEPENDENCIA DO GATE — declarada na abertura
**Nao produz estrategia, numero de lance nem plano de habilitacao sem as 4 provas documentais:** **[1] EDITAL** (`analise-de-edital`) · **[2] MATRICULA** (`leitura-de-matricula`) · **[3] OCUPACAO** (`situacao-possessoria`) · **[4] DEBITOS** (`debitos-propter-rem`), mais `risco-de-anulacao-do-certame` e `custo-total-real-e-precificacao`, **fechados em `parecer-go-nogo-lote` com veredito GO ou GO-CONDICIONADO**.

**Faltando qualquer prova, esta skill RECUSA e devolve ao gate** — a resposta e **NO-GO por insuficiencia de prova**, nunca "provavelmente esta ok" nem "de uma olhada e lance com cuidado".

**A razao e TEXTUAL:** o **CPC 903, §2º** conta os 10 dias do **APERFEICOAMENTO da arrematacao** (a assinatura do auto), **nao da ciencia do vicio** — **due diligence pos-lance chega tarde por construcao da lei**.

## Anexos obrigatorios (context/)
- `context/metodologia-leiloes.md` — **§3 o gate** e **§8 os selos** — **ler antes de operar**.
- `context/resolucao-cnj-236-2016.md` — **11** (abertura ≥ 5 dias) · **21** (3 min / 15 s) · **22 §unico** (proibido lance por e-mail) · 27 (rastreamento de IP) · 29 — **grep + ler a faixa**.
- `context/leiloeiro-decreto-21981-in-drei-52.md` — IN DREI 52 arts. **60** (credencia-se a pessoa fisica), **74 XXIII** (nome e matricula no edital), **87**, **89 VII** (a Junta publica a situacao) — **grep + ler a faixa**.
- `context/custo-total-do-arrematante.md` — §3 (encargos e gargalos de plataforma) e §2 (comissao) — **grep + ler a faixa**.
- `context/clausulas-armadilha-de-edital.md` — **ARM-11** (desistencia e banimento) e **ARM-12** (24 horas + caucao) — **grep + ler a faixa**.
- `context/cpc-leilao-879-903.md` — **890** (impedidos) · 892-894 · **895** · 896 · **897-900** (remisso) — **grep + ler a faixa**.

## Metodologia
1. **Confirmar o veredito do gate.** Sem GO ou GO-CONDICIONADO, parar aqui.
2. **Pergunta em botoes (lista fechada): como sera o pagamento?** — **a vista, recurso confirmado** · **proposta parcelada do art. 895** · **financiamento bancario** · **ainda nao definido**. ⚠️ As duas ultimas sao **bandeira vermelha**: financiamento **nao roda em 24 horas** e "nao definido" nao habilita.
3. **Auditar o leiloeiro** (bloco abaixo) — antes de cadastrar.
4. **Montar a linha do tempo** de cadastro, validacao e habilitacao **contando de tras para frente** a partir da data do pregao.
5. **Fixar o numero:** o **teto vem de `custo-total-real-e-precificacao`**, e **lanca-se o teto MENOS a comissao**.
6. **Escrever o plano de pregao** — quando entrar, ate onde ir, quando parar. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## ⭐ Due diligence do LEILOEIRO — por nome e matricula
**Credencia-se o LEILOEIRO pessoa fisica, nao a plataforma** (IN DREI 52, art. 60 · Res. CNJ 236, arts. 1º e 2º). A plataforma e **atividade-meio**, e o art. 60 **nao afasta a responsabilidade pessoal** do leiloeiro.
- **Procurar "a empresa" na Junta Comercial nao devolve nada.** A busca e por **nome + matricula**, cruzando a **lista do tribunal** com a **lista da Junta** — o **art. 89, VII** obriga a Junta a publicar a **situacao: regular / licenciado / suspenso**.
- O **art. 74, XXIII** exige **nome e matricula do leiloeiro no proprio edital**: se nao estiverem la, ja e achado.
- **Leiloeiro e prepostos nao dao lance** (Res. CNJ 236, art. 3º); autocompra e punida com **multa** (Dec. art. 36) — **nao com destituicao**.
- 🟡 **Nao usar em peca** o bloco de dispositivos de 1932 cuja compatibilidade nao foi verificada — entre eles a **prisao do leiloeiro como depositario remisso** (Dec. 21.981 art. 27, §4º) diante da **SV 25/STF** → `base-legal-leiloeiro` e `validador-leiloes`.

## ⏱️ Os prazos que fazem perder o lote antes do pregao
- **Cadastro NAO e habilitacao.** Todas as plataformas exigem **habilitacao por leilao**, alem do cadastro.
- **O gargalo real e a validacao do cadastro:** uma plataforma avisa que a validacao *"tem prazo de ate 3 (tres) dias uteis para ser **iniciada**"* — iniciada, nao concluida. ⭐ **Quem descobre o lote na vespera nao consegue dar lance.**
- **Abertura do sistema com ≥ 5 dias** e o simultaneo no ultimo dia (Res. CNJ 236, art. 11); publicacao do edital com **≥ 5 dias** (CPC 887).
- **Meios de pagamento:** conferir no edital e na plataforma — **uma das cinco verificadas VEDA PIX**. Pagamento tipicamente em **24 horas**, as vezes com **caucao de 20% do lance no ato** (ARM-12). **Recurso liquido confirmado ANTES de habilitar.**

## 🔴 Sniping nao funciona — a prorrogacao e automatica
**Res. CNJ 236, art. 21:** no leilao **exclusivamente eletronico**, cada lance nos **3 minutos** finais empurra o fechamento em mais 3, **recursivamente**; no **presencial ou simultaneo**, **15 segundos**. **Nao existe lance-surpresa no estalar do prazo** — quem guarda o lance para o ultimo segundo **so perde dinheiro a toa**, porque a disputa continua de qualquer forma.
- **Proibido lance por e-mail** ou qualquer intervencao humana na coleta e registro (art. 22, §unico); o juiz pode determinar **rastreamento de IP** (art. 27 Res. CNJ 236).
- 🟡 **Incremento minimo: NENHUMA das 5 plataformas publica.** E parametro definido **lote a lote no sistema**, e por isso **e impossivel calcular de antemao o custo de cobrir um lance**. ⛔ **Dizer isso ao operador — nunca estimar o incremento.** Consequencia pratica: levar **folga** entre o ultimo lance planejado e o teto, porque o passo real so aparece no pregao.

## As travas do CPC no momento do lance
- **890, VI:** **advogado de qualquer das partes nao arremata** — impedimento que vicia na origem.
- **892:** pagamento imediato; a **preferencia de familia** so vale **em igualdade de oferta**.
- **896:** imovel de incapaz tem piso de **80%**.
- **895 — a parcelada NAO reserva o bem:** **§7º qualquer lance a vista sempre prevalece** e **§6º a proposta nao suspende o leilao**; minimo **25% a vista** + saldo em ate **30 meses**, e a multa do §4º incide sobre a parcela inadimplida **somada as vincendas**. Detalhe em `arrematacao-parcelada-895`.
- **897-900 e ARM-11 — o custo de errar o lance:** o remisso **perde a caucao e fica banido daquele leilao**; os editais praticam **10% (judicial) a 25% (extrajudicial) do lance** de perda **sem receber o imovel**, e o **cadastro e banido da plataforma, junto com usuarios vinculados a ele**. **O percentual varia muito entre editais: ler antes do pregao.**
- ⭐ **Comissao: impugnar ANTES do lance ou nao impugnar.** 5% e **piso sem teto**, e **7% no judicial e licito**; publicado o edital, houve ciencia dos termos — **nao impugnado e pago, consolida-se**. 🟡 No **extrajudicial** o raciocinio **nao se transporta** (nenhum julgado localizado) → `validador-leiloes`.

## Regras de ouro
- **Lance o teto MENOS a comissao.** A comissao e somada **por fora** (901, §1º) e e **condicao para a carta**.
- **O plano de saida entra antes do plano de entrada:** teto, passo e **o ponto em que se para**. Disputa vencida acima do teto e prejuizo com cara de vitoria.
- ⛔ **Nao habilitar sem recurso liquido confirmado** e sem ter lido a clausula de inadimplemento **daquele** edital.
- ⛔ **Nao opinar sobre lance com prova faltando** — a resposta e devolver ao gate, sempre.
- **Nunca prometer desconto de 70%** (a media provada e **37,3%**) nem dizer que "leilao e seguro".
- Cross-link soft: a conta e o teto vem de `custo-total-real-e-precificacao`; o veredito, de `parecer-go-nogo-lote`; a parcelada, de `arrematacao-parcelada-895`; auto e carta, de `arrematacao-auto-e-carta`.

## Entrega obrigatoria final
Plano com: (a) **veredito do gate** citado; (b) **auditoria do leiloeiro** (nome, matricula, situacao na Junta, fonte consultada); (c) **linha do tempo** de cadastro, validacao e habilitacao com folga; (d) **meio de pagamento** confirmado e o prazo do edital; (e) **teto, valor a lancar (teto menos comissao) e o ponto de parada**; (f) o aviso do **incremento nao publicado** e da **prorrogacao automatica**; (g) o **custo de desistir** daquele edital. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
**Sem as 4 provas e sem GO, esta skill nao opera** — recusa e devolve ao gate. Nunca estimar **incremento minimo**. Nunca ensinar sniping como estrategia. Nunca assumir 5% de comissao sem ler o edital, nem PIX sem conferir a plataforma. Nunca lancar o teto cheio. Nunca afirmar situacao do imovel — isso e das provas [1] a [4]. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
