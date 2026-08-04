---
name: leiloes-onboarding-dual
description: "Onboarding DUAL do plugin leiloes-os, rodado uma unica vez na primeira sessao. Em botoes clicaveis (AskUserQuestion), fixa a TRILHA — sou advogado 🎓 x sou investidor 💰 — e o perfil (escritorio ou operacao), gravando tudo em memoria-de-caso-leilao. A trilha muda LINGUAGEM, ENTREGAVEL e ORDEM; NUNCA muda o corpus: os dois leem a mesma lei, com as mesmas ressalvas honestas. Tambem avisa, ja na entrada, o que o plugin nao faz (leilao publico administrativo da Lei 14.133 e gap declarado) e que nenhuma opiniao de lance sai sem as 4 provas documentais do gate DUE-DILIGENCE-FIRST. Use na primeira vez que alguem abrir o plugin, ou quando disserem start leiloes, configurar, sou advogado, sou investidor, quero comecar, /start-leiloes."
---

> **🖱️ Escolhas = botoes:** nas perguntas de **lista fechada** (trilha, perfil, foco) use a ferramenta **AskUserQuestion** para mostrar **botoes clicaveis** (max. 4 por pergunta; havendo mais, divida em 2).

# LEILOES-ONBOARDING-DUAL — `/start-leiloes`

> Camada 0. Porta de entrada, roda **uma vez**. Fixa quem e o operador e como ele quer receber — e deixa claro, ja aqui, o que o plugin **nao** promete. Nao produz peca.

## Anexos obrigatorios (context/)
- `context/metodologia-leiloes.md` — §4 o mapa das 9 camadas · §12 as fronteiras · §14 o tom — **grep + ler a faixa**.
- `context/mercado-leiloes-2026.md` — vocabulario do nicho e as travas de copy (o desagio medio provado e **37,3%**) — **grep + ler a faixa**.

## Objetivo e quando ativar
Gravar **trilha + perfil** e devolver o operador ao `leiloes-master` sabendo o que esperar. Roda na **primeira** sessao (sem perfil gravado em `memoria-de-caso-leilao`) ou quando o operador pedir para reconfigurar.

## Pergunta 1 (botoes) — A TRILHA
- **🎓 Sou advogado** — atende cliente (arrematante, executado, fiduciante, credor ou leiloeiro). Entregavel padrao: **peca + tese + fundamento**.
- **💰 Sou investidor** — arremata para si ou para terceiros. Entregavel padrao: **parecer + a conta + o teto de lance**.

> ⚠️ **A trilha muda LINGUAGEM, ENTREGAVEL e ORDEM. NUNCA muda o CORPUS.** Os dois leem a mesma lei, recebem as mesmas ressalvas honestas e passam pelos mesmos gates. O investidor **nao** recebe uma versao simplificada da lei — recebe a mesma lei em linguagem de decisao. O advogado **nao** deixa de ver a conta — ele a ve como fundamento de peca.

**O que a trilha muda, concretamente:**

| | 🎓 Advogado | 💰 Investidor |
|---|---|---|
| Vocabulario | tecnico-processual (dies a quo, litisconsorcio, ineficacia) | operacional (teto de lance, carrego, desagio liquido) — termo tecnico aparece **traduzido na primeira vez** |
| Entregavel | peca, tese, quesito, minuta | parecer GO/NO-GO, conta fechada, checklist |
| Ordem | fundamento → prazo → via → peca | veredito → numero → risco → o que fazer agora |
| Fecho | `suprema-corte-leiloes` + `validador-leiloes` | **os mesmos dois** |

## Pergunta 2 (botoes) — O PERFIL
- **🎓 Escritorio:** area de atuacao dominante · atende mais o **arrematante** ou o **devedor/fiduciante** · comarca/UF de atuacao.
- **💰 Operacao:** tipo de imovel-alvo (residencial · comercial · terreno) · faixa de ticket · **judicial, extrajudicial ou os dois**.

> 🔒 **Despersonalizacao obrigatoria:** grave **funcao e preferencia**, nunca **nome de pessoa, numero de OAB, e-mail ou dado de cliente**. O escritorio ou a operacao sao descritos por **papel**, nao por identidade.

## Pergunta 3 (botoes) — O FOCO DE ENTRADA (opcional, acelera a 1a tarefa)
- **Avaliar um lote agora** → `triagem-leiloes` → gate → `parecer-go-nogo-lote`.
- **Ja arrematei e apareceu problema** → `triagem-leiloes` (a **FASE** decide tudo).
- **Vou perder meu imovel / meu cliente vai** → C6, defesa do devedor/fiduciante.
- **So conhecer o plugin** → mapa das 9 camadas.

## O que dizer na entrada — sem promessa
1. ⭐ **Nenhuma opiniao de lance sai sem as 4 provas documentais** — edital, matricula, ocupacao e debitos. **Documento faltando ⇒ NO-GO por insuficiencia de prova.** O motivo e legal, nao burocratico: o prazo do **CPC 903, §2º corre do aperfeicoamento da arrematacao**, entao due diligence pos-lance chega tarde.
2. ⛔ **Leilao publico administrativo (Lei 14.133) e GAP DECLARADO** — o plugin **reconhece e encaminha**, nunca improvisa.
3. 📊 O que o plugin **nao** diz: "leilao e seguro" · "70% de desconto garantido" (o desagio medio provado e **37,3%**) · "essa arrematacao nunca cai". Onde a jurisprudencia esta **condicionada, monocratica ou ausente**, ele **diz que esta**.
4. 🔴 A lei vendida e a **vigente em agosto/2026** — inclusive o que e recente: **DL 70/66 arts. 29-41 revogados** e o rito hipotecario novo do **art. 9º da Lei 14.711/2023**.

## Entrega obrigatoria final
Confirmacao em 3 a 5 linhas: **trilha + perfil + foco**, o que muda no formato das entregas, o aviso do gate das 4 provas, e o handoff para o `leiloes-master`. Gravar em `memoria-de-caso-leilao`.

## Guard
Nao produzir peca nem parecer aqui — so configurar e rotear. **Nunca gravar nome de cliente, OAB, e-mail ou dado pessoal.** Nao prometer resultado, prazo de retorno ou percentual de desconto. Se o operador escolher a trilha do investidor, **nao simplificar a lei**: simplificar a **linguagem** e manter **todas** as ressalvas 🟡 — e exatamente ai que os 8 concorrentes do nicho erram, dando resposta binaria.
