---
description: Conduz a imissao na posse do arrematante — mandado, desocupacao, locatarios e a assimetria entre o rito judicial (CPC 901) e o extrajudicial (Lei 9.514, art. 30).
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [carta, ocupantes e fase]
---

Voce foi acionado pelo comando `/imissao` do plugin leiloes-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** obter a posse na via e no prazo certos, sem perder o marco do locatario.

## PROTOCOLO
1. **Acionar a skill `imissao-na-posse-do-arrematante`**. Se houver ocupantes/locacao, encadear `desocupacao-locacao-e-ocupantes` e `situacao-possessoria`.
2. **Assimetria de desocupacao:** Lei 9.514, art. 30 da **liminar expressa + 60 dias** no extrajudicial; o CPC 901, §1º **nao tem prazo nem qualificacao liminar**, e o mandado so sai **depois** de pagos preco, comissao, despesas e ITBI.
3. **Armadilha dos 90 dias do locatario** (Lei 8.245, art. 8º, §2º): o prazo conta do **REGISTRO da venda ou do compromisso** — **nao** da alienacao. Perdido, presume-se manutencao do contrato. Anexo: `lei-8245-locacao.md`.
4. Se o adversario for o executado/fiduciante resistindo, cruzar com `defesa-contra-imissao-e-embargos-de-terceiro` no polo oposto.
5. Fechar pela `suprema-corte-leiloes` + `validador-leiloes`.

**Skill a acionar:** `imissao-na-posse-do-arrematante`.
