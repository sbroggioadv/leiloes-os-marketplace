---
description: Avalia tese de preco vil no leilao judicial (cascata do CPC 891) e no extrajudicial (AREsp 2.165.101/PR — decisao monocratica, nao repetitivo) — separa os dois "50%" e diz a forca real da peca.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [avaliacao, lance, edital e via]
---

Voce foi acionado pelo comando `/preco-vil` do plugin leiloes-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** dizer se existe tese de preco vil neste caso, com qual regua, qual forca e o que ela consegue.

## PROTOCOLO
1. **Acionar a skill `preco-vil-como-tese`**. Anexos: `cpc-leilao-879-903.md` (891, 885, 886 II, 896), `lei-9514-consolidada.md` (art. 27, §2º), `jurisprudencia-leiloes.md`.
2. **Via primeiro (botoes):** judicial · extrajudicial AF · hipoteca 14.711 · nao sei. **Usar a regua da outra via queima a peca.**
3. **Judicial — cascata do art. 891, §unico:** com preco minimo no edital, vil e o que fica **abaixo dele**; so na ausencia vale o piso supletivo de **50% da avaliacao**. Piso proprio de **80%** para imovel de incapaz (art. 896).
4. **Extrajudicial:** nao ha regra legal de preco vil; a linha e construcao judicial **contra** a literalidade do art. 27, §2º, sustentada pelo **AREsp 2.165.101/PR** (**decisao monocratica do relator** no AgInt; **nao localizamos acordao colegiado na base oficial**; **nao e repetitivo**, **nao vincula**). Escrever *"ha linha no STJ que anula em casos concretos"*, **nunca** "tese firmada" nem "acordao de Turma".
5. **Os dois "50%":** piso supletivo de vileza **x** faculdade exclusiva do credor no 2º leilao — **nao se misturam**.
6. Fechar pela `suprema-corte-leiloes` + `validador-leiloes`.

**Skill a acionar:** `preco-vil-como-tese`.
