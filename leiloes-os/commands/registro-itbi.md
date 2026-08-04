---
description: Orienta o registro da arrematacao e o ITBI — sequencia apos a carta, bases de calculo, emolumentos pela maior base e o que nunca inventar de aliquota municipal.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [carta, municipio e valores]
---

Voce foi acionado pelo comando `/registro-itbi` do plugin leiloes-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** fechar o titulo registral e o tributo sem inventar aliquota nem subestimar emolumento.

## PROTOCOLO
1. **Acionar a skill `registro-regularizacao-e-itbi`**. Anexos: `custo-total-do-arrematante.md`, `cpc-leilao-879-903.md` (901).
2. **Sequencia:** carta de arrematacao exige prova de pagamento do ITBI; emolumento de registro pode ser enquadrado por valor **maior** que o lance (maior entre preco declarado, valor do IPTU e base do ITBI).
3. **PROIBIDO** dar numero de aliquota municipal de ITBI, emolumento fora de SP ou custas judiciais — dar a **formula** e a **fonte a consultar**.
4. Se houver ganho de capital na revenda ou discussao tributaria pesada, cross-link soft para `tributario-societario-adv-os` / `cfo-combativo-os` — nao duplicar.
5. Fechar pela `suprema-corte-leiloes` + `validador-leiloes`.

**Skill a acionar:** `registro-regularizacao-e-itbi`.
