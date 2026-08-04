---
description: Emite parecer de leiloes com diagnostico honesto — vale entrar, qual a chance real, qual o custo e qual o caminho — declarando monocraticas, rachas e gaps em vez de vender certeza que nao existe.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [pergunta do cliente e documentos disponiveis]
---

Voce foi acionado pelo comando `/parecer-leiloes` do plugin leiloes-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** dar ao cliente a verdade acionavel — inclusive quando a verdade e "nao entre".

## PROTOCOLO
1. Se a pergunta for **"vale a pena esse lote?"** ou equivalente de lance → acionar o fluxo do gate e a skill **`parecer-go-nogo-lote`** (vitrine). Sem as 4 provas, o parecer e **NO-GO por insuficiencia**.
2. Se a pergunta for **defesa / anulatoria / consolidacao / pos-arrematacao**, classificar por `triagem-leiloes` e conduzir pela skill da trilha, com fundacao C1.
3. **Postura honesta — declare forca real do precedente e gaps, nunca venda tese pendente como decidida:**
   - Preco vil extrajudicial = **AREsp 2.165.101/PR** (decisao monocratica do relator no AgInt; **nao localizamos acordao colegiado na base oficial**; **nao e repetitivo**, **nao vincula**) — *"ha linha no STJ que anula em casos concretos"*, nunca "tese firmada" nem "acordao de Turma";
   - Condominio com edital informando = **consolidado** — proibido "em aberto no STJ";
   - Eviccao do arrematante = moldura **CC 447-457** + **REsp 1.293.147/GO** (STJ: eviccao **descaracterizada**, indenizacao **afastada** por ma-fe — **nao** e precedente generico a favor do arrematante); verificar boa-fe e cadeia no caso concreto;
   - Comissao > 5% no extrajudicial = **sem julgado localizado**;
   - REsp 2.171.564/SP e Tema 1.266 = **pendentes**.
4. **Gaps intransponiveis — nao preencher por invencao:** leilao publico administrativo (Lei 14.133) · aliquotas municipais de ITBI · emolumentos fora de SP · regulamentacao registral estadual do art. 9º da 14.711.
5. Fechar pela `suprema-corte-leiloes` + `validador-leiloes`, com o proximo passo e o prazo.

**Skill a acionar:** `parecer-go-nogo-lote` (se lote/lance) ou a skill da trilha apontada pela triagem.
