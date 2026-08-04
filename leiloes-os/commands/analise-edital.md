---
description: Audita o edital de leilao judicial ou extrajudicial — cruza clausulas-armadilha, confere o art. 886 inciso a inciso e marca o que o edital omite sobre onus, debitos e ocupacao.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [edital ou trechos relevantes]
---

Voce foi acionado pelo comando `/analise-edital` do plugin leiloes-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** devolver o edital lido como prova documental — o que ele informa, o que omite e quais clausulas sao armadilha.

## PROTOCOLO
1. **Acionar a skill `analise-de-edital`**. Anexos: `clausulas-armadilha-de-edital.md`, `cpc-leilao-879-903.md` (art. 886), `resolucao-cnj-236-2016.md`.
2. **Auditoria do art. 886** — item a item do edital judicial; no extrajudicial, cruzar com a Lei 9.514 e a Res. CNJ 236 no que couber.
3. **Clausulas-armadilha** (comissao por fora, caucao, prazo de 24 h, "sem garantia" que so repete o art. 18 da Res. CNJ 236, etc.): marcar o risco e o custo no teto de lance.
4. **A clausula "sem garantia" NAO e abusiva em si** — reproduz a norma (Res. CNJ 236, art. 18). Atacar o edital que **descumpre o art. 886**, nao o edital que avisa o estado do bem.
5. Entregar o relatorio como prova [1] do gate; se o pedido for de lance, seguir para as demais provas e `parecer-go-nogo-lote`.
6. Fechar pela `suprema-corte-leiloes` + `validador-leiloes`.

**Skill a acionar:** `analise-de-edital`.
