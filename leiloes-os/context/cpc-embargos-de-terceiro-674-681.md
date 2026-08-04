# Anexo — CPC/2015: embargos de terceiro (arts. 674-681)

> **Anexo de legislação do `leiloes-os`.** É a âncora textual da **via do terceiro** prejudicado pela
> constrição (penhora, arresto, sequestro, ou ameaça de constrição) — inclusive do **titular de direito
> real não intimado** e do **possuidor/locatário** que não é parte na execução. Toda skill que citar
> embargos de terceiro fecha aqui — citar de cabeça reprova no `validador-leiloes`.
>
> **Fonte:** texto **compilado** do **CPC (Lei 13.105/2015)** capturado do Planalto em **2026-08-02** —
> `https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2015/lei/l13105.htm`. Transcrição **verbatim**
> a partir da captura já no monorepo (`_planning/civel/fontes/cpc-13105-15.md`, faixa dos arts. 674-681).
> Não redigitada, não parafraseada.
>
> **Legenda:** ✅ conferido verbatim na fonte oficial · 🟡 não confirmado (não citar sem checar) ·
> 🔴 verdade dura / erro de mercado a bloquear · ⭐ eixo do domínio.

---

## ⚠️ AVISO 1 — grep o artigo e leia a faixa. NUNCA despeje o anexo inteiro

Este arquivo é **consulta pontual**, não leitura de contexto. **Faça `grep` do número do artigo e leia
só a faixa correspondente.** Carregar o anexo inteiro numa peça queima contexto e não melhora a
citação. Cada bloco traz: **artigo · texto literal · o que isso decide no leilão · quem usa**.

## ⚠️ AVISO 2 — vigência: a faixa 674-681 NÃO tem nota de alteração (conferido) ✅

Varredura feita na própria captura de 02/08/2026, no intervalo dos arts. 674 a 681: **zero**
ocorrências de `Redação dada`, `Incluído pela`, `Revogado` ou `Vigência` **dentro** da faixa. Os
dispositivos dos embargos de terceiro permanecem com a **redação original da Lei 13.105/2015**.

## ⚠️ AVISO 3 — a pegadinha de Planalto, e por que ela NÃO incide aqui

A página compilada do Planalto exibe, lado a lado, **redação revogada e redação vigente**. **Na faixa
674-681 a armadilha não se materializa**, porque não há redação sucessiva: o texto exibido é único.
**Mas a disciplina permanece:** ao citar **qualquer** artigo do CPC fora desta faixa, conferir na
página se há duas redações antes de transcrever.

## ⚠️ AVISO 4 — 🔴 fronteira com o art. 903 (arrematação já aperfeiçoada)

Os embargos de terceiro **não são** a via de invalidação da arrematação do art. 903. São vias
**distintas**:

| Via | Quem usa | O que ataca | Até quando (âncora) |
|---|---|---|---|
| **Embargos de terceiro** (674-681) | quem **não é parte** e sofre constrição | o **ato constritivo** (penhora etc.) | art. **675**: em execução, até **5 dias depois** da adjudicação/alienação particular/**arrematação**, **sempre antes da assinatura da carta** |
| **Art. 903** (invalidação/ineficácia/resolução) | partes e legitimados do leilão | a **arrematação** já aperfeiçoada | **10 dias** do aperfeiçoamento (assinatura do auto) nas hipóteses do §1º; depois, ação autônoma (§4º) |

⭐ **A fronteira prática:** se a **carta de arrematação já foi assinada**, o prazo do art. 675 **fechou**
para embargos de terceiro contra o ato expropriatório. O que sobra ao terceiro prejudicado é outra
via (ação autônoma, ineficácia do 804 se for titular de direito real não intimado, perdas e danos) —
**não** “embargos de terceiro a qualquer tempo”. A âncora do 903 está em
`context/cpc-leilao-879-903.md`.

## ⚠️ AVISO 5 — 🔴 nota de homônimo (numeração)

Os números **674-681** neste anexo são **só do CPC/2015**. Não confundir com numeração de outros
diplomas do plugin (Lei 9.514, Lei 8.245, Res. CNJ 236, Decreto 21.981, IN DREI 52/2022). Ao grepar
“art. 675” ou “art. 678” no corpus, **confira o diploma na linha**.

---

## 0. O mapa dos embargos de terceiro — o que o leilão precisa

1. **Legitimidade** (art. 674 + §§) — quem é “terceiro” e as quatro hipóteses expressas do §2º.
2. **Prazo** (art. 675) — no processo de conhecimento, até o trânsito; na execução/cumprimento, **5 dias
   depois** da adjudicação, alienação particular ou arrematação, **sempre antes da assinatura da carta**.
3. **Competência e forma** (art. 676) — dependência ao juízo da constrição; carta precatória no deprecado
   (com ressalvas).
4. **Petição e prova sumária** (art. 677) — posse ou domínio + qualidade de terceiro; legitimado passivo.
5. **Efeito suspensivo / posse provisória** (art. 678) — suspensão das medidas constritivas + manutenção
   ou reintegração provisória; caução possível.
6. **Contestação e rito** (art. 679) — 15 dias, depois procedimento comum.
7. **Credor com garantia real** (art. 680) — alegações taxativas do embargado.
8. **Procedência** (art. 681) — cancelamento da constrição indevida + domínio/posse definitivos.

---

## 1. Legitimidade — art. 674 ✅ ⭐

> **Art. 674.** Quem, não sendo parte no processo, sofrer constrição ou ameaça de constrição sobre bens que possua ou sobre os quais tenha direito incompatível com o ato constritivo, poderá requerer seu desfazimento ou sua inibição por meio de embargos de terceiro.
>
> **§ 1º** Os embargos podem ser de terceiro proprietário, inclusive fiduciário, ou possuidor.
>
> **§ 2º** Considera-se terceiro, para ajuizamento dos embargos:
>
> I - o cônjuge ou companheiro, quando defende a posse de bens próprios ou de sua meação, ressalvado o disposto no art. 843;
>
> II - o adquirente de bens cuja constrição decorreu de decisão que declara a ineficácia da alienação realizada em fraude à execução;
>
> III - quem sofre constrição judicial de seus bens por força de desconsideração da personalidade jurídica, de cujo incidente não fez parte;
>
> IV - o credor com garantia real para obstar expropriação judicial do objeto de direito real de garantia, caso não tenha sido intimado, nos termos legais dos atos expropriatórios respectivos.

- **O que decide:** legitimidade **ampla** — dono, possuidor e **fiduciário**; e o §2º, IV é a ponte
  expressa com a **falta de intimação do credor real** (cruzar com **CPC art. 804** e **art. 889** em
  `context/cpc-leilao-879-903.md`).
- ⭐ **No leilão:** o terceiro **dentro do imóvel** (possuidor/locatário) e o **titular de ônus real
  não intimado** são os dois públicos mais comuns desta via.
- **Usa:** `defesa-contra-imissao-e-embargos-de-terceiro` · `nulidades-de-intimacao-e-notificacao` ·
  `situacao-possessoria` · `imissao-na-posse-do-arrematante`.

---

## 2. Prazo — art. 675 ✅ ⭐⭐

> **Art. 675.** Os embargos podem ser opostos a qualquer tempo no processo de conhecimento enquanto não transitada em julgado a sentença e, no cumprimento de sentença ou no processo de execução, até 5 (cinco) dias depois da adjudicação, da alienação por iniciativa particular ou da arrematação, mas sempre antes da assinatura da respectiva carta.
>
> **Parágrafo único.** Caso identifique a existência de terceiro titular de interesse em embargar o ato, o juiz mandará intimá-lo pessoalmente.

- **O que decide:** na execução, o prazo é **curto e de duas condições cumulativas** — (1) até **5 dias
  depois** da adjudicação / alienação particular / **arrematação** e (2) **sempre antes da assinatura
  da carta**.
- 🔴 **Não vender “embargos de terceiro a qualquer tempo” no leilão judicial.** Isso vale no
  **conhecimento** (até o trânsito), não na execução após arrematação.
- ⭐ **Parágrafo único:** se o juízo identifica o terceiro, **intima pessoalmente** — achado de due
  diligence quando a matrícula/ocupação era visível e ninguém foi cientificado.
- **Usa:** `defesa-contra-imissao-e-embargos-de-terceiro` · `triagem-leiloes` · `parecer-go-nogo-lote`.

---

## 3. Distribuição e competência — art. 676 ✅

> **Art. 676.** Os embargos serão distribuídos por dependência ao juízo que ordenou a constrição e autuados em apartado.
>
> **Parágrafo único.** Nos casos de ato de constrição realizado por carta, os embargos serão oferecidos no juízo deprecado, salvo se indicado pelo juízo deprecante o bem constrito ou se já devolvida a carta.

- **O que decide:** **dependência** ao juízo da constrição; autuação **em apartado**. Na precatória, a
  regra é o **deprecado** (com as duas ressalvas do parágrafo único).
- **Usa:** `defesa-contra-imissao-e-embargos-de-terceiro` · `tutela-de-urgencia-leiloes`.

---

## 4. Petição inicial e prova sumária — art. 677 ✅

> **Art. 677.** Na petição inicial, o embargante fará a prova sumária de sua posse ou de seu domínio e da qualidade de terceiro, oferecendo documentos e rol de testemunhas.
>
> **§ 1º** É facultada a prova da posse em audiência preliminar designada pelo juiz.
>
> **§ 2º** O possuidor direto pode alegar, além da sua posse, o domínio alheio.
>
> **§ 3º** A citação será pessoal, se o embargado não tiver procurador constituído nos autos da ação principal.
>
> **§ 4º** Será legitimado passivo o sujeito a quem o ato de constrição aproveita, assim como o será seu adversário no processo principal quando for sua a indicação do bem para a constrição judicial.

- **O que decide:** **prova sumária** de posse/domínio + qualidade de terceiro na inicial; o §2º
  autoriza o possuidor direto a alegar **domínio alheio** (útil ao locatário/comodatário).
- ⭐ **§4º — polo passivo:** quem **se beneficia** da constrição (exequente/arrematante em formação) e,
  se for o caso, quem **indicou** o bem.
- **Usa:** `defesa-contra-imissao-e-embargos-de-terceiro` · `situacao-possessoria`.

---

## 5. Efeito suspensivo e posse provisória — art. 678 ✅ ⭐

> **Art. 678.** A decisão que reconhecer suficientemente provado o domínio ou a posse determinará a suspensão das medidas constritivas sobre os bens litigiosos objeto dos embargos, bem como a manutenção ou a reintegração provisória da posse, se o embargante a houver requerido.
>
> **Parágrafo único.** O juiz poderá condicionar a ordem de manutenção ou de reintegração provisória de posse à prestação de caução pelo requerente, ressalvada a impossibilidade da parte economicamente hipossuficiente.

- **O que decide:** o efeito **não é automático** — depende de decisão que reconheça prova
  **suficiente** de domínio ou posse. Pedido de **manutenção/reintegração provisória** tem de ser
  **expresso**. Caução é faculdade do juiz (com ressalva de hipossuficiência).
- 🔴 **Não prometer “embargos suspendem o leilão automaticamente”.** A suspensão das medidas
  constritivas sobre o bem litigioso exige a decisão do art. 678.
- **Usa:** `tutela-de-urgencia-leiloes` · `defesa-contra-imissao-e-embargos-de-terceiro` ·
  `imissao-na-posse-do-arrematante`.

---

## 6. Contestação e rito — art. 679 ✅

> **Art. 679.** Os embargos poderão ser contestados no prazo de 15 (quinze) dias, findo o qual se seguirá o procedimento comum.

- **O que decide:** contestação em **15 dias**; depois, **procedimento comum**.
- **Usa:** `defesa-contra-imissao-e-embargos-de-terceiro` · `agravo-de-instrumento-leiloes`.

---

## 7. Embargos do credor com garantia real — art. 680 ✅

> **Art. 680.** Contra os embargos do credor com garantia real, o embargado somente poderá alegar que:
>
> I - o devedor comum é insolvente;
>
> II - o título é nulo ou não obriga a terceiro;
>
> III - outra é a coisa dada em garantia.

- **O que decide:** quando o embargante é o **credor real** do 674, §2º, IV, as defesas do embargado
  são **taxativas** (I a III).
- **Usa:** `nulidades-de-intimacao-e-notificacao` · `leitura-de-matricula` ·
  `defesa-contra-imissao-e-embargos-de-terceiro`.

---

## 8. Procedência — art. 681 ✅

> **Art. 681.** Acolhido o pedido inicial, o ato de constrição judicial indevida será cancelado, com o reconhecimento do domínio, da manutenção da posse ou da reintegração definitiva do bem ou do direito ao embargante.

- **O que decide:** procedência → **cancelamento** da constrição indevida + reconhecimento de
  domínio / manutenção / reintegração **definitiva**.
- ⚠️ **Isso desfaz a constrição, não “anula a arrematação” pelo regime do 903.** Se a carta já foi
  assinada, a análise de via muda (AVISO 4).
- **Usa:** `defesa-contra-imissao-e-embargos-de-terceiro` · `reparacao-por-leilao-irregular`.

---

## 9. GUARD — o que este anexo proíbe

1. Citar **art. 674-681 de memória** sem grep neste anexo.
2. Dizer que embargos de terceiro cabem **a qualquer tempo** na **execução** após arrematação (o art.
   **675** corta em 5 dias **e** antes da carta).
3. Prometer **efeito suspensivo automático** (art. **678** exige decisão com prova suficiente).
4. Usar embargos de terceiro como sinônimo de **invalidação do art. 903**.
5. Esquecer o **§2º, IV do art. 674** quando o problema for **credor real não intimado** (cruzar 804).
6. Inventar legitimidade fora do 674 — se não cabe, declarar o limite e rotear ao `validador-leiloes`.

Toda peça fecha por **`suprema-corte-leiloes`** (R1-R4) **+ `validador-leiloes`**.

---

## Fonte e verificação

- **CPC — texto compilado:** `https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2015/lei/l13105.htm`
  — capturado em **2026-08-02**; faixa 674-681 extraída de
  `_planning/civel/fontes/cpc-13105-15.md` (verbatim).
- **Vigência:** varredura na captura confirmou **zero** notas de alteração/revogação na faixa
  **arts. 674 a 681**.
- **Anexos irmãos:** `context/cpc-leilao-879-903.md` (leilão judicial + 804 + 903) ·
  `context/lei-9514-consolidada.md` e `context/lei-14711-2023.md` (extrajudicial — reintegração art. 30
  é regime **próprio**, não embargos de terceiro) · `context/lei-8245-locacao.md` (locatário) ·
  `context/jurisprudencia-leiloes.md`.

### Gap declarado

Nenhum dispositivo da faixa 674-681 faltou na fonte primária do monorepo. **Gap 0** nesta captura.
