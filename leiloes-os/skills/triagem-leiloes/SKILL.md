---
name: triagem-leiloes
description: "Classifica a demanda de leilao e roteia para as skills certas, em botoes clicaveis. Tres perguntas, e a terceira e a que mais derruba peca: (a) JUDICIAL x EXTRAJUDICIAL — e, no extrajudicial, alienacao fiduciaria da Lei 9.514 ou hipoteca do art. 9º da Lei 14.711, que exige checar o filtro do §15; (b) PAPEL — arrematante, executado/fiduciante, credor ou leiloeiro; (c) ⭐ FASE — antes do lance, pos-lance com menos de 10 dias do auto, pos-carta ou pos-imissao. A FASE e IRREVERSIVEL e decide a via (CPC 903 §§2º-4º): pedir invalidacao nos autos depois da carta, ou acao autonoma dentro dos 10 dias, e erro que se paga com extincao. Use quando o operador descrever um caso de leilao e nao souber o caminho, ou disser triagem, por onde comeco, que peca eu uso, arrematei e apareceu problema, vao leiloar meu imovel, recebi intimacao do leilao, /triagem-leiloes."
---

> **🖱️ Escolhas = botoes:** nas perguntas de **lista fechada** (via, papel, fase) use a ferramenta **AskUserQuestion** para mostrar **botoes clicaveis** (max. 4 por pergunta; havendo mais, divida em 2).

# TRIAGEM-LEILOES

> Camada 0. Porta de classificacao, chamada pelo `leiloes-master` no inicio de todo caso. Define **via → papel → FASE**, e a fase e a que nao volta atras.

## Anexos obrigatorios (context/)
- `context/metodologia-leiloes.md` — §5 a arvore de triagem · §4 o mapa das camadas · §12 as fronteiras — **grep o artigo e leia a faixa**.
- `context/cpc-leilao-879-903.md` — para conferir, ainda na triagem, se a **janela de 10 dias do art. 903 §2º** ainda esta aberta — **grep + ler a faixa**.
- `context/lei-8245-locacao.md` — imovel ocupado por locatario: o art. 8º §2º verbatim, os **90 dias do REGISTRO** — **grep o artigo e leia a faixa**.

## Objetivo e quando ativar
Em poucas perguntas devolver **via + papel + fase + skill(s) alvo + prazo em curso**, e passar o handoff ao `leiloes-master`. Roda quando o operador descreve o caso sem saber o caminho, pergunta "que peca eu uso" ou "vale a pena", ou quando o master abre caso novo.

## Pergunta 1 (botoes) — A VIA
- **Judicial** (CPC 879-903 + Res. CNJ 236) → C3 · C2 · C6.
- **Extrajudicial — alienacao fiduciaria** (Lei 9.514) → C4 · C2 · C6.
- **Extrajudicial — hipoteca** (Lei 14.711, art. 9º) 🔴 → C4, e **checar o FILTRO DO §15** antes de tudo: o rito so vale se o **titulo constitutivo da hipoteca** trouxer, como **requisito de validade**, previsao expressa com mencao aos §§1º a 10. Hipoteca anterior a 31/10/2023 tipicamente **nao tem** — e essa e a **defesa de primeira linha** do devedor e **item obrigatorio** da due diligence do arrematante.
- **Leilao publico administrativo** (Lei 14.133) → ⛔ **GAP DECLARADO**: reconhecer e encaminhar a `licitacoes-adv-os`. **Nunca improvisar.**

> 🔴 Se alguem trouxer "execucao extrajudicial por agente fiduciario do DL 70/66": os **arts. 29-41 estao REVOGADOS** desde 31/10/2023 (14.711 art. 18, I). O rito vivo e o **art. 9º**. Corrigir **na triagem**, antes de qualquer peca.

## Pergunta 2 (botoes) — O PAPEL
- **Arrematante** (ou pretendente) → C2 (due diligence) · C5 (pos-arrematacao).
- **Executado / fiduciante** (vai perder ou perdeu o imovel) → C6.
- **Credor / exequente** → C3 · C4.
- **Leiloeiro** → transversal: `leiloeiro-comissao-e-prestacao-de-contas` · `leiloeiro-responsabilidade-e-regularidade`.

## ⭐ Pergunta 3 (botoes) — A FASE (irreversivel; decide a via)
- **ANTES do lance** → **GATE de due diligence** (as 4 provas). Ainda da para nao errar. → `analise-de-edital` · `leitura-de-matricula` · `situacao-possessoria` · `debitos-propter-rem` · `risco-de-anulacao-do-certame` · `custo-total-real-e-precificacao` → `parecer-go-nogo-lote`.
- **POS-lance, menos de 10 dias do auto** → **janela aberta** do CPC 903 §1º (invalidacao · ineficacia · resolucao) + as **3 portas de desistencia do §5º** → `invalidacao-embargos-e-desistencia-903`. ⏰ **Conferir a data da assinatura do auto AGORA** — o prazo corre do **aperfeicoamento**, nao da ciencia do vicio.
- **POS-carta** → **so acao autonoma** (903 §4º), com o arrematante como **litisconsorte necessario** → `anulatoria-de-arrematacao-judicial` (judicial) · `anulatoria-de-leilao-extrajudicial` (extrajudicial).
- **POS-imissao** → discussao indenizatoria, debitos e eviccao → `debitos-e-creditos-pos-arrematacao` · `reparacao-por-leilao-irregular` · `eviccao-e-desfazimento-da-arrematacao`.

> 🚨 **Errar a fase entrega a peca errada.** Pedir invalidacao nos autos depois da carta, ou acao autonoma dentro dos 10 dias, e erro que se paga com **extincao**. A fase e a primeira coisa a travar, e ela vale mais que a pressa do operador.

## Roteamento por sintoma (quando o operador nao usa termo tecnico)
1. **"vale a pena esse lote?" · "quanto posso dar?"** → gate completo → `parecer-go-nogo-lote` (o teto de lance sai de `custo-total-real-e-precificacao`, com a comissao **por fora**).
2. **"arrematei e o imovel esta ocupado"** → `situacao-possessoria` · `imissao-na-posse-do-arrematante` · `desocupacao-locacao-e-ocupantes` (os **90 dias** do locatario correm **do REGISTRO da venda ou do compromisso**, nunca da alienacao — 8.245 art. 8º §2º em `context/lei-8245-locacao.md`: **grep o artigo e leia a faixa**).
3. **"estao me cobrando IPTU/condominio do antigo dono"** → `debitos-e-creditos-pos-arrematacao` (tributo **a favor** do arrematante pelo Tema 1.134 **com a modulacao**; condominio **contra** ele quando o **edital informa**).
4. **"vao leiloar meu imovel" · "recebi intimacao"** → `consolidacao-da-propriedade-e-intimacao` · `regime-do-imovel-residencial-26a` · `defesa-fiduciante-consolidacao-e-purga` (⏰ purga **ate a averbacao**).
5. **"o leilao saiu por um preco absurdo"** → `preco-vil-como-tese` — **duas reguas que nao se misturam**: judicial e a **cascata do CPC 891 §unico**; extrajudicial e construcao judicial contra a literalidade do art. 27 §2º (🟡 **monocratica** — "o STJ vem anulando").
6. **"quero suspender o leilao antes"** → `tutela-de-urgencia-leiloes` (⚠️ no extrajudicial, o art. 30 §unico diz que **quase nada obsta** a reintegracao — so a notificacao).
7. **"quero cobrar por esse servico"** → `assessoria-de-arrematacao-proposta-e-contrato`.

## Gestao obrigatoria (sempre, antes da peca)
Toda entrega passa pela fundacao **C1** (`base-legal-leilao-judicial` · `base-legal-alienacao-fiduciaria` · `base-legal-marco-das-garantias` · `base-legal-leiloeiro` · `jurisprudencia-leiloes`) e fecha por `suprema-corte-leiloes` + `validador-leiloes`. O estado do caso vive em `memoria-de-caso-leilao`.

## Entrega obrigatoria final
**Via + papel + fase + skill(s) alvo + prazo em curso**, em 3 a 5 linhas, e o handoff para o `leiloes-master`.

## Guard
Nao redigir peca aqui — so classificar e rotear. **Sem a fase travada, nao rotear**: na duvida, perguntar de novo, porque a fase manda na via. Se a demanda toca lance e as **4 provas** nao foram lidas, o roteamento e para o **gate**, nunca direto para estrategia de lance. Demanda mista (o mesmo imovel gerando anulatoria, defesa de IPTU e imissao) sai como **lista ordenada** para o master encadear via `protocolo-p4-leiloes`. Leilao da Lei 14.133 **nao se improvisa**: encaminhar.
