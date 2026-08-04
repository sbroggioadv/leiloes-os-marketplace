---
name: protocolo-p4-leiloes
description: "Cruzamento multi-esfera do MESMO imovel: judicial x extrajudicial x registral x tributario. Mapeia qual esfera resolve o que e em que ORDEM — anulatoria e invalidacao (judicial), impugnacao de consolidacao e filtro do §15 (registral/extrajudicial), defesa de IPTU/ITBI (tributario) e imissao/reintegracao (possessorio). Evita o erro de protocolar a peca certa no foro errado, ou de atacar preco quando o eixo que sobrou e intimacao. Use quando o mesmo lote gera varias frentes, disserem onde eu ataco primeiro, o juizo da execucao resolve o IPTU, posso anular e registrar ao mesmo tempo, ordem de prioridades."
---

> **🖱️ Escolhas = botoes:** nas perguntas de lista fechada use **AskUserQuestion** (max. 4 por pergunta).

# PROTOCOLO-P4-LEILOES

> Transversal. O imovel e um; as frentes sao quatro. **Errar a esfera e errar o foro, o titulo e o prazo.** Esta skill nao redige a peca — **ordena** qual skill redige, e em que sequencia.

## Anexos obrigatorios (context/)
- `context/jurisprudencia-leiloes.md` — ⭐ **§3 Tema 1.134/STJ + CTN, art. 130, §unico** (tributo no preco); **§4** condominio (edital informa); **§11** vacuos — **grep + ler a faixa**.
- `context/cpc-leilao-879-903.md` — **CPC, arts. 804, 901, 903, 908 §1º** (ineficacia, carta/imissao, relogio dos 10 dias, sub-rogacao no preco) — **grep + ler a faixa**.
- `context/lei-14711-2023.md` — **Lei 14.711, art. 9º** (rito + **§15** filtro + **§11** ata notarial) e **art. 10** (concurso **cartorial**) — **grep + ler a faixa**.
- `context/lei-9514-consolidada.md` — **Lei 9.514, arts. 26/26-A/27/30** (consolidacao, leiloes, reintegracao liminar 60 dias) — **grep + ler a faixa**.
- `context/metodologia-leiloes.md` — fase · papel · via (o relogio da triagem) — **grep + ler a faixa**.

## Objetivo
Devolver um **mapa de esferas** + **ordem de ataque/defesa** + **cross-link** para a skill que executa cada frente — sem duplicar o conteudo delas.

## Metodologia
1. **Botoes: papel?** — **arrematante** · **executado/fiduciante** · **credor** · **terceiro/ocupante**.
2. **Botoes: via do titulo?** — **judicial (CPC)** · **AF extrajudicial (9.514)** · **hipoteca art. 9º (14.711)** · **ainda nao sei**.
3. **Botoes: FASE?** — **antes do leilao** · **pos-lance <10 dias do auto** · **pos-carta/ata** · **pos-imissao/registro**. 🔴 A fase e **irreversivel** no judicial (CPC 903).
4. **Listar frentes abertas** (anulatoria, consolidacao, tributo, posse, registro) e **montar a ordem** abaixo.
5. **Roteiar** cada frente a uma skill de peca; fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## As 4 esferas — o que cada uma resolve

| Esfera | Resolve | NAO resolve | Skill de peca |
|---|---|---|---|
| **JUDICIAL** | Invalidacao / ineficacia / resolucao nos autos (CPC 903 §§1º-2º); acao autonoma pos-carta (903 §4º, arrematante litisconsorte necessario); mandado de imissao nos autos (901) | Consolidacao de AF; concurso cartorial do art. 10 | `anulatoria-de-arrematacao-judicial` · `invalidacao-embargos-e-desistencia-903` · `imissao-na-posse-do-arrematante` |
| **EXTRAJUDICIAL** | Vicio de **notificacao** (unico eixo que ainda obsta reintegracao — 9.514 art. 30 §unico); anulatoria de leilao AF; purga/preferencia | Tributo municipal; ITBI | `anulatoria-de-leilao-extrajudicial` · `defesa-fiduciante-consolidacao-e-purga` · `nulidades-de-intimacao-e-notificacao` |
| **REGISTRAL** | Filtro do **§15 do art. 9º da 14.711** (clausula expressa no titulo = requisito de validade); averbacao da excussao; **ata notarial de arrematacao** (titulo habil, §11); **concurso cartorial art. 10** (habilitacao 15 dias, distribuicao a cargo do credor exequente); baixa de gravames na matricula | Merito de preco vil "como tese STJ vinculante" | `hipoteca-extrajudicial-14711` · `excussao-multipla-e-concurso-de-credores` · `registro-regularizacao-e-itbi` · `leitura-de-matricula` |
| **TRIBUTARIO** | IPTU/tributo **anterior** sub-roga no **preco** (CTN 130 §unico + **Tema 1.134/STJ**); ITBI **antes** da carta (CPC 901 §2º) | Condominio (regime **oposto** — ver abaixo) | `debitos-e-creditos-pos-arrematacao` · `debitos-propter-rem` · `registro-regularizacao-e-itbi` |

## 🚨 Ordem padrao (quando tudo grita ao mesmo tempo)

```
1. FASE / relogio legal          → se o prazo do 903 §2º esta correndo, ELE manda
2. POSSE / reintegracao         → quem esta dentro decide a via (imissao x despejo x reintegracao)
3. TITULO / REGISTRO            → sem titulo correto nao ha matricula limpa nem credito
4. TRIBUTO / ITBI               → ITBI e pre-requisito da carta; tributo anterior e defesa
5. ANULATORIA / consolidacao    → paralela se liminar, mas NAO substitui 1-4
```

### Ajustes por papel

**Arrematante (defesa do ativo):**
1. Se **pos-lance <10 dias**: `invalidacao-embargos-e-desistencia-903` **antes** de qualquer anulatoria longa — o **CPC, art. 903, §2º** e prazo (10 dias do **aperfeicoamento**), nao multa; a multa de **ate 20% do valor atualizado do bem** e o **§6º** (ato atentatorio; base = valor atualizado do bem), **outra base**.
2. **ITBI + carta + registro** em paralelo com defesa de cobranca tributaria (Tema 1.134) — `registro-regularizacao-e-itbi` + `debitos-e-creditos-pos-arrematacao`.
3. **Imissao/reintegracao** so com pre-requisitos pagos (CPC 901 §1º no judicial; consolidacao/ata no extrajudicial).
4. Anulatoria de terceiro so se o titulo ainda nao firmou ou se a via nos autos **fechou** (903 §4º).

**Executado / fiduciante (ataque):**
1. **Antes do leilao:** tutela + vicio de intimacao/notificacao — `tutela-de-urgencia-leiloes` + `nulidades-de-intimacao-e-notificacao`. No extrajudicial, **atacar a intimacao, nao o preco** (art. 30 §unico).
2. **Hipoteca 14.711:** checar **§15** (clausula expressa §§1º-10 no titulo) **antes** de discutir leilao — sem clausula o rito novo **nao se aplica**.
3. **Pos-consolidacao:** anular consolidacao (raiz) > anular so o leilao — `defesa-fiduciante-consolidacao-e-purga`.
4. **Concurso art. 10:** habilitar credito no **cartorio** (15 dias), nao so no juizo.

**Credor:** priorizar consolidacao regular + edital atual + rateio; nao misturar Tema 1.134 com condominio.

## Distincoes que o P4 obriga a escrever

- ⛔ **Tema 1.134/STJ e exclusivamente TRIBUTARIO** — **nao** e condominio. Com edital **informando** divida condominial, o arrematante **RESPONDE** (REsp 2.042.756/SP + AgInt nos EREsp, 2a Secao, unanime, j. 13/05/2026). ⚠️ PENDENTE: EDcl no AgInt nos EREsp 2.042.756/SP (admissibilidade, nao merito). 🚫 **PROIBIDO** "materia em aberto no STJ". Edital **omisso** = **tese**, nao regra.
- ⛔ **Ineficacia ≠ nulidade** (CPC 804 + 903 §1º II): titular de direito real nao intimado — arrematante fica com imovel **e** gravame.
- ⛔ **Carta de arrematacao ≠ ata notarial ≠ carta de alienacao** (CPC 880) — titulo errado = indeferimento no RI.
- 🟡 **Modulacao Tema 1.134:** marco e publicacao da **ata de julgamento**; data da ata **nao declarada** — praxe 24/10/2024 e **convencao**, nao texto. Acoes/pedidos pendentes: aplicacao **imediata**.
- 🟡 **Regulamentacao registral do art. 9º da 14.711** (provimentos estaduais) **nao verificada** — operacionalmente decisiva antes de descrever passo cartorario.
- ⚠️ **REsp 2.171.564/SP** (ex-AREsp 2.471.891; art. 886, VI no extrajudicial) **pendente** na 3a Turma — se julgado "sim", abala editais ja feitos.
- ⚠️ **Tema 1.266/STJ** PENDENTE afetado **sem suspensao nacional** — materia **diversa** (penhora em AF); nao e saida de condominio.
- ⚠️ **EDcl no AgInt nos EREsp 2.042.756/SP** — PENDENTE (admissibilidade); conferir andamento.

## Regras de ouro
- **Uma frente por peca, mapa no parecer.** Nao amontoar anulatoria + ITBI + imissao no mesmo pedido sem competencia e via claras.
- **FASE primeiro.** Passados os 10 dias do 903 §2º sem alegacao, a via nos autos **fechou** — so acao autonoma (§4º).
- **Documento lido.** Matricula, edital, intimacao e certidao tributaria **antes** de ranquear frentes.
- Cross-link soft: triagem → `triagem-leiloes` · risco pre-lance → `risco-de-anulacao-do-certame` · desfazimento/eviccao → `eviccao-e-desfazimento-da-arrematacao` · recursos → C7 · registral geral → `direito-imobiliario-adv-os` · tributo como tributo → `tributario-societario`.

## Entrega obrigatoria final
(a) **Tabela 4 esferas** com frentes abertas/fechadas; (b) **ordem numerada** de ataque/defesa com o **porque legal** de cada passo; (c) **skill de peca** por frente; (d) **prazos-relogio** (903 §2º, purga, 15 dias do art. 10, ITBI antes da carta); (e) **selos 🟡/⚠️** dos pontos pendentes na mesma linha; (f) o que **nao** protocolar ainda por falta de documento. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Nunca misturar **Tema 1.134** com condominio. Nunca chamar de **nulidade** a falta de intimacao do art. 804 (e **ineficacia**). Nunca aplicar o rito do **art. 9º da 14.711** sem checar o **§15**. Nunca pedir imissao judicial sem preco+comissao+despesas+ITBI (901 §1º-2º). Nunca contar os 10 dias do **903 §2º** da ciencia do vicio — correm do **aperfeicoamento**. Nunca confundir **903 §6º** (ate 20% do valor **atualizado do bem**, ato atentatorio) com **896 §2º** (20% da **avaliacao**, incapaz) nem com o **§2º** (prazo de 10 dias). Nunca passo cartorario do art. 9º como se houvesse norma registral nacional verificada. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
