---
description: Conduz a sequencia pos-lance do leilao judicial — auto de arrematacao, deposito do preco, comissao e despesas, carta de arrematacao e a trava dos 10 dias do art. 903, §3º.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [auto, valores pagos e o que falta]
---

Voce foi acionado pelo comando `/arrematacao` do plugin leiloes-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** dizer o que falta para a carta sair, quanto ainda desembolsa e quando a posse entra.

## PROTOCOLO
1. **Acionar a skill `arrematacao-auto-e-carta`**. Anexos: `cpc-leilao-879-903.md` (901, 903 §3º, 884), `custo-total-do-arrematante.md`.
2. **Sequencia obrigatoria (CPC 901):** auto lavrado de imediato → deposito do preco (ou garantias) **MAIS** comissao **MAIS** despesas → so entao carta e mandado de imissao. A carta ainda exige prova de **ITBI** e indicacao de onus remanescente.
3. **Trava do art. 903, §3º:** a carta so e expedida **passados os 10 dias** sem alegacao de invalidacao / ineficacia / resolucao.
4. **Comissao e despesas NAO estao dentro do lance** — sao pagamento adicional e condicao da carta. O CPC nao fixa percentual (884, §unico); 5% e piso.
5. Se houver parcelamento, cruzar com `arrematacao-parcelada-895` (minimo 25% a vista; lance a vista **sempre prevalece** — §7º).
6. Fechar pela `suprema-corte-leiloes` + `validador-leiloes`.

**Skill a acionar:** `arrematacao-auto-e-carta`.
