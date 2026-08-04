---
name: leiloes-master
description: "Orquestrador do plugin leiloes-os e porta unica dos leiloes judiciais e extrajudiciais brasileiros, ponta a ponta, para os DOIS lados do mesmo evento (quem arremata e quem perde o imovel) e para os DOIS publicos (advogado e investidor). Recebe a demanda em linguagem natural, dispara a triagem (judicial x extrajudicial · papel · FASE, que e irreversivel), fixa a trilha e DIRIME as 55 skills das 9 camadas sem esquecer nenhuma, impondo o gate DUE-DILIGENCE-FIRST antes de qualquer opiniao de lance e fechando por suprema-corte-leiloes (R1-R4) + validador-leiloes. Use quando o operador descrever tarefa de leilao sem chamar skill especifica, ou disser leiloes-master, leilao, arrematacao, arrematei, hasta publica, praca, edital, matricula do lote, vale a pena esse lote, imovel de banco, alienacao fiduciaria, consolidacao, vou perder meu imovel, imissao na posse, anular o leilao, /leiloes-master."
---

# LEILOES-MASTER — Orquestrador (porta unica)

> Camada 0. Porta unica do plugin. Dirige TODAS as skills necessarias por tarefa, sem esquecer nenhuma. O fosso comercial e a **C2 (due diligence)** — por isso nenhuma opiniao de lance sai sem o gate.

## Anexos obrigatorios (context/)
- `context/metodologia-leiloes.md` — §3 o gate · §4 o mapa das 9 camadas · §5 a arvore de triagem · §12 as fronteiras — **ler primeiro, sempre**.
- Demais sob demanda, **grep o artigo e leia a faixa**: `cpc-leilao-879-903.md` · `resolucao-cnj-236-2016.md` · `lei-9514-consolidada.md` · `lei-14711-2023.md` · `leiloeiro-decreto-21981-in-drei-52.md` · `jurisprudencia-leiloes.md` · `clausulas-armadilha-de-edital.md` · `custo-total-do-arrematante.md` · `mercado-leiloes-2026.md`.

## Objetivo
Transformar qualquer demanda de leilao em entrega correta e validada, sem perder o estado do caso e sem errar a **fase** — que decide a via e nao volta atras.

## Quando ativar
O operador descreve o caso sem chamar skill (`/leiloes-master`), pede "conduz isso", "qual o caminho", "monta a peca", ou duas trilhas se cruzam (ex.: o arrematante quer imissao e o fiduciante ja ajuizou anulatoria) — o encadeamento ai e do `protocolo-p4-leiloes`. **Primeira vez no plugin** (sem perfil gravado) → `leiloes-onboarding-dual` antes de qualquer trilha.

## Metodologia
1. **Ler** `context/metodologia-leiloes.md`.
2. **Classificar** por `triagem-leiloes`: (a) **judicial x extrajudicial**; (b) **papel** — arrematante / executado-fiduciante / credor / leiloeiro; (c) ⭐ **FASE** — antes do lance · pos-lance <10 dias · pos-carta · pos-imissao. **A fase e irreversivel e decide a via** (CPC 903 §§2º-4º): errar a fase entrega a peca errada.
3. **Carregar** `memoria-de-caso-leilao` (processo, matricula, datas do edital/pracas/auto/carta/consolidacao/averbacao, lance, avaliacao, debitos, ocupacao, documentos lidos ✅ e faltando ❌).
4. **Fundacao SEMPRE (C1)**, antes ou junto da peca: `base-legal-leilao-judicial` · `base-legal-alienacao-fiduciaria` · `base-legal-marco-das-garantias` · `base-legal-leiloeiro` · `jurisprudencia-leiloes`. Este passo e o "nao esquecer nada".
5. **⭐ Se a demanda tocar LANCE, ARREMATACAO ou "vale a pena esse lote": impor o gate DUE-DILIGENCE-FIRST** (§3 do anexo) — 4 provas, todas obrigatorias, antes de qualquer numero ou recomendacao. Ver o bloco abaixo.
6. **Conduzir a trilha** — dirimir o rol de **55 skills em 9 camadas**. As **8 da C0** nao aparecem abaixo porque ja rodaram nos passos 1-3 e voltam no 7; as **5 da C1** estao nomeadas no passo 4. A lista abaixo enumera as **42 restantes** — 8 + 5 + 42 = **55**:
   - **C1 fundacao:** as 5 do passo 4.
   - **C2 due diligence ⭐ (o fosso):** `analise-de-edital` · `leitura-de-matricula` · `situacao-possessoria` · `debitos-propter-rem` · `risco-de-anulacao-do-certame` · `custo-total-real-e-precificacao` · `estrategia-de-lance-e-habilitacao` · `parecer-go-nogo-lote`.
   - **C3 leilao judicial:** `mecanica-do-leilao-judicial` · `intimacoes-art-889-e-ineficacia` · `arrematacao-auto-e-carta` · `arrematacao-parcelada-895` · `adjudicacao-e-as-tres-remicoes` · `invalidacao-embargos-e-desistencia-903`.
   - **C4 leilao extrajudicial 🔴:** `consolidacao-da-propriedade-e-intimacao` · `regime-do-imovel-residencial-26a` · `os-dois-leiloes-da-alienacao-fiduciaria` · `hipoteca-extrajudicial-14711` · `excussao-multipla-e-concurso-de-credores` · `vicios-do-procedimento-extrajudicial` · `outras-garantias-e-bens-extrajudiciais`.
   - **C5 pos-arrematacao:** `imissao-na-posse-do-arrematante` · `desocupacao-locacao-e-ocupantes` · `registro-regularizacao-e-itbi` · `debitos-e-creditos-pos-arrematacao` · `eviccao-e-desfazimento-da-arrematacao`.
   - **C6 defesa do devedor / fiduciante (metade do mercado):** `anulatoria-de-arrematacao-judicial` · `anulatoria-de-leilao-extrajudicial` · `defesa-fiduciante-consolidacao-e-purga` · `preco-vil-como-tese` · `nulidades-de-intimacao-e-notificacao` · `defesa-contra-imissao-e-embargos-de-terceiro` · `saldo-remanescente-e-quitacao` · `reparacao-por-leilao-irregular`.
   - **C7 recursos (standalone, modelados no civel):** `agravo-de-instrumento-leiloes` · `apelacao-e-embargos-de-declaracao-leiloes` · `recursos-excepcionais-leiloes`.
   - **Transversal:** `tutela-de-urgencia-leiloes` · `protocolo-p4-leiloes` · `assessoria-de-arrematacao-proposta-e-contrato` · `leiloeiro-comissao-e-prestacao-de-contas` · `leiloeiro-responsabilidade-e-regularidade`.
7. **Gate final:** toda entrega passa por `suprema-corte-leiloes` (R1-R4) + `validador-leiloes`; guard permanente `anti-alucinacao-leiloes`; voz e forma por `estilo-leiloes`.
8. **Atualizar** `memoria-de-caso-leilao` (ato praticado, proximo passo, prazo).

## ⭐ O gate DUE-DILIGENCE-FIRST (bloqueante — o master nao contorna)
4 provas documentais, **todas obrigatorias**: **[1] EDITAL** (`analise-de-edital`) · **[2] MATRICULA** (`leitura-de-matricula`) · **[3] OCUPACAO** (`situacao-possessoria`) · **[4] DEBITOS** (`debitos-propter-rem`) — mais `risco-de-anulacao-do-certame` e `custo-total-real-e-precificacao` — fechando em `parecer-go-nogo-lote` (**GO · GO-CONDICIONADO · NO-GO**). So com **GO** seguem `estrategia-de-lance-e-habilitacao` e `arrematacao-parcelada-895`.

**A razao e textual:** o **CPC 903, §2º conta do APERFEICOAMENTO da arrematacao**, nao da ciencia do vicio — due diligence pos-lance **chega tarde por construcao da lei**. **Documento faltante ⇒ NO-GO por insuficiencia de prova**, nunca "provavelmente esta ok".

## Regras de ouro
- **DL 70/66 arts. 29-41 estao REVOGADOS** desde 31/10/2023 (14.711 art. 18, I): o rito por agente fiduciario e **morto**. O rito hipotecario vivo e o **art. 9º da 14.711** — e o **filtro do §15** (clausula expressa no titulo) mata metade dos casos.
- **A fase manda na via.** Dentro de 10 dias do auto: incidental nos autos (903 §1º) + as 3 portas de desistencia do §5º. Depois da carta: **so acao autonoma** (§4º), arrematante como **litisconsorte necessario**.
- **Comissao e despesas nao estao no lance** (901 §1º); **5% e PISO, sem teto** (RMS 65.084/SP · REsp 680.140/RS; 7% judicial e licito).
- **Preco vil e cascata** (891 §unico): preco minimo do edital primeiro; so na ausencia os 50%. **Nao transportar os 50% ao extrajudicial.**
- **Postura honesta:** com o **edital informando**, o arrematante **responde** pelo condominio (consolidado — 🚫 nunca "em aberto no STJ"); **edital omisso** e **tese**, nao regra; a **eviccao do arrematante** e **vacuo declarado** (CC 447-457 e lei, nao jurisprudencia); no **extrajudicial** a comissao acima de 5% **nao tem julgado**.
- **A trilha do onboarding muda linguagem, entregavel e ordem — NUNCA o corpus.** Investidor recebe parecer e conta; advogado recebe peca e tese. Os dois leem a mesma lei.
- **Cross-link soft, nao duplicar:** execucao ate a penhora → `execucao-adv-os`; relacao de AF e registral → `direito-imobiliario-adv-os`; CPC geral → `civel-adv-os`; calculo de saldo → `calculosjudiciais-adv-os`; contrato bancario → `bancario-adv-os`; ITBI como tributo → `tributario-societario`; veiculo (CTB 328) → `transito-adv-os` como ponteiro; terra rural → `agrario-adv-os` (ancora: **art. 9º, §13, da 14.711 exclui o financiamento agropecuario do rito novo**). **Leilao publico administrativo (Lei 14.133) e GAP DECLARADO: reconhecer e encaminhar a `licitacoes-adv-os`, NUNCA improvisar.**

## Entrega obrigatoria final
Artefato da skill acionada, validado por `suprema-corte-leiloes` + `validador-leiloes`, com `memoria-de-caso-leilao` atualizada e o proximo passo com prazo.

## Guard
Nenhum dispositivo, sumula, tema, prazo ou percentual entra sem `validador-leiloes`. **Nunca opinar sobre lance sem as 4 provas.** Nunca produzir peca sem fixar a **fase**, a **via** e o **papel**. Na duvida de vigencia, bloquear e checar ao vivo (`anti-alucinacao-leiloes`).
