---
description: Emite o parecer GO / GO-CONDICIONADO / NO-GO do lote — consolida as 4 provas do gate (edital, matricula, ocupacao, debitos), o risco de anulacao e a conta completa com teto de lance.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [edital, matricula, debitos e o que se sabe da ocupacao]
---

Voce foi acionado pelo comando `/go-no-go` do plugin leiloes-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** dar ao operador a verdade acionavel — inclusive quando a verdade e "NAO entre" — com o **porque** de cada componente e o **teto de lance**.

## PROTOCOLO
1. **Acionar a skill `parecer-go-nogo-lote`**. Este parecer **nao sai** sem as 4 provas documentais.
2. **Rodar o gate na ordem:**
   - [1] Edital → `analise-de-edital` (anexo: `clausulas-armadilha-de-edital.md`)
   - [2] Matricula → `leitura-de-matricula`
   - [3] Ocupacao → `situacao-possessoria`
   - [4] Debitos → `debitos-propter-rem`
   - + `risco-de-anulacao-do-certame` + `custo-total-real-e-precificacao` (anexo: `custo-total-do-arrematante.md`)
3. **Documento faltando = NO-GO por insuficiencia de prova.** Nunca "provavelmente ok", nunca "aparentemente livre", nunca "nao identifiquei onus" quando o que houve foi nao ter lido a matricula.
4. **Vereditos:** GO (teto de lance com comissao embutida) · GO-CONDICIONADO (teto rebaixado + condicao nomeada) · NO-GO (motivo especifico).
5. Entrega em dois registros **sem trocar o corpus**: conta e teto para o investidor; parecer e tese para o advogado.
6. Fechar pela `suprema-corte-leiloes` + `validador-leiloes`.

**Skill a acionar:** `parecer-go-nogo-lote`.
