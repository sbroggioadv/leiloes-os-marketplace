---
description: Mapeia debitos e creditos pos-arrematacao — condominio propter rem, IPTU, saldo remanescente, taxas de ocupacao e o que o arrematante realmente assume.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [edital, debitos levantados e fase]
---

Voce foi acionado pelo comando `/debitos-pos` do plugin leiloes-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** dizer o que o arrematante assume e o que ainda e do executado/fiduciante — com a jurisprudencia consolidada, nao o folclore.

## PROTOCOLO
1. **Acionar a skill `debitos-e-creditos-pos-arrematacao`**, cruzando com `debitos-propter-rem` e, se for o caso, `saldo-remanescente-e-quitacao`.
2. **Condominio com edital informando:** arrematante **responde** (*propter rem* + sucessao processual) — REsp 2.042.756/SP consolidado. **PROIBIDO** "materia em aberto no STJ". Edital omisso = **tese de defesa**, nao regra.
3. **Tema 1.134 e exclusivamente TRIBUTARIO** — nao citar como ancora de condominio. **Tema 1.266 e materia diversa.**
4. **IPTU do fiduciante:** endereco vigente e o **art. 23, §2º da Lei 9.514** (red. Lei 14.620/2023) — **nao** o art. 24, §2º residual da MP. Limite: rege fiduciante x fiduciario e **nao resolve sozinho** a divida do arrematante.
5. **Leilao negativo:** fora do art. 26-A, o §5º-A mantem o devedor obrigado pelo saldo remanescente.
6. Fechar pela `suprema-corte-leiloes` + `validador-leiloes`.

**Skill a acionar:** `debitos-e-creditos-pos-arrematacao`.
