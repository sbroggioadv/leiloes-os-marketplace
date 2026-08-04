---
description: Le a matricula do imovel leiloado — onus reais, gravames, averbacoes de consolidacao, penhoras e o que o edital deveria ter mencionado sob o art. 886, VI.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [matricula, numero e cartorio]
---

Voce foi acionado pelo comando `/matricula` do plugin leiloes-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** transformar a matricula em prova documental [2] do gate — onus, gravames e o que o edital omitiu.

## PROTOCOLO
1. **Acionar a skill `leitura-de-matricula`**.
2. **Mapear a cadeia:** aquisicao, hipotecas, alienacao fiduciaria, penhoras, indisponibilidades, averbacoes de consolidacao e de leilao.
3. **Cruzar com o edital** — gravame na matricula nao mencionado no edital e a saida forte do **CPC art. 903, §5º, I** (desistencia com devolucao do deposito), que **caduca em 10 dias** do aperfeicoamento.
4. **Nunca afirmar "livre e desembaracado" sem a matricula lida.** Documento faltando = prova [2] ausente = NO-GO no gate.
5. Entregar o relatorio como prova [2]; se o pedido for de lance, seguir para ocupacao, debitos e `parecer-go-nogo-lote`.
6. Fechar pela `suprema-corte-leiloes` + `validador-leiloes`.

**Skill a acionar:** `leitura-de-matricula`.
