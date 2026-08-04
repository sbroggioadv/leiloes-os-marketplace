---
name: suprema-corte-leiloes
description: "Gate de qualidade final do plugin leiloes, default-on. Aplica 4 validacoes antes de qualquer entrega: R1 fatos, papel e FASE (arrematante x executado-fiduciante x credor x leiloeiro; antes do lance, pos-lance <10 dias, pos-carta, pos-imissao; e as 4 provas documentais quando a demanda toca lance), R2 fundamentacao vigente (nunca DL 70/66 arts. 29-41, a 14.711 no lugar; monocratica nunca como repetitivo; pendente sempre como pendente), R3 prazos e dies a quo (10 dias do 903 §2º contados do APERFEICOAMENTO, 15/60/15 do extrajudicial, 90 dias do locatario contados do REGISTRO da venda ou do compromisso, 1%/mes desde a CONSOLIDACAO), R4 forma, via e competencia (incidental nos autos x acao autonoma com litisconsorcio x via extrajudicial). Use SEMPRE antes de entregar peca, parecer ou dossie; acionada pelo leiloes-master ao fechar qualquer ato, ou quando disserem revisao final, confere a peca, pode protocolar, /revisao-final-leiloes."
---

# SUPREMA-CORTE-LEILOES — Gate R1-R4

> Camada 0. Auditoria final obrigatoria e **default-on**: nenhuma entrega do plugin sai sem passar por aqui. Opera **depois** do `validador-leiloes` (que cruza citacao por citacao) e do guard `anti-alucinacao-leiloes` (que atua na geracao).

## Anexos obrigatorios (context/)
- `context/cpc-leilao-879-903.md` · `context/lei-9514-consolidada.md` · `context/lei-14711-2023.md` · `context/resolucao-cnj-236-2016.md` · `context/leiloeiro-decreto-21981-in-drei-52.md` · `context/jurisprudencia-leiloes.md` · `context/clausulas-armadilha-de-edital.md` · `context/custo-total-do-arrematante.md` · `context/mercado-leiloes-2026.md` · `context/metodologia-leiloes.md` · `context/lei-8245-locacao.md` — **grep o artigo e leia a faixa**, nunca despejar o anexo inteiro.

## Objetivo e quando ativar
Devolver veredito binario — **LIBERADO** ou **CORRIGIR** — sobre a entrega, com a lista do que foi checado em cada regua. Nao redige: audita. Roda ao fechar qualquer ato (peca, parecer, dossie, impugnacao, contrato), automaticamente pelo `leiloes-master`, ou a pedido ("revisao final", "pode protocolar?").

## As 4 validacoes

**R1 — Fatos, papel e FASE.** Os fatos batem com a `memoria-de-caso-leilao`? O **imovel** esta qualificado (matricula, comarca, avaliacao, lance, onus averbados)? O **papel** esta fixado — arrematante · executado/fiduciante · credor/exequente · leiloeiro? ⭐ **A FASE esta travada** — antes do lance · pos-lance **<10 dias do auto** · pos-carta · pos-imissao? **A fase decide a via e nao volta atras.** E, se a demanda toca **lance, arrematacao ou "vale a pena"**: as **4 provas documentais** (edital · matricula · ocupacao · debitos) foram **lidas**? Faltando qualquer uma, a entrega correta e **NO-GO por insuficiencia de prova** — reprovar parecer que afirme situacao do imovel sem documento.

**R2 — Fundamentacao vigente.** Cada dispositivo, sumula e tema existe e esta vigente? Travas duras: **DL 70/66 arts. 29-41 REVOGADOS** (14.711 art. 18, I) desde 31/10/2023 — o rito por agente fiduciario **nao pode aparecer como vigente**; o rito hipotecario e o **art. 9º da 14.711**, com o **filtro do §15**; **art. 889 tem 8 incisos e NAO lista o conjuge**; **Tema 1.134 e tributario**, nao condominial, e vem **com a modulacao** (item XIII da ementa, verbo "publicizados"); **REsp 2.165.101 e MONOCRATICA** — so "o STJ vem anulando"; **5% e PISO, sem teto** (RMS 65.084/SP · **REsp 680.140/RS**, nunca "640.140"); **Sumula 121/STF nao e de leilao** e a **128/STJ** e so de execucao fiscal; **condominio com edital informando: o arrematante RESPONDE** (consolidado) — 🚫 reprovar "materia em aberto no STJ"; **eviccao do arrematante = vacuo declarado** (CC 447-457 e lei). Materia **pendente** (REsp 2.171.564/SP · Tema 1.266 · EDcl de 06/08/2026) esta citada **como pendente**? Todo precedente consta como ✅ em `jurisprudencia-leiloes.md`?

**R3 — Prazos e dies a quo.** O prazo esta certo e o marco identificado? **10 dias** do 903 §§1º-2º e §5º contados do **APERFEICOAMENTO (assinatura do auto)**, jamais da ciencia do vicio — e o **erro mais caro do dominio**; **5 dias** de publicacao do edital (887), de ciencia do 889 e de abertura do leilao eletronico (Res. CNJ 236 art. 11); **3 min / 15 s** de prorrogacao (art. 21); **1 dia** de deposito e **2** de contas (884); **15 dias** de intimacao da mora (9.514 art. 26) e **15 dias** da **intimacao eletronica** antes do edital (§4º-B); **purga ate a AVERBACAO** no residencial (26-A §2º); **60 + 15 dias** dos dois leiloes (art. 27 · 14.711 art. 9º §§3º e 6º); **5 dias** (AF) x **15 dias** (hipoteca) para o excedente; **30 dias** da excussao sucessiva (27-A §3º); **60 dias** de desocupacao apos a liminar (art. 30); ✅ **90 dias** do locatario contados do **REGISTRO da venda ou do compromisso** (8.245 art. 8º §2º, verbatim) — perdido, presume-se a manutencao; **reprovar peca que conte da ALIENACAO**, porque o registro e posterior e contar da alienacao mata prazo que ainda corre (`context/lei-8245-locacao.md` — **grep o artigo e leia a faixa**); **1%/mes sobre o valor do art. 24, VI** de taxa de ocupacao desde a **CONSOLIDACAO** (37-A), nao desde o leilao.

**R4 — Forma, via e competencia.** A **via** esta certa? Dentro dos 10 dias ⇒ **incidental nos proprios autos**; depois da carta ⇒ **acao autonoma** (903 §4º) com o arrematante como **litisconsorte necessario** — inverter isso extingue a peca. Imissao: **judicial e mandado nos proprios autos** (901 §1º), so apos preco + comissao + despesas + **ITBI**; **extrajudicial e acao propria** com **liminar e 60 dias** (art. 30). No extrajudicial, lembrar que **so a notificacao obsta** a reintegracao (30 §unico). Enderecamento, qualificacao, valor da causa, CPC 319, tutela (CPC 300) quando cabivel. E o **freio do 903 §6º**: vicio infundado para forcar desistencia e ato atentatorio, multa de ate **20%** — reprovar peca especulativa, sem lastro documental.

## Metodologia
1. Rodar R1 → R2 → R3 → R4, nesta ordem.
2. Marcar cada item OK / CORRIGIR, citando o anexo e a faixa conferida.
3. Havendo CORRIGIR, devolver a skill de origem com o substituto proposto; **nao entregar**.
4. Liberar so quando R1-R4 = OK.

## Regras de ouro
- **Gate default-on:** ninguem pula a Suprema Corte por urgencia. Peca com prazo curto se corrige mais rapido, nao se libera sem gate.
- **Na duvida em R2/R3, o default e remover ou checar ao vivo** — nunca chutar numero.
- **Reprova automatica:** DL 70/66 arts. 29-41 como rito vivo · 10 dias contados da ciencia do vicio · afirmacao sobre o imovel sem documento lido · "materia em aberto no STJ" no condominio · monocratica vendida como repetitivo · pendente vendido como decidido · numero de aliquota de ITBI, emolumento fora de SP ou custas · promessa de 70% de desconto ou "leilao e seguro".
- **Postura honesta preservada:** condicionante do condominio exposta, vacuo da eviccao declarado, residuos da comissao no extrajudicial ditos. Resposta unica onde a jurisprudencia e condicionada, monocratica ou ausente **e alucinacao com cara de certeza**.

## Entrega obrigatoria final
Veredito (**LIBERADO** / **CORRIGIR**) + lista do que foi checado por regua + correcoes propostas com a ancora substituta.

## Guard
Nao "passar pano". Item nao confirmado nao vira item aprovado — vira pendencia. Se o `validador-leiloes` deixou algo em **CHECAR AO VIVO**, a peca **nao e liberada** ate a checagem ser feita na fonte oficial. E se a demanda tocava lance sem as 4 provas, o veredito e **CORRIGIR**, qualquer que seja a qualidade do texto.
