---
name: registro-regularizacao-e-itbi
description: "Transforma o lance vencedor em PROPRIEDADE REGISTRADA e revendavel: sequencia de pagamento, titulo correto, ITBI, emolumentos, baixa de gravames e regularizacao. Trava a inversao que quebra fluxo de caixa — o ITBI e pago ANTES do titulo, porque a carta de arrematacao tem de conter a prova de pagamento do imposto (CPC, art. 901, §2º), e no extrajudicial da hipoteca o art. 9º, §14 da Lei 14.711 poe ITBI e laudemio antes do registro. Base do ITBI na arrematacao e o valor alcancado na hasta (REsp 1.188.655/RS, turma, NAO repetitivo; o Tema 1.113 nao e sobre arrematacao), e a aliquota municipal nunca vira numero — vira formula e fonte. Emolumento se enquadra pela MAIOR base, entao 50 por cento de desagio nao corta o cartorio pela metade. Use depois de arrematado e quando disserem como registro a carta, quanto vou pagar de ITBI e cartorio, como tiro a hipoteca da matricula, o banco nao financia meu comprador, preciso revender."
---

> **🖱️ Escolhas = botoes:** nas perguntas de lista fechada use **AskUserQuestion** (max. 4 por pergunta).

# REGISTRO-REGULARIZACAO-E-ITBI

> Camada 5. Publico 💰 primeiro. **Arrematar nao e ser proprietario.** Enquanto a matricula nao reflete o novo titular sem gravame, o ativo nao financia, nao revende e nao vale o que a planilha diz.

## Anexos obrigatorios (context/)
- `context/cpc-leilao-879-903.md` — **CPC, art. 901, §§1º e 2º** (sequencia e ITBI na carta) e **CPC, art. 880, §2º, I** (alienacao particular → **carta de ALIENACAO**) — **grep + ler a faixa**.
- `context/custo-total-do-arrematante.md` — §4 (ITBI) e ⭐ §5 (**emolumentos pela MAIOR base**, tres limites honestos) — **grep + ler a faixa**.
- `context/lei-14711-2023.md` — **Lei 14.711, art. 9º, §11** (**ata notarial de arrematacao** = titulo habil) e **§14** (ITBI e laudemio **antes** do registro) — **grep + ler a faixa**.
- `context/jurisprudencia-leiloes.md` — §9 (REsp 1.188.655/RS) e §2 (**Tema 1.113 na lista negra**) — **grep + ler a faixa**.
- `context/clausulas-armadilha-de-edital.md` — **ARM-03** (ad corpus / area), **ARM-05** (catch-all / baixa de hipoteca), **ARM-08** (laudemio e emolumentos) — **grep + ler a faixa**.

## Objetivo
Devolver a **sequencia executavel** ate a matricula limpa, com **cada custo em formula e fonte**, o que **falta** de documento, e o que **nao** se resolve no cartorio.

## Metodologia
1. **Botoes: qual titulo?** — **carta de arrematacao (judicial)** · **carta de alienacao (CPC 880)** · **ata notarial (hipoteca Lei 14.711)** · **consolidacao/leilao Lei 9.514**. 🔴 **Nao sao o mesmo documento** nem o mesmo rito.
2. **Conferir conteudo obrigatorio do titulo** e **rodar a sequencia de pagamento** na ordem — textual, nao pedagogica.
3. **Calcular ITBI e emolumentos por FORMULA** + fonte. **Nunca numero.**
4. **Mapear gravames** da matricula: o que cai **e por qual mecanismo**, e o que **sobrevive**.
5. **Listar regularizacao pendente**. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## 🚨 A SEQUENCIA E INVERTIDA — pague antes do titulo e da posse

```
preco  ->  comissao  ->  despesas  ->  ITBI  ->  CARTA  ->  mandado de imissao  ->  REGISTRO
```

- **CPC, art. 901, §1º:** carta e mandado so apos deposito do preco + **comissao + demais despesas** da execucao.
- **CPC, art. 901, §2º:** a carta contem descricao do imovel, remissao a matricula, copia do auto, ⭐ **prova de pagamento do imposto de transmissao** e **indicacao de eventual onus real ou gravame**.
- **Extrajudicial da hipoteca:** **Lei 14.711, art. 9º, §14** — **ITBI e, se o caso, laudemio** ao registro **antes** do ato.

> 🚨 **Quem planejou pagar o ITBI "depois, com o aluguel" trava a propria carta.** Conta completa em `custo-total-real-e-precificacao` — aqui vira **cronograma de desembolso**.

⚠️ Carta que silencia sobre gravame conhecido e **documento defeituoso** (CPC 901, §2º). Conferir a indicacao **antes** de receber.

## ITBI — base ✅, aliquota 🟡, lista negra

- ✅ **Base:** valor **alcancado na hasta**, nao o venal — **REsp 1.188.655/RS**, Rel. Min. Luiz Fux, **1a Turma**, j. 20/05/2010. ⚠️ **TURMA. Nao existe tese repetitiva sobre ITBI em arrematacao.**
- ⛔ **Tema 1.113/STJ NAO e sobre arrematacao** — ITBI em geral, **sem transito**. Cita-lo como se fosse do arrematante e lista negra.
- 🟡 **Aliquota: varia por municipio; NAO pesquisada neste corpus.** **NUNCA dar o numero.** Formula: `aliquota municipal x base da arrematacao` → legislacao do municipio do imovel.
- ✅ **Extrajudicial Lei 9.514, art. 24, §unico:** prevalece a **base do ITBI quando maior**.

## 🚨 EMOLUMENTOS — pela MAIOR base (regional)

Em **Sao Paulo**, **art. 7º da Lei estadual 11.331/2002** enquadra pelo **MAIOR** entre **preco declarado** (lance), **valor tributario do IPTU** e **base do ITBI** — **§unico**: **valor da avaliacao judicial** quando a lei exigir.

> 🚨 **50% de desconto sobre a avaliacao NAO corta o emolumento pela metade.**

🟡 **Tres limites honestos, obrigatorios sempre que esta linha for citada:** (a) emolumento e **estadual** e **so SP verificado** — demais estados: **formula + tabela local**, **nunca extrapolar SP**; (b) **nao existe item "carta de arrematacao"** — usa-se o generico de **registro com valor declarado**; (c) faixas com **OCR corrompido** nao se reproduzem — conferir PDF original. Duvida: **formula e fonte** → `validador-leiloes`.

⚠️ **Laudemio:** imovel **foreiro** (enfiteuse / marinha) pode somar dezenas de milhares. **Checar na matricula** → `leitura-de-matricula`.

## Baixa de gravames

| Gravame | Mecanismo | Cuidado |
|---|---|---|
| **Tributo anterior** | sub-roga-se no **preco** (**CTN, art. 130, §unico** + **Tema 1.134/STJ**) | ✅ com a **modulacao** — `debitos-e-creditos-pos-arrematacao` |
| **Penhoras/onus** de titular **intimado** | caem com o titulo, na forma do juizo | conferir **intimacao** nos autos, uma a uma |
| 🔴 **Onus de titular NAO intimado** | **NAO cai** | **CPC, art. 804**: arrematacao **INEFICAZ** perante ele — imovel **e gravame** → `risco-de-anulacao-do-certame` |
| **Hipoteca** | edital-ancora **[E1]** invoca **art. 1.499 do CC**, *"uma vez tendo o referido credor sido intimado"* | 🟡 **condicionante = intimacao** |

🟡 **Ressalva de segunda mao:** o **art. 1.499 do CC** aparece neste corpus **dentro de clausula de edital de terceiro** (ARM-05), **nao** em captura verbatim do CC — **nao ha anexo do CC nestes onze**. Conferir o texto no diploma antes de usar em peca → `validador-leiloes`.

## Regularizacao
Construcao **nao averbada**, **habite-se** ausente ou **divergencia de area**: custo de **projeto + INSS + averbacao**. Enquanto pendente, **comprador seguinte nao consegue credito** — saida presa a comprador a vista. Confrontar **matricula x IPTU x planta** (ARM-03) e **orcar no pior cenario**: com "no estado em que se encontra" e renuncia a vicio oculto, o custo e **do arrematante**.

🟡 **Lacuna do rito novo:** **nao verificado** se ha provimento da Corregedoria Nacional ou norma estadual sobre **averbacao da excussao**, **ata notarial de arrematacao** e concurso do **art. 10 da Lei 14.711**. **Antes de protocolar passo cartorario do art. 9º da Lei 14.711, conferir norma registral do Estado** → `validador-leiloes`.

## Regras de ouro
- ⛔ **NUNCA dar numero** de aliquota de ITBI, emolumento fora de SP ou custas. Formula + fonte. **Custas nao pesquisadas.**
- 🔴 **Titulo errado = pedido indeferido.** Arrematacao → **carta de arrematacao**; alienacao particular → **carta de ALIENACAO** (**CPC 880, §2º, I**, por **termo nos autos**); hipoteca do **art. 9º da Lei 14.711** → **ata notarial de arrematacao** (tabeliao de notas = **titulo habil**). 🟡 **Nao estender automaticamente o CPC 903 a alienacao particular** — ponto em aberto.
- ⏰ **Judicial: carta so apos 10 dias do CPC 903, §2º** sem alegacao (§3º). Pedir antes e perder tempo.
- ⛔ **Nao afirmar matricula "limpa" sem matricula atualizada pos-registro.**
- Cross-link soft: conta → `custo-total-real-e-precificacao` · gravames pre-lance → `leitura-de-matricula` · titulo judicial → `arrematacao-auto-e-carta` · posse → `imissao-na-posse-do-arrematante` · ITBI/ganho de capital → `tributario-societario` / `cfo-combativo-os` · registro fora do leilao → `direito-imobiliario-adv-os`.

## Entrega obrigatoria final
(a) **Titulo correto** conferido contra o conteudo legal; (b) **cronograma de desembolso** na ordem textual; (c) **ITBI e emolumentos em formula + fonte**, selo 🟡 onde regional; (d) **mapa de gravames**: o que cai, **por qual mecanismo**, e o que **sobrevive** por falta de intimacao; (e) **plano de regularizacao** e o que destrava; (f) documentos faltantes. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Nunca **numero** de aliquota de ITBI, emolumento fora de SP ou custas. Nunca emolumento **pelo lance** se IPTU ou base do ITBI forem maiores. Nunca **Tema 1.113/STJ** como arrematacao, nem **REsp 1.188.655/RS** como repetitivo. Nunca prometer ITBI **depois** do titulo. Nunca chamar de "carta de arrematacao" o titulo do **CPC 880** (e **carta de alienacao**) nem o do **art. 9º da Lei 14.711** (e **ata notarial**). Nunca baixa de hipoteca pelo **art. 1.499 do CC** sem conferir o diploma — aqui so aparece **citado em edital de terceiro**. Nunca gravame caido sem **intimacao** do titular (CPC 804). Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
