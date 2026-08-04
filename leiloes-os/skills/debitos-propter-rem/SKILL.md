---
name: debitos-propter-rem
description: "Responde quem paga as dividas anteriores do imovel arrematado em DOIS regimes que nao se misturam, nunca em resposta unica. Tributario: fechado A FAVOR do arrematante — Tema 1.134/STJ mais CTN 130, §unico, sub-rogacao sobre o PRECO e aquisicao originaria, com a modulacao do item XIII da ementa. Condominial: CONTRA o arrematante quando o EDITAL INFORMA a divida — ele responde propter rem e sofre sucessao processual, orientacao consolidada pelo REsp 2.042.756/SP mantido pela Segunda Secao por unanimidade em 13/05/2026. Proibido escrever que a materia esta em aberto no STJ; a brecha real e o edital OMISSO, e ela e tese de defesa, jamais regra. E a prova [4] do gate de due diligence. Use antes de qualquer lance e quando disserem quem paga o condominio atrasado, tem IPTU em aberto, o edital fala de divida, arrematei e o condominio esta me cobrando, a divida some com a arrematacao, e propter rem."
---

> **🖱️ Escolhas = botoes:** nas perguntas de lista fechada use **AskUserQuestion** (max. 4 por pergunta).

# DEBITOS-PROPTER-REM

> Camada 2. **Prova [4] do gate.** Aqui a resposta e **sempre dupla**: tributo e condominio seguem regimes **opostos**. Quem responde "some tudo na arrematacao" ou "voce herda tudo" erra metade das vezes — e e exatamente o que os 8 SaaS concorrentes fazem.

## Anexos obrigatorios (context/)
- `context/jurisprudencia-leiloes.md` — §3 Tema 1.134 e a modulacao · §4 o condominio (REsp 2.042.756/SP + AgInt nos EREsp) · Sumula 478 · Tema 1.266 como **materia diversa** — **grep o precedente e leia a faixa**.
- `context/cpc-leilao-879-903.md` — **908 §1º** (creditos propter rem sub-rogam-se no preco, observada a preferencia) — **grep + ler a faixa**.
- `context/custo-total-do-arrematante.md` — §6, os dois regimes com os numeros reais de edital — **grep + ler a faixa**.
- `context/clausulas-armadilha-de-edital.md` — **ARM-06** (debito quantificado) e ARM-05 (catch-all) — **grep + ler a faixa**.
- `context/lei-9514-consolidada.md` — **AVISO 3** e o **art. 23, §2º** (encargo do fiduciante) — **grep + ler a faixa**.

## Objetivo
Devolver, divida por divida, **quem responde**, **com que fundamento** e **com que grau de certeza** — e transformar isso em numero para `custo-total-real-e-precificacao` e em veredito para o `parecer-go-nogo-lote`.

## Metodologia
1. **Pergunta 1 (botoes, lista fechada): o edital informa divida condominial?** — **sim, com valor** · **sim, sem valor** · **e omisso** · **ainda nao li o edital**. A ultima opcao **para o fluxo**: sem `analise-de-edital` nao ha resposta, e o veredito e **NO-GO por insuficiencia de prova**.
2. **Separar por natureza**: tributo (IPTU, taxas, contribuicao de melhoria) · **condominio** · outros (concessionarias, ambiental, associacao — ARM-05).
3. **Levantar com documento**: certidoes negativas municipais e de concessionarias, **declaracao de debito atualizada** da administradora ou do sindico, e a **conferencia nos autos** de o condominio estar **habilitado**.
4. **Aplicar o regime** de cada natureza (blocos abaixo).
5. **Lancar na conta**: valor certo, risco quantificado ou R$ 0 — **nunca "provavelmente nao ha"**.
6. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## ✅ Regime 1 — TRIBUTARIO: fechado A FAVOR do arrematante
**Tema 1.134/STJ** (1a Secao, j. 09/10/2024, transito 12/12/2024): e **invalida** a clausula de edital que atribui ao arrematante os debitos **tributarios** anteriores. A sub-rogacao ocorre **sobre o PRECO** (**CTN, art. 130, §unico**), e a aquisicao em hasta publica e **originaria**.

**Na conta: R$ 0** de tributo anterior — **desde que** o edital tenha sido **publicizado apos a publicacao da ata de julgamento** (modulacao), **ou** haja **acao judicial ou pedido administrativo pendente**, hipotese de **aplicacao imediata**.

- ⭐ **Como citar a modulacao:** ela esta no **item XIII da ementa**, e o verbo e **"publicizados"**. **Citar pelo item XIII ou pelo voto — nunca so pelo dispositivo**, que transcreve apenas a tese.
- 🟡 **A DATA da ata de julgamento NAO e declarada na fonte.** A praxe usa **24/10/2024** (publicacao do acordao), mas isso e **convencao, nao texto**. Afirmar a data como certa e inventar: escrever a ressalva ao lado e **rotear ao `validador-leiloes`** antes de protocolar.
- ⚠️ **Tema 1.134 NAO cobre condominio** — o acordao **nao trata** de despesas condominiais. E a correcao nº 1 do plugin.
- ✅ **Achado de mercado:** nenhum dos tres editais-ancora joga tributo anterior no arrematante — **o mercado ja se ajustou**. Encontrar hoje um que jogue e **anomalia** e clausula **invalida**.

## 🚨 Regime 2 — CONDOMINIAL: pode inverter o sinal do negocio
**Com o edital INFORMANDO a divida, o arrematante RESPONDE** (*propter rem*) **e sofre sucessao processual**. Orientacao **CONSOLIDADA**: REsp 2.042.756/SP (3a Turma, **3x2**, j. 12/11/2024) mantido pelo **AgInt nos EREsp 2.042.756/SP, 2a SECAO, UNANIME, j. 13/05/2026** — inadmitido por **ausencia de divergencia atual**, com os **dois vencidos da Turma participando sem divergir**. A divisao 3x2 era **intra-turma**, nao inter-turmas.

🚫 **PROIBIDO escrever "a materia esta em aberto no STJ"** — a Corte teve a via formal de uniformizacao e **a recusou**. Tambem proibido: "divergencia real", "tese em construcao", "racha".

**Edital OMISSO — a brecha real, e ela e TESE:** leitura *a contrario* do **CPC 908, §1º**, com lastro de **2º grau**. 🟡 **Nenhum acordao do STJ afirma a proposicao inversa**, e ha **REsp 1.299.081/SP** em sentido contrario (contexto falimentar, **inteiro teor nao aberto**). Escrever como **tese de defesa bem fundamentada**, dizer que o inteiro teor nao foi aberto, e **rotear ao `validador-leiloes`** antes de protocolar. **Jamais como regra pacifica.**

⚠️ **Tema 1.266 e materia DIVERSA** (penhora de imovel alienado fiduciariamente por divida condominial) — **afetado, sem tese e sem suspensao nacional**. **Nao citar como saida do arrematante.**

⚠️ **Sumula 478/STJ** (a cota condominial prefere ao credito hipotecario) e **ordem de RATEIO do produto**, **nao** responsabilidade pessoal do arrematante. Confundir as duas coisas e erro classico.

⚠️ **A clausula de sub-rogacao no edital NAO e garantia.** A protecao do **908, §1º** depende de o credito estar **documentalmente comprovado e habilitado**. **Se o condominio nao se habilitar, a natureza propter rem puxa a divida para o imovel.** Por isso a conferencia nos autos e obrigatoria.

## ⭐⭐ O grito desta skill
**Ler a clausula de debitos condominiais do edital ANTES do lance decide quem responde pela divida.** Nao e detalhe de leitura: e a variavel que muda o resultado financeiro.

Em edital real: **R$ 53.374,15** de debito condominial + **R$ 5.337,41** de honorarios, sobre avaliacao de **R$ 136.142,37** — **39% da avaliacao**. Um lote com **37% de desagio** e **39% de divida informada** nao e oportunidade: **e prejuizo**.

**Na conta:** edital que informa ⇒ lancar o **valor integral como custo certo**. Edital omisso ⇒ lancar como **risco quantificado** (obter a declaracao da administradora), **nunca como R$ 0**.

## Regras de ouro
- **Duas naturezas, duas respostas.** Resposta unica sobre "debitos do imovel" e alucinacao com cara de certeza.
- **Alienacao fiduciaria: o encargo do fiduciante esta no art. 23, §2º da Lei 9.514** (incluido pela **Lei 14.620/2023, art. 28**) — IPTU e taxas condominiais. ⛔ **Nao cite o art. 24, §2º**: aquele endereco veio da **MP 1.162/2023** e ficou **sem eficacia**. 🚫 **E proibido escrever que a MP "nao vingou" — ela FOI convertida** (Lei 14.620/2023), e a parte contraria refuta em dois cliques. ⚠️ **Por que o erro nasce:** o compilado exibe **os dois dispositivos na tela, sem tachado**, e quem faz grep de "IPTU" acha os dois; o que desqualifica o art. 24, §2º e a **atribuicao apenas a MP**. ⚠️ **Limite honesto, na mesma frase:** o art. 23, §2º rege **fiduciante x fiduciario** e **nao resolve sozinho a divida do ARREMATANTE**.
- **IPTU no extrajudicial:** e do **fiduciante ate a imissao do credor na posse** (**REsp 1.949.182**). 🟡 O numero do Tema ("1.158") veio de busca, nao da ficha — **citar o REsp, nunca o Tema**.
- **O catch-all cobra o que ninguem lembra** (ARM-05): multa ambiental, gas canalizado, taxa de associacao, concessionarias. **Ler a ressalva ao lado da clausula e listar o que ficou de fora dela.**
- ⛔ **Nao afirmar "nao ha debitos" sem certidao lida.** Ausencia de informacao **nao e** ausencia de divida.
- Cross-link soft: a **defesa** do arrematante ja cobrado esta em `debitos-e-creditos-pos-arrematacao` (C5); o **calculo** de atualizacao cruza para `calculosjudiciais-adv-os`; o ITBI como tributo, para `tributario-societario`.

## Entrega obrigatoria final
Quadro por divida: **natureza · valor · fonte documental · quem responde · fundamento com a qualificacao · grau (✅ ancorado / 🟡 a conferir) · o que entra na conta**. Mais a resposta explicita da pergunta "o edital informa?" e, sendo omisso, a **tese** com a ressalva escrita. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
🚫 **Nunca "a materia esta em aberto no STJ"** no condominio. Nunca **Tema 1.134 como condominio**. Nunca **Tema 1.266 como saida**. Nunca **Sumula 478 como responsabilidade pessoal**. Nunca **art. 24, §2º** como fonte do encargo do fiduciante, e nunca dizer que a MP nao vingou. Nunca tratar a clausula de sub-rogacao do edital como garantia sem **habilitacao** verificada. Nunca R$ 0 de condominio sem documento. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
