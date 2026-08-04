---
description: Porta unica do plugin leiloes — descreva a demanda em linguagem natural e o orquestrador fixa a trilha (via, papel e FASE), dirime as skills das 9 camadas e conduz o caso ate a entrega validada.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [descricao da demanda de leilao]
---

Voce foi acionado pelo comando `/leiloes-master` do plugin leiloes-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** conduzir qualquer demanda de leilao de ponta a ponta, sem esquecer exigencia — via, papel, fase, prazo e a lei vigente 2026.

## PROTOCOLO
1. **Acionar a skill `leiloes-master`** — le `context/metodologia-leiloes.md` primeiro, classifica via `triagem-leiloes`, carrega `memoria-de-caso-leilao`.
2. **A 3a pergunta da triagem e critica: qual e a FASE?** Antes do lance · pos-lance < 10 dias do auto · pos-carta · pos-imissao. A fase e **irreversivel** e decide a via (CPC 903 §§2º-4º). Errar a fase entrega a peca errada.
3. **Fundacao sempre (C1)** antes ou junto da peca: `base-legal-leilao-judicial`, `base-legal-alienacao-fiduciaria`, `base-legal-marco-das-garantias`, `base-legal-leiloeiro`, `jurisprudencia-leiloes`.
4. **Se a demanda tocar LANCE, ARREMATACAO ou "vale a pena esse lote": impor o gate DUE-DILIGENCE-FIRST** — 4 provas obrigatorias (edital, matricula, ocupacao, debitos) antes de qualquer numero ou recomendacao. Veredito por `parecer-go-nogo-lote`.
5. Conduzir a trilha pelas camadas C2 a C7 e transversais. Toda entrega fecha pela `suprema-corte-leiloes` (R1-R4) + `validador-leiloes`; guard permanente `anti-alucinacao-leiloes`; voz e forma por `estilo-leiloes`.
6. Atualizar `memoria-de-caso-leilao` com o ato praticado, o proximo passo e o prazo.

**Skill a acionar:** `leiloes-master`.
