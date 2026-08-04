---
description: Defende ou reage a embargos de terceiro e a resistencia a imissao — posse de terceiro, locatario, coproprietario e a via adequada contra a arrematacao ou a consolidacao.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [papel do cliente, posse e fase]
---

Voce foi acionado pelo comando `/embargos-terceiro` do plugin leiloes-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** escolher a via certa para quem nao e parte e tem posse ou direito incompativel com a arrematacao.

## PROTOCOLO
1. **Acionar a skill `defesa-contra-imissao-e-embargos-de-terceiro`**.
2. **Fixar o papel e a fase** com `triagem-leiloes` se ainda nao estiver: arrematante defendendo a imissao **x** terceiro/locatario/coproprietario resistindo.
3. **Cruzar documentos:** matricula, contrato de locacao, comprovantes de posse, edital (intimacoes do art. 889) e, se for o caso, a carta de arrematacao.
4. **Locacao:** marco dos 90 dias do **REGISTRO** (Lei 8.245, art. 8º, §2º). Anexo: `lei-8245-locacao.md`.
5. Se a via for anulatoria judicial ou extrajudicial, encadear `anulatoria-de-arrematacao-judicial` ou `anulatoria-de-leilao-extrajudicial`.
6. Fechar pela `suprema-corte-leiloes` + `validador-leiloes`.

**Skill a acionar:** `defesa-contra-imissao-e-embargos-de-terceiro`.
