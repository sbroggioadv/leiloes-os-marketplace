---
name: memoria-de-caso-leilao
description: "Estado do caso de leilao entre sessoes: identificacao (processo, matricula, comarca, plataforma, leiloeiro por nome e matricula), a VIA e a FASE travadas na triagem, o RELOGIO com todas as datas que geram prazo (edital, pracas, assinatura do AUTO, carta, consolidacao, averbacao, registro da venda, imissao), os numeros (avaliacao, preco minimo, lance, comissao, debitos, teto), e — o campo que decide o gate — o inventario das 4 provas documentais com marcacao ✅ lido x ❌ faltando. Enquanto houver ❌, nenhuma skill de lance roda e o parecer sai NO-GO por insuficiencia de prova. Use ao abrir ou retomar um caso, ao gravar um documento lido ou uma data nova, e quando disserem onde paramos, retoma o caso, ja li a matricula, qual o prazo, o que falta."
---

# MEMORIA-DE-CASO-LEILAO — Estado do caso

> Camada 0. Guarda o que nao pode ser perguntado duas vezes e o que nao pode ser esquecido uma vez. Nao redige e nao opina: registra. **O inventario de provas daqui e o que liga ou desliga o gate DUE-DILIGENCE-FIRST.**

## Anexos obrigatorios (context/)
- `context/metodologia-leiloes.md` — §10 o relogio do leilao (a tabela de prazos e marcos iniciais) · §3 o gate — **grep o artigo e leia a faixa**.
- `context/lei-8245-locacao.md` — o art. 8º §2º verbatim: os **90 dias do locatario correm do REGISTRO**, nao da alienacao — **grep o artigo e leia a faixa**.

## Objetivo e quando ativar
Manter um registro unico, atualizado e honesto do caso, de modo que qualquer skill saiba **em que fase esta**, **o que ja foi lido** e **qual prazo esta correndo**. Roda ao abrir caso novo, ao retomar ("onde paramos"), sempre que um documento for lido ou uma data descoberta, e ao fim de toda entrega.

## O registro

**1. Identificacao** — numero do processo (judicial) ou do procedimento/matricula (extrajudicial) · matricula e cartorio de registro · comarca e UF · plataforma do leilao · **leiloeiro por NOME + MATRICULA** (nunca "a empresa" — credencia-se a pessoa fisica) · situacao do leiloeiro na Junta (regular / licenciado / suspenso).

**2. Classificacao travada** (vem da `triagem-leiloes`) — **VIA:** judicial · extrajudicial AF (9.514) · extrajudicial hipoteca (14.711 art. 9º) · ⛔ administrativo (encaminhado). **PAPEL:** arrematante · executado/fiduciante · credor · leiloeiro. ⭐ **FASE:** antes do lance · pos-lance <10 dias · pos-carta · pos-imissao. **TRILHA:** 🎓 advogado · 💰 investidor.

**3. ⏰ O relogio — datas que geram prazo** (registrar a data **e** o prazo que ela dispara):

| Data a gravar | O que dispara |
|---|---|
| Publicacao do edital · 1a e 2a praca | 5 dias de antecedencia (CPC 887) · ciencia do 889 |
| ⭐ **Assinatura do AUTO** | **10 dias** do 903 §§1º-2º e §5º — contados **daqui**, nao da ciencia do vicio |
| Expedicao da **carta** | fecha o incidental; dali em diante **so acao autonoma** (§4º) |
| Intimacao da mora · intimacao **eletronica** | 15 dias (9.514 art. 26) · 15 dias antes do edital (§4º-B) |
| **Consolidacao** e sua **averbacao** | purga ate a averbacao (26-A §2º) · 60 + 15 dias dos dois leiloes · **1%/mes de taxa de ocupacao desde a CONSOLIDACAO** (37-A) |
| ⭐ **REGISTRO da venda ou do compromisso** (gravar tambem a data da **alienacao**, so como referencia) | **90 dias** para o arrematante denunciar a locacao (8.245 art. 8º §2º) — o prazo corre **do REGISTRO**, nunca da alienacao; perdido, presume-se a manutencao |
| Liminar de reintegracao | 60 dias de desocupacao (9.514 art. 30) |
| Imissao na posse | encerra o carrego; abre a fase indenizatoria |

**4. Numeros** — avaliacao · preco minimo do edital (se houver) · lance · **percentual e valor da comissao** (por fora do lance) · despesas e encargos da plataforma · ITBI (aliquota **a consultar**, nunca presumida) · emolumentos (pela **maior base** — regra de SP, Lei 11.331/2002 art. 7º; fora de SP, tabela local) · debitos de condominio e IPTU levantados · custo estimado de desocupacao · **teto de lance** calculado.

**5. ⭐ Inventario das 4 provas — o campo que liga o gate**

| Prova | Estado | Skill |
|---|---|---|
| [1] EDITAL lido | ✅ / ❌ | `analise-de-edital` |
| [2] MATRICULA lida | ✅ / ❌ | `leitura-de-matricula` |
| [3] OCUPACAO apurada | ✅ / ❌ | `situacao-possessoria` |
| [4] DEBITOS levantados | ✅ / ❌ | `debitos-propter-rem` |

> 🚨 **Enquanto houver um ❌, nenhuma skill de lance roda** e o parecer sai **NO-GO por insuficiencia de prova**. Marcar ✅ significa **documento efetivamente lido** — nunca "o anuncio dizia", "o leiloeiro informou" ou "presumi que estava livre". Fonte de ouvido **nao vira ✅**.

**6. Pendencias e ressalvas** — itens **🟡** que a peca carregou e o que falta conferir (com o roteamento ao `validador-leiloes`) · itens do **gate de calendario** que incidem no caso (EDcl de 06/08/2026 · REsp 2.171.564/SP · Tema 1.266) · **proximo passo com prazo e responsavel**.

## Metodologia
1. Abrir o registro na primeira interacao do caso; **retomar** o existente nas seguintes.
2. Gravar **so o que foi confirmado**, com a origem (documento lido, autos, matricula, edital). Informacao nao confirmada entra como **hipotese marcada**, nunca como fato.
3. Ao ler um documento, marcar ✅ **e** anotar o achado que muda a decisao (onus, ocupante, clausula de debito condominial, gravame fora do edital).
4. Ao gravar uma data, gravar tambem **o prazo que ela dispara** e a data-limite.
5. Ao fim de toda entrega, atualizar ato praticado, proximo passo e prazo.

## Entrega obrigatoria final
Ficha do caso em blocos 1-6, com o inventario das 4 provas em destaque, o prazo mais proximo de vencer no topo e o proximo passo nomeado.

## Guard
🔒 **Zero PII:** nunca gravar nome de cliente, CPF/CNPJ de pessoa fisica, e-mail, telefone, endereco pessoal ou numero de OAB. As partes entram por **papel** (arrematante, fiduciante, credor). O imovel entra por **matricula e comarca**, nao por endereco residencial identificavel.
Nunca marcar ✅ sem documento lido — o inventario e a base do gate, e falsear um ✅ **desarma a unica protecao real do arrematante**. Nunca apagar uma ressalva 🟡 por parecer resolvida: ela sai quando o `validador-leiloes` confirmar, e so entao.
