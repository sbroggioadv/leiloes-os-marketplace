---
description: Opera as tres hipoteses do art. 903 do CPC (invalidacao, ineficacia e resolucao) e as tres portas de desistencia do §5º — cada uma com seu marco (so o inciso I tem janela de 10 dias).
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [data do auto, vicio alegado e documentos]
---

Voce foi acionado pelo comando `/invalidacao-903` do plugin leiloes-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** escolher a via certa dentro da janela certa — e nao confundir invalidacao nos autos com acao autonoma.

## PROTOCOLO
1. **Acionar a skill `invalidacao-embargos-e-desistencia-903`**. Anexo: `cpc-leilao-879-903.md` (art. 903 integral + 804).
2. **Travar a fase ANTES de qualquer peca:**
   - **Invalidacao / ineficacia / resolucao nos autos** (§§1º-2º): prazo de **10 dias** contado do **aperfeicoamento** do auto (assinatura), **nao** da ciencia do vicio.
   - **Desistencia do arrematante (§5º) — tres marcos distintos (NAO unificar em "10 dias"):**
     - **Inciso I** — onus real ou gravame nao mencionado no edital (violacao do art. 886, VI): alegar em **ate 10 dias** do aperfeicoamento do auto → devolucao do deposito.
     - **Inciso II** — se, **antes** da expedicao da carta ou da ordem de entrega, o **executado** alegar hipotese do §1º (sujeito: **executado**; marco: expedicao, nao "10 dias").
     - **Inciso III** — uma vez **citado** na acao autonoma do §4º, o arrematante desiste **desde que apresente a desistencia no prazo de resposta** a essa acao (citacao **+** prazo de resposta; nao "10 dias" do auto).
   - **Pos-carta** → so **acao autonoma** (§4º), arrematante como **litisconsorte necessario**.
3. **Dies a quo (invalidacao nos autos e §5º, I):** o prazo de 10 dias conta do **aperfeicoamento** (assinatura do auto), **nao** da ciencia do vicio. Os incisos II e III do §5º **nao** usam essa janela.
4. **Ineficacia ≠ nulidade** — falta de intimacao do **credor pignoraticio, hipotecario ou anticretico** (804 + 903, §1º, II) deixa o arrematante com o imovel **e** com o gravame; a lei **nao** diz "qualquer titular de direito real".
5. **Saida mais forte e caduca no relogio de 10 dias:** §5º, **I** apenas — onus real ou gravame **nao mencionado no edital** (violacao do art. 886, VI) → desistencia com devolucao do deposito.
6. **Freio do §6º:** suscitar vicio **infundado** e ato atentatorio, com multa de ate **20% do valor atualizado** do bem. Auditoria tem de ser documental. (Nao confundir com a multa de **20% da avaliacao** em beneficio do incapaz — **CPC art. 896, §2º**.)
7. Fechar pela `suprema-corte-leiloes` + `validador-leiloes`.

**Skill a acionar:** `invalidacao-embargos-e-desistencia-903`.
