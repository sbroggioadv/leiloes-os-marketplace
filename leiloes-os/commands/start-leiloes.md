---
description: Inicia o wizard de configuracao dual do plugin leiloes — fixa a trilha (advogado x investidor), o perfil do escritorio ou da operacao, e grava o estado em memoria-de-caso-leilao antes de qualquer trilha.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [--update para reconfigurar]
---

Voce foi acionado pelo comando `/start-leiloes` do plugin leiloes-os (leiloes judiciais e extrajudiciais brasileiros ponta a ponta).

Argumento recebido: `$ARGUMENTS`

**Objetivo:** configurar o plugin ao perfil do operador (advogado ou investidor) antes de qualquer trilha.

## PROTOCOLO
1. **Acionar a skill `leiloes-onboarding-dual`** (wizard com botoes via AskUserQuestion nas escolhas de lista fechada).
2. Fixa a **trilha**: sou advogado (peca + tese + fundamento) **x** sou investidor (parecer + conta + teto de lance). A trilha muda linguagem, entregavel e ordem — **nunca o corpus**.
3. Grava o perfil (escritorio ou operacao) em `memoria-de-caso-leilao` / pasta local de runtime. Se ja existir, oferecer continuar / atualizar / recriar.
4. Declarar na entrada o que o plugin **nao** faz: leilao publico administrativo da Lei 14.133 (gap → `licitacoes-adv-os`) e que **nenhuma opiniao de lance** sai sem as 4 provas do gate DUE-DILIGENCE-FIRST.
5. Fechar apontando a porta unica (`/leiloes-master`).

**Skill a acionar:** `leiloes-onboarding-dual`.
