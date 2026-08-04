---
description: Triagem by-conversation do caso de leilao — identifica a trilha por tres perguntas (via, papel e FASE), e devolve a rota com a via, a competencia e o prazo critico antes de qualquer peca.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [descricao do caso ou dos documentos disponiveis]
---

Voce foi acionado pelo comando `/triagem-leiloes` do plugin leiloes-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** fixar a trilha correta antes de gastar peca na via errada.

## PROTOCOLO
1. **Acionar a skill `triagem-leiloes`**.
2. **Ordem das perguntas — tres e a terceira e a que mais derruba peca:**
   - (a) **JUDICIAL** (CPC 879-903 + Res. CNJ 236) **x EXTRAJUDICIAL** (AF Lei 9.514 **x** hipoteca Lei 14.711 art. 9º — checar o **filtro do §15**). Leilao publico administrativo (Lei 14.133) = **GAP DECLARADO** → encaminhar, nunca improvisar.
   - (b) **PAPEL** — arrematante / executado-fiduciante / credor / leiloeiro.
   - (c) ⭐ **FASE** — antes do lance · pos-lance < 10 dias do auto · pos-carta · pos-imissao. A fase e **irreversivel** (CPC 903 §§2º-4º).
3. Fixar, para a trilha escolhida: **via**, **papel**, **fase**, **prazo em curso** (especialmente a janela de 10 dias do art. 903 contada do **aperfeicoamento**) e skills alvo.
4. Se imovel ocupado por locatario, lembrar o marco dos **90 dias do REGISTRO** (Lei 8.245, art. 8º, §2º) — nao da alienacao.
5. Carregar `memoria-de-caso-leilao` e devolver a rota nomeando as skills seguintes.

**Skill a acionar:** `triagem-leiloes`.
