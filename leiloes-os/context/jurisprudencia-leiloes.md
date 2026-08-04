# Jurisprudência de leilões — corpus SELADO (✅ ancorado + 🔴 qualificado) · LISTA NEGRA · PENDENTES · 🟡 NÃO CITAR

> ⚠️ **"✅-only" era rótulo impreciso e foi corrigido em 02/08.** O corpus é **selado**, não exclusivamente ✅: entram também os **🔴 qualificados** (monocrática · afetado sem tese · pendente), **cada verbete com a ressalva embutida**. **Nada entra sem selo** — e o 🔴 entra *porque* precisa ser citável **com a qualificação junto**. Excluí-los deixaria a defesa do devedor sem o REsp 2.165.101 e a due diligence sem o REsp 2.171.564/SP, e o guard não teria como bloquear "monocrática vendida como repetitivo" se a monocrática não estivesse no corpus.

> Anexo de referência do plugin **leiloes-os**. **Regra deste arquivo: só entra no corpus o que foi conferido em fonte oficial (STJ, STF, CNJ) — inteiro teor de acórdão, ficha de precedente, consulta processual eletrônica ou notícia institucional identificada como tal.**
> **Captura:** portal de precedentes e consulta processual do STJ (`processo.stj.jus.br`), inteiro teor certificado (`scon.stj.jus.br`), portal do STF (`portal.stf.jus.br`) e `atos.cnj.jus.br`, em **02/08/2026**. Quatro inteiros teores foram efetivamente abertos (Tema 1.134, RMS 65.084/SP, AgInt nos EREsp 2.042.756/SP e a consulta do ex-AREsp 2.471.891).
> **Legenda:** ✅ conferido em fonte oficial · 🟡 localizado mas **não confirmado** — não citar com número · 🔴 pós-corte de treino, isolado de Turma, monocrático ou pendente.
> **Como usar:** `grep` pelo número (`Tema 1.134`, `RMS 65.084`, `REsp 2.042.756`, `Súmula 478`) e **leia a faixa**. Nunca despeje o arquivo inteiro em contexto.

---

## 0. ⛔ AS QUATRO TRAVAS DESTE ANEXO

1. **Nada da seção §2 LISTA NEGRA pode ser citado como âncora de leilão.** São homônimos, matérias diversas e um erro de digitação do próprio STJ.
2. **Nada da seção §10 PENDENTES pode ser citado como decidido.** Citar pendente como decidido perde a causa e a credibilidade.
3. **Nada marcado 🟡 entra em peça com número.** Roteie ao `validador-leiloes`.
4. **Monocrática nunca vira "tese firmada em repetitivo".** A redação obrigatória para decisão monocrática é ***"o STJ vem anulando"*** / *"o STJ vem decidindo"* — ver §6.

---

## 1. ÍNDICE RÁPIDO — o corpus ✅ em uma linha cada

| Corte | Instrumento | Nº | Tese em uma linha | Selo |
|---|---|---|---|---|
| STJ | Repetitivo | **1.134** | Inválida a cláusula de edital que joga **tributo** anterior no arrematante — sub-rogação **no preço** (CTN 130 §único). **Modulado.** | ✅ |
| STJ | Repetitivo | **1.288** | Consolidada a propriedade sem purga (pós-13.465/2017), resta ao fiduciante "**tão somente**" a preferência do art. 27, §2º-B | ✅ |
| STJ | 3ª Turma + **2ª Seção** | **REsp 2.042.756/SP** | **Edital que informa a dívida ⇒ arrematante RESPONDE** por condomínio (*propter rem*) **+ sucessão processual** | ✅ |
| STJ | 4ª Turma | **RMS 65.084/SP** | Os **5% do leiloeiro são PISO**, não teto — reafirmando o REsp 680.140/RS | ✅ |
| STJ | 5ª Turma | **REsp 680.140/RS** | "**Não há limitação quanto ao percentual máximo**"; **10% validado** | ✅ |
| STJ | 3ª Turma | **REsp 2.198.525** | Remição **após o lance** e antes do auto **não** afasta a comissão; leiloeiro recorre como terceiro prejudicado (CPC 996) | ✅ 🔴 |
| STJ | 3ª Turma | **REsp 2.135.500** | **Registro do contrato** é requisito para usar a via extrajudicial da 9.514 (*supressio*) | ✅ |
| STJ | Turma | **REsp 2.167.979/PB** | Descrição do imóvel no edital **não se vincula ao contrato fiduciário** — deve refletir a situação **atual** | ✅ 🔴 |
| STJ | Repetitivo | **REsp 1.949.182** | IPTU é do **fiduciante** até a **imissão do credor na posse** (nº do Tema 🟡) | ✅ |
| STJ | 1ª Turma | **REsp 1.188.655/RS** | Base do ITBI na arrematação é o **valor alcançado na hasta** — turma, não repetitivo | ✅ |
| STJ | **Monocrática** | **REsp 2.165.101** | Arrematação **abaixo de 50%** da avaliação no **extrajudicial** é preço vil — **monocrática, jamais "repetitivo"** | 🔴 |
| STJ | Súmula | **478** | Cota condominial **prefere** ao crédito hipotecário — **ordem de rateio**, não responsabilidade pessoal | ✅ |
| STJ | Súmula | **128** | Na **execução fiscal** haverá 2º leilão se no 1º não houver lanço superior à avaliação | ✅ |
| STF | Repercussão Geral | **982** | **Constitucional** o procedimento da Lei 9.514/97 — valida **em abstrato** | ✅ |
| STF | Repercussão Geral | **249** | DL 70/66 **recepcionado** — constitucional **porém revogado no núcleo** (arts. 29-41) | ✅ 🔴 |
| STF | ADIs | **7600 · 7601 · 7608** | Lei 14.711 **validada**, com **balizas de conduta** (só dados públicos, vedada força e perseguição) | ✅ |
| STJ | Repetitivo | **1.266** | Penhora de imóvel em AF por dívida condominial — **AFETADO, SEM tese, SEM suspensão nacional**. **Matéria DIVERSA** | 🔴 |
| STJ | 3ª Turma | **REsp 2.171.564/SP** | (ex-AREsp 2.471.891) art. 886, VI no edital extrajudicial — **PENDENTE, sem julgamento** | 🔴 |

---

## 2. 🚫 LISTA NEGRA — o que NUNCA pode ser citado como âncora de leilão

### ⛔ Súmula 121/STF — NÃO É LEILÃO. É ANATOCISMO.

Texto literal conferido na página oficial de aplicação das súmulas do STF: *"É vedada a capitalização de juros, ainda que expressamente convencionada."* A própria página vincula o verbete ao **Tema 33** de repercussão geral (RE 592.377, capitalização de juros na MP 2.170-36/2001) e remete à Súmula 596/STF.

> **Se algum material citar "Súmula 121/STF" a propósito de praça, leilão, arrematação ou intimação do executado, está errado.** Não reproduza. A súmula de leilão que existe e é válida é a **128/STJ**, restrita à **execução fiscal** (§8).

### ⛔ Tema 1.134/STJ NÃO é condomínio — é exclusivamente TRIBUTÁRIO

O ramo do direito registrado na ficha oficial é **Direito Tributário**, e o acórdão **não trata** de despesas condominiais. Estender a tese ao condomínio é erro que inverte o resultado: no condomínio a orientação é **oposta** (§4).

### ⛔ Tema 1.113/STJ (ITBI) NÃO é sobre arrematação

REsp 1.937.821/SP, Rel. Min. Gurgel de Faria, 1ª Seção, j. 24/02/2022 — trata de ITBI **em geral** (base é o valor de mercado declarado, não vinculada ao IPTU; presunção do valor declarado; o município não pode arbitrar previamente por valor de referência). Situação na ficha oficial: *"Acórdão Publicado – RE Pendente"*, **sem trânsito em julgado**, com **RE 1.412.419** (Rel. Min. Cármen Lúcia) concluso no STF. Para arrematação, a âncora é o **REsp 1.188.655/RS** — e é **turma, não repetitivo** (§9).

### ⛔ Tema 1.266/STJ NÃO resolve a responsabilidade do arrematante por condomínio

É sobre **penhorar imóvel alienado fiduciariamente** por dívida condominial. Questão **diversa**. Não citar como saída para o débito condominial do arrematante (§4 e §10).

### ⛔ "REsp 640.140/RS" NÃO EXISTE como precedente-matriz da comissão

O item 1 da ementa do RMS 65.084/SP traz "REsp **640**.140/RS" — é **erro de digitação do próprio acórdão do STJ**. O relatório e o corpo do voto trazem, **três vezes** e corretamente, **REsp 680.140/RS**, Rel. Min. Gilson Dipp, 5ª Turma, j. 02/02/2006, DJ 06/03/2006, p. 429. **Cite sempre 680.140/RS.** Reproduzir o "640.140" é reproduzir o erro (§5).

### ⛔ Matérias que o buscador oferece e que não são deste recorte

| Aparece na busca | O que realmente é | Por que não serve |
|---|---|---|
| **Tema 886/STJ** | Obrigações condominiais do **promissário comprador** (imissão na posse + ciência do condomínio) | Não é arrematante em hasta pública |
| **Controvérsia n. 750/STJ** | Débitos condominiais como créditos **extraconcursais** em recuperação judicial (afetação encerrada 28/10/2025) | Contexto concursal, não arrematação |
| **Tema 1.293** | Matéria aduaneira | Nada com leilão de imóvel |
| **CPC art. 889 + "cônjuge"** | O art. 889 tem **8 incisos fechados e NÃO lista o cônjuge** | A intimação do cônjuge tem sede na disciplina da **penhora de imóvel** |

---

## 3. TRIBUTOS — Tema 1.134/STJ ✅ (e a modulação, lida no acórdão)

### ✅ Tema 1.134/STJ — o arrematante NÃO responde por tributo anterior, ainda que o edital diga o contrário

- **Identificação completa:** REsp **1.914.902/SP** (registro 2021/0003778-1) + REsp **1.944.757/SP** + REsp **1.961.835/SP** · Rel. Min. **Teodoro Silva Santos** · **Primeira Seção** · **julgado em 09/10/2024** · acórdão publicado em **24/10/2024** · **trânsito em julgado em 12/12/2024**. Unânime.
- **Tese firmada (verbatim do dispositivo):**
  > "Diante do disposto no art. 130, parágrafo único, do Código Tributário Nacional, é inválida a previsão em edital de leilão atribuindo responsabilidade ao arrematante pelos débitos tributários que já incidiam sobre o imóvel na data de sua alienação."
- **Fundamento:** CTN art. 130, §único — *"No caso de arrematação em hasta pública, a sub-rogação ocorre sôbre o respectivo preço"* — e a natureza **originária** da aquisição: *"a aquisição da propriedade dar-se-á na sua forma originária, visto que não há relação de causalidade entre o antigo proprietário do bem e seu adquirente"*.
- **Status:** precedente qualificado, **vinculante**, transitado em julgado.

### ✅ A MODULAÇÃO — cláusula literal, extraída do inteiro teor (43 pp., documento certificado)

**Item XIII da ementa** — é por aqui que se cita:

> "Por aplicação analógica do art. 1.035, § 11º, do CPC/2015, a tese repetitiva ora fixada deverá ser aplicada aos leilões cujos editais sejam **publicizados após a publicação da ata de julgamento** do tema repetitivo, **ressalvadas as ações judiciais ou pedidos administrativos pendentes de julgamento, em relação aos quais a aplicabilidade é imediata**."

Mesma cláusula no corpo do voto do Relator (redação ligeiramente diversa, sentido idêntico): *"[…] seja observada pelos editais de leilão publicizados após a publicação da ata de julgamento do presente recurso, ressalvadas as ações judiciais e/ou pedidos administrativos pendentes de apreciação, para os quais a tese se aplica de imediato"*.

**Três precisões que só o inteiro teor dá — e que mudam a peça:**

1. O verbo é **"publicizados"**, não "divulgados". Publicização de edital é **ato formal** — importa para discutir edital **republicado ou aditado**.
2. O marco é a **publicação da ata de julgamento** — não a data da sessão, não a publicação do acórdão.
3. **Cite pelo item XIII da ementa (ou pelo voto), nunca só pelo dispositivo.** O parágrafo do "acordam" transcreve **apenas a tese**, sem repetir a modulação; ele integra o *decisum* por adotar o acórdão "nos termos do voto do Sr. Ministro Relator", mas isoladamente não prova a modulação.

### ⚠️ Resíduo obrigatório — a DATA da ata NÃO é declarada na fonte

A cláusula está confirmada; **a data para a qual ela aponta, não**. Nas fases processuais do REsp 1.914.902/SP **não existe evento de "publicação da ata de julgamento"**. A sequência real registrada é:

```
09/10/2024  Proclamação Final de Julgamento (Primeira Seção)
23/10/2024  Disponibilizado no DJ Eletrônico — EMENTA / ACORDÃO
24/10/2024  Publicado EMENTA / ACORDÃO
24/10/2024  Ofício aos Presidentes dos TJs e TRFs comunicando o resultado
12/12/2024  Trânsito em Julgado
```

O mercado adota **24/10/2024** como marco — que é a data de publicação do **acórdão**. **É convenção, não texto.** Nem o acórdão nem a ficha do tema declaram a data da ata. **Não afirmar "o marco é 24/10/2024" como fato verificado**; escrever "a praxe usa 24/10/2024, mas o acórdão fixa a ata de julgamento e não declara a data".

> **Consequência para a defesa do arrematante em arrematação ANTERIOR à virada:** ele **não** se apoia na modulação — apoia-se em ter **ação judicial ou pedido administrativo já pendente**, hipótese em que a tese incide **de imediato**.

---

## 4. ⭐ CONDOMÍNIO — a orientação é OPOSTA à tributária, e está CONSOLIDADA

> 🚫 **PROIBIDO escrever "a matéria está em aberto no STJ".** A Corte teve a via formal de uniformização — os embargos de divergência — e **a recusou**, por entender que **não há divergência atual**. Dizer "em aberto" é contrariar a fonte primária.

### ✅ A regra vigente — REsp 2.042.756/SP, mantido pela SEGUNDA SEÇÃO

**Formulação canônica (item 5 da ementa do acórdão embargado, transcrita integralmente no acórdão da 2ª Seção):**

> "Segundo a jurisprudência do Superior Tribunal de Justiça, (i) **tendo o imóvel sido alienado em hasta pública com informação no edital acerca da existência de débitos condominiais, responde o arrematante por dívidas condominiais anteriores à arrematação, devido ao caráter *propter rem* da obrigação** e (ii) **é possível a sucessão processual do executado originário pelo arrematante do imóvel quando constante do edital de leilão a existência do débito**."

**Cadeia processual completa (o dado que o mercado não tem):**

```
REsp 2.042.756/SP — 3ª Turma, Rel. Min. Moura Ribeiro,
   Rel. p/ acórdão Min. Ricardo Villas Bôas Cueva, j. 12/11/2024 (DJe 29/11/2024)
   → placar 3×2: Villas Bôas Cueva + Humberto Martins + Antonio Carlos Ferreira
     venceram Moura Ribeiro + Nancy Andrighi (que isentavam pelo CPC art. 908, §1º)
   → resultado: arrematante RESPONDE (o edital informava os débitos)
        ↓
Embargos de Divergência (EREsp) para a SEGUNDA SEÇÃO
        ↓
07/03/2025 — Min. Marco Buzzi INDEFERE LIMINARMENTE os EREsp (DJe 12/03/2025)
        ↓
14/03/2025 — Agravo Interno
        ↓
25/02/2026 — redistribuído por sucessão ao Min. Luís Carlos Gambogi
        ↓
13/05/2026 — SEGUNDA SEÇÃO, UNÂNIME: NEGA PROVIMENTO ao AgInt
             (mantido o indeferimento liminar) — DJe 18/05/2026
        ↓
25/05/2026 — Embargos de Declaração (Petição 521106/2026)
        ↓
06/08/2026 — EDcl no AgInt nos EREsp EM PAUTA, 2ª Seção (Sessão Virtual)
```

**AgInt nos EREsp 2.042.756/SP** — registro 2022/0384739-8 · Rel. Min. **Luís Carlos Gambogi** (Des. convocado do TJMG) · **SEGUNDA SEÇÃO** · **por unanimidade** · Sessão Virtual de 07/05 a **13/05/2026** · DJe **18/05/2026**. Ementa, itens 6 e 7:

> "6. Constata-se a **ausência de similitude fática** entre o acórdão embargado e o acórdão paradigma indicado, pois a conclusão da Turma embargada apoia-se em peculiaridades expressamente destacadas no acórdão recorrido, sobretudo quanto à **informação, em edital de hasta pública, da existência de débitos condominiais** e à consequente responsabilidade do arrematante e sucessão processual.
>
> 7. Os precedentes desta Corte Superior firmam orientação no sentido de que **não se admite a instauração de embargos de divergência com base em entendimento superado ou pretérito, demandando-se divergência atual e contemporânea** ao julgamento questionado […]"

**O sinal mais forte de que a Corte não considera a questão aberta:** votaram com o Relator os Ministros **Nancy Andrighi, João Otávio de Noronha, Humberto Martins, Raul Araújo, Maria Isabel Gallotti, Antonio Carlos Ferreira, Ricardo Villas Bôas Cueva e Daniela Teixeira**; presidiu **Moura Ribeiro**. Ou seja: **os dois vencidos da 3ª Turma participaram e não divergiram** da inadmissão. O paradigma invocado era o REsp 981.544/DF (DJe 18/02/2014), recusado por ser "entendimento superado ou pretérito".

**A divisão 3×2 era *intra*-turma, não *inter*-turmas** — por isso o EREsp não passou. Quem descreve isso como "racha entre Turmas" está errado.

### ⚠️ Consequências práticas que a due diligence DEVE gritar

1. **Nunca afirmar que "o arrematante não responde por condomínio".** É o inverso da regra vigente quando o edital avisa.
2. A responsabilidade vem acompanhada de **sucessão processual** — o arrematante pode ser **incluído no polo passivo** da execução já em curso.
3. **Ler a cláusula de débitos condominiais do edital ANTES do lance decide a responsabilidade.** Uma vez que o edital avisa, a discussão está perdida no STJ. No edital real [E2] esse número era **R$ 53.374,15 + R$ 5.337,41 de honorários**, sobre avaliação de R$ 136.142,37 — **39% da avaliação**.
4. **Não existe tema repetitivo** sobre a matéria. Afirmação de ausência com ônus declarado: foram feitas buscas dirigidas e verificada a via real de uniformização (o EREsp), **não** uma varredura exaustiva do banco de temas. Trate como **"não localizado"**, não como "inexistente".

### 🟡 EDITAL OMISSO — a única brecha real, e ela é de segundo grau

**O que está provado:** a fórmula do STJ é **expressamente condicionada** à informação no edital (*"tendo o imóvel sido alienado em hasta pública **com informação no edital**…"*). A condicionante é parte da *ratio*, não retórica — foi exatamente ela que a 2ª Seção usou para negar similitude fática.

**O que NÃO está provado:** a proposição afirmativa inversa — *"edital omisso ⇒ arrematante não responde"*. É **inferência *a contrario***. O apoio disponível é de **segundo grau**:

- **CPC art. 908, §1º** (lei, não jurisprudência): *"No caso de adjudicação ou alienação, os créditos que recaem sobre o bem, inclusive os de natureza propter rem, sub-rogam-se sobre o respectivo preço, observada a ordem de preferência."* Foi o fundamento dos **vencidos** Moura Ribeiro e Nancy Andrighi.
- **Compilação oficial do TJRJ** sobre leilão e débitos condominiais, que enuncia a regra com a ressalva embutida em acórdãos estaduais que invocam o STJ: *"ressalvada a hipótese de omissão do edital quanto aos referidos débitos"* e *"somente quando o edital é omisso acerca da existência de dívidas condominiais é que o arrematante não deve responder pelos débitos pretéritos de condomínio"*.

**Contra:** **REsp 1.299.081/SP** (contexto **falimentar**), cuja ementa aponta em sentido oposto — *"omissão no edital que não afasta a obrigação"*. **Inteiro teor não aberto.**

> **Regra de escrita:** edital omisso é **tese de defesa bem fundamentada**, com lastro no CPC 908 §1º e em precedente estadual — **jamais regra pacífica**. Sustentar como regra é entregar ao adversário a fonte que a derruba.

---

## 5. ⭐ COMISSÃO DO LEILOEIRO — 5% é PISO, não teto, e NÃO EXISTE TETO

### ✅ RMS 65.084/SP — a decisão que resolve o núcleo

- **Identificação:** RMS **65.084/SP** · registro 2020/0302796-5 · Rel. Min. **Maria Isabel Gallotti** · **Quarta Turma** · **unânime** · **julgado em 27/06/2023** · DJe **03/07/2023** · **trânsito em julgado em 14/09/2023**. Inteiro teor (18 pp.) aberto.
- **Contexto:** leilão em **falência**; a decisão de origem havia **reduzido a comissão do leiloeiro para 2%**, aplicando o Provimento CG 17/2016 do TJSP (art. 266), que tratava os 5% como **teto** (*"arbitrada até o percentual máximo de 5%"*). O STJ **derrubou** essa leitura e concedeu a segurança.
- **Ementa (trechos literais):**
  > "ART. 884, PARÁGRAFO ÚNICO, DO CÓDIGO DE PROCESSO CIVIL. ART. 24, PARÁGRAFO ÚNICO, DO DECRETO 21.981/1932. NATUREZA DE LEI ESPECIAL. **VALOR MÍNIMO DE 5% (CINCO POR CENTO)**. ART. 7º, *caput*, DA RESOLUÇÃO CNJ 236/2016.
  >
  > 1. 'A expressão *obrigatoriamente*, inserta no § único do art. 24 do Decreto-lei nº 21.981/32, revela que a intenção da norma foi **estabelecer um valor mínimo**, ou seja, **pelo menos cinco por cento** sobre o bem arrematado' […]
  >
  > 2. Jurisprudência do STJ que reconhece a **índole de lei especial** ao Decreto 21.981/1932, para dispor sobre o **percentual mínimo** da comissão do leiloeiro, percentual mínimo este também determinado pelo art. 7º, *caput*, da Resolução CNJ 236/2016."

### ✅ REsp 680.140/RS — o precedente-matriz: NÃO HÁ TETO

O voto da Min. Gallotti transcreve **na íntegra** a ementa do precedente-matriz. Trechos **literais**:

> "**VALOR MÍNIMO 5%. LIMITAÇÃO DE VALOR MÁXIMO. INEXISTÊNCIA.** […] **PERCENTUAL DE 10% VÁLIDO.**
>
> II - **Não há limitação quanto ao percentual máximo a ser pago ao leiloeiro a título de comissão.**
>
> III - Não há que se falar na exigência de negociação prévia acerca da remuneração do leiloeiro, pois **com a publicação do edital, o arrematante teve ciência de todos os seus termos, oportunidade em que poderia ter impugnado o valor referente à comissão**.
>
> V - Não se vislumbra óbice à cobrança da taxa de comissão do leiloeiro no percentual de **10%** sobre o valor do bem arrematado."
>
> — 5ª Turma, Rel. Min. **GILSON DIPP**, unânime, j. 02/02/2006, DJ **06/03/2006**, p. 429.

> ⚠️ **Ao citar o precedente-matriz use REsp 680.140/RS.** A ementa do RMS 65.084 traz "640.140/RS" por **erro de digitação do próprio STJ**; relatório e voto trazem 680.140 três vezes. Ver §2.

### ✅ A leitura consolidada — tabela de decisão

| Comando | Leitura confirmada |
|---|---|
| Decreto 21.981/32, art. 24, §único ("obrigatoriamente 5%") | **Piso** — nem valor fixo, nem teto (RMS 65.084 · REsp 680.140/RS) |
| Percentual máximo | **NÃO EXISTE** — *"não há limitação quanto ao percentual máximo"* |
| 10% em leilão judicial | **Expressamente validado** (REsp 680.140/RS, item V) |
| Res. CNJ 236, art. 7º ("no mínimo 5%… fixada pelo magistrado") | **Coerente** com o Decreto: é o piso, e o juiz arbitra acima |
| **7% em leilão judicial** (edital real [E2], por provimento estadual) | **LÍCITO** — está acima do piso, arbitrado na moldura do CPC 884 §único, e o edital dá publicidade prévia |
| Comissão **abaixo** de 5% | **Ilegal**, ainda que arbitrada por juiz ou autorizada por norma estadual — o leiloeiro tem direito à **complementação** (foi o que o STJ concedeu no RMS 65.084) |
| IN DREI 52/2022, art. 75, II, "a" ("comissão **diversa**") | Lê-se como **vedação a cobrar ABAIXO do mínimo legal** |

**Por que a IN DREI não derruba os 7% no leilão judicial (dois fundamentos, ambos verificados):**

1. **Competência.** O CPC art. 882, §1º delegou ao **CNJ** a regulamentação da alienação judicial eletrônica, e o CPC art. 884, §único atribui ao **juiz** o arbitramento. O próprio RMS 65.084 transcreve o **PCA CNJ 0002997-82.2020.2.00.0000** (Rel. Cons. Flávia Pessoa, 81ª Sessão Virtual, unânime, j. 05/03/2021), que reafirmou *"a competência privativa do CNJ para regulamentar a matéria"*. Uma instrução normativa do **DREI** — órgão de registro empresarial — **não** governa o arbitramento judicial da comissão.
2. **Hierarquia e objeto.** A IN DREI 52 é norma **administrativo-disciplinar** que rege a relação leiloeiro ↔ Junta Comercial. Não é norma processual e não pode contrariar a lei especial na leitura que o STJ lhe deu.

### ⭐ O eixo de ataque do arrematante mudou: virou TEMPORAL, não substantivo

O STJ é explícito: *"com a publicação do edital, o arrematante teve ciência de todos os seus termos, oportunidade em que poderia ter impugnado o valor referente à comissão"* (REsp 680.140/RS, item III). **Percentual não impugnado antes do lance, e depois pago, consolida-se.**

> **Impugne ANTES de lançar, ou não impugne.** "O percentual é ilegal" não é mais tese; "o percentual não estava no edital antes do pregão" é.

### ⚠️ Os três resíduos honestos — obrigatórios em qualquer skill que toque comissão

1. **Não existe ato do DREI** (nem parecer, nem decisão) que cite expressamente o art. 75, II, "a", da IN 52/2022 e o declare inaplicável a comissão judicial superior a 5%. A harmonização acima é **construção jurídica ancorada em fontes verificadas**, não um ato de harmonização existente. O **risco disciplinar formal** do leiloeiro perante a Junta Comercial permanece teoricamente aberto.
2. **No leilão EXTRAJUDICIAL da Lei 9.514/97 o raciocínio NÃO se transporta.** RMS 65.084 e REsp 680.140/RS são casos de leilão **judicial** (falência e execução). No extrajudicial **não há juiz arbitrando** — logo, o argumento de competência do item 1 não se aplica, e cobrar acima de 5% fica **mais exposto** ao art. 75, II, "a". **Nenhum julgado localizado sobre essa hipótese.**
3. **São acórdãos de TURMA, não repetitivos.** Não vinculam.

### ✅ 🔴 REsp 2.198.525 — remição depois do lance não afasta a comissão (julho/2026)

- **Identificação:** **Terceira Turma**, unânime, Rel. Min. **Ricardo Villas Bôas Cueva**. Notícia institucional do STJ de **17/07/2026**.
- **Tese:** a arrematação **já existe** com a aceitação do lance e o depósito do preço; a remição feita **antes da assinatura do auto** não retira a comissão, *"desde que seu trabalho tenha sido concluído com resultado útil"*. O acórdão distingue o art. 903 do CPC (momento de **consolidação** dos efeitos) da **existência** da arrematação. Reconheceu também a **legitimidade do leiloeiro para recorrer como terceiro prejudicado** (CPC art. 996).
- **Voto (verbatim da notícia):** *"Condicionar o recebimento da remuneração à perfeição do auto significaria transferir ao leiloeiro o risco de eventos supervenientes à conclusão de seu trabalho, o que não encontra suporte legal e contraria a lógica da remuneração pelo resultado útil da atividade profissional."*
- **⚠️ Ressalvas:** **turma, não repetitivo** — não vincula. O critério é "trabalho concluído com **resultado útil**": **não alcança leilão negativo nem acordo ANTERIOR ao pregão**. Fonte é a **notícia institucional do STJ**; o inteiro teor não foi aberto. **Não localizada** decisão que declare a comissão indevida em acordo celebrado **antes** do leilão.

---

## 6. PREÇO VIL — a régua judicial e a linha extrajudicial (monocrática)

### 🔴 REsp 2.165.101 — MONOCRÁTICA. A redação é "o STJ vem anulando".

- **Identificação:** decisão **monocrática** do Min. **Marco Buzzi**, noticiada em 02/11/2025. Imóvel arrematado por **39,8%** da avaliação → leilão **anulado**. O TJPR havia validado o certame porque o valor superava a dívida; o STJ reformou.
- **Trecho citado:** *"muito embora o artigo 27, § 2º, da Lei 9.514/1997 autorize a venda do imóvel em segundo leilão pelo valor da dívida, a arrematação não poderá ser realizada por preço vil, assim considerado aquele inferior a 50% do valor de avaliação, sob pena de causar um prejuízo exagerado em desfavor do devedor fiduciante"*.
- **🚫 REDAÇÃO OBRIGATÓRIA:** ***"o STJ vem anulando"*** arrematações extrajudiciais abaixo de 50% da avaliação. **NUNCA** "o STJ fixou tese", "tese firmada em repetitivo", "entendimento vinculante" ou "súmula". **Não é repetitivo, não é súmula, é decisão monocrática** — e a linha é construída **contra a literalidade** do art. 27, §2º, da Lei 9.514/97.

### ✅ A régua do leilão JUDICIAL é outra — cascata do CPC 891, §único

Fixado **preço mínimo no edital**, vil é o que fica **abaixo dele**; só na **ausência** de preço mínimo vale o piso supletivo de **50% da avaliação**. Três erros a bloquear: (a) "o CPC fixa 50%" como regra geral — não fixa; (b) o piso valeria só para a 1ª praça — o CPC não separa praças na régua do preço vil; (c) transportar os 50% do CPC para o extrajudicial — lá a régua é própria e de construção judicial.

> **As duas réguas não se misturam.** Judicial = cascata legal ✅. Extrajudicial = construção judicial 🔴 monocrática.

### ✅ REsp 2.167.979/PB — edital deve descrever o imóvel na situação ATUAL

- **Identificação:** julgado em **09/09/2025**; comunicado oficial do STJ em **24/10/2025**.
- **Tese:** a descrição do imóvel no edital **não se vincula à do contrato fiduciário** — deve refletir a **situação atual**. Edital desatualizado → nulidade.
- **⚠️ Mesmo cuidado do REsp 2.165.101:** é **acórdão de turma**, noticiado — **não é repetitivo**. Escreva "o STJ decidiu, em acórdão de turma", nunca "tese firmada".
- **Por que é a melhor tese operacional do domínio:** é **auditável por documento** — lê-se o edital, lê-se a matrícula, compara-se, e o vício aparece sozinho.

---

## 7. EXTRAJUDICIAL / ALIENAÇÃO FIDUCIÁRIA

### ✅ Tema 1.288/STJ — depois da consolidação, resta "tão somente" a PREFERÊNCIA

- **Identificação:** **Segunda Seção**, REsp **2.126.726/SP**, Rel. Min. **Ricardo Villas Bôas Cueva** · afetação 18/10/2024 · **julgado em 10/12/2025** · acórdão publicado 17/12/2025 · **trânsito em julgado em 15/06/2026**. Vide Controvérsia n. 339/STJ; origem IRDR 2166423-86.2018.8.26.0000/SP (Tema 26/TJSP).
- **Tese firmada (verbatim):**
  > "a) antes da entrada em vigor da Lei n. 13.465/2017, nas situações em que já consolidada a propriedade e purgada a mora nos termos do art. 34 do Decreto-Lei n. 70/1966 (ato jurídico perfeito), impõe-se o desfazimento do ato de consolidação, com a consequente retomada do contrato de financiamento imobiliário; e b) a partir da entrada em vigor da Lei n. 13.465/2017, nas situações em que consolidada a propriedade, mas não purgada a mora, é assegurado ao devedor fiduciante **tão somente** o exercício do direito de preferência previsto no § 2º-B do art. 27 da Lei n. 9.514/1997."
- **⚠️ Duas armadilhas:**
  1. **É precedente vivo sobre texto morto** — a questão versava o art. 39, II, da Lei 9.514, **hoje revogado** pela Lei 14.711/2023 (art. 18).
  2. **Não confundir com o art. 26-A, §2º Lei 9.514** (purga possível **até a averbação** da consolidação): o Tema 1.288 cuida do que sobra **depois** de consolidada a propriedade. E **preferência não é purga** — o §2º-B assegura preferência **até a data do 2º leilão**.
- **⚠️ Divergência de data registrada:** a notícia institucional do STJ está datada de **19/02/2026** e circula como se fosse a data do julgamento. **Prevalece o portal de precedentes: 10/12/2025.**

### ✅ Tema 982/STF — a via extrajudicial da 9.514 é constitucional (em abstrato)

- **Identificação:** RE **860.631**, Rel. Min. **Luiz Fux**, **Tribunal Pleno**, mérito julgado em **26/10/2023** (maioria; vencidos os Ministros Edson Fachin e Cármen Lúcia; **tese fixada por unanimidade**) · acórdão publicado no DJE em **14/02/2024** · **trânsito em julgado em 22/02/2024**.
- **Tese literal:** *"É constitucional o procedimento da Lei nº 9.514/1997 para a execução extrajudicial da cláusula de alienação fiduciária em garantia, haja vista sua compatibilidade com as garantias processuais previstas na Constituição Federal."*
- **⚠️ Corrija a memória:** o mérito foi julgado em **26/10/2023**, **não em 2024** — 2024 é publicação e trânsito.
- **⚠️ Limite de alcance:** valida o procedimento **em abstrato**; **não convalida vício concreto** (falta de notificação, preço vil, edital defeituoso). O próprio voto condutor assenta que a via extrajudicial **não exclui o controle judicial**.

### ✅ 🔴 Tema 249/STF — DL 70/66 constitucional, porém revogado no núcleo

- **Identificação:** RE **627.106**, Rel. Min. **Dias Toffoli**, mérito julgado em **08/04/2021** (Sessão Virtual de 26/03 a 07/04/2021), por maioria, **vencidos os Ministros Luiz Fux, Cármen Lúcia, Ayres Britto, Edson Fachin e Marco Aurélio** · acórdão publicado 14/06/2021 · **trânsito em julgado em 22/06/2021**.
- **Tese literal:** *"É constitucional, pois foi devidamente recepcionado pela Constituição Federal de 1988, o procedimento de execução extrajudicial, previsto no Decreto-lei nº 70/66."*
- **🔴 A coexistência que quase ninguém enuncia corretamente:** a **tese** segue formalmente vigente e transitada, mas os **arts. 29 a 41 do DL 70/66 foram REVOGADOS** pela Lei 14.711/2023 (art. 18, I — Capítulo III inteiro), desde 31/10/2023. **O Tema 249 NÃO é fundamento para execução hipotecária extrajudicial nova.** Serve a situações regidas pela lei anterior e como precedente de método. E o **art. 34 do DL 70/66 continua sendo aplicado** pelo Tema 1.288 a situações **anteriores a 2017**.

### ✅ ADIs 7600 · 7601 · 7608 — a 14.711 validada, COM balizas de conduta ⭐

- **Identificação:** **Plenário**, sessão virtual encerrada em **30/06/2025**, Rel. Min. **Dias Toffoli**. Acompanharam integralmente Cristiano Zanin, Alexandre de Moraes, André Mendonça, Edson Fachin, Gilmar Mendes, Luiz Fux, Nunes Marques e Luís Roberto Barroso; **Flávio Dino acompanhou com ressalvas**; **Cármen Lúcia vencida**. Propostas por entidades de oficiais de justiça e magistrados.
- **O que foi validado:** os procedimentos extrajudiciais criados pela Lei 14.711/2023 — consolidação em AF de móveis, busca e apreensão extrajudicial, execução de créditos com garantia hipotecária e execução de garantia imobiliária em concurso de credores.
- **⭐ AS BALIZAS — material de defesa concreta do executado (o ativo prático deste verbete):**
  - **proibidos atos de perseguição** ao devedor e a seus familiares;
  - o cartório ou a empresa especializada **só pode usar dados públicos**;
  - os agentes **não podem usar força física ou psicológica** para constranger o devedor a entregar o bem.
- **🟡 Ressalva:** a **tese exata e o dispositivo** (inclusive eventual interpretação conforme e a extensão da ressalva do Min. Dino quanto ao art. 8º-E do DL 911/69) **não foram lidos no acórdão** — a notícia oficial não os transcreve na íntegra. **Confirmar o dispositivo antes de citar tese literal.** As balizas de conduta, essas, são verificáveis.

### ✅ REsp 2.135.500 — sem registro do contrato, não há via extrajudicial

- **Identificação:** **Terceira Turma**, Rel. Min. **Nancy Andrighi**, notícia institucional de **20/01/2025**.
- **Tese:** *"o registro do contrato é requisito indispensável para a aplicação da Lei 9.514/1997"*; *"a boa-fé objetiva e o instituto da supressio devem ser observados nos casos de contratos de alienação fiduciária"*. No caso, a vendedora deixou de registrar por dois anos (reduzindo custos) e só registrou após o comprador ajuizar rescisão. *"Não se pode admitir que os contratos de venda de imóveis sejam submetidos ao absoluto critério do alienante quanto ao momento do registro."*
- **⚠️** Julgado de **turma**, não repetitivo. A *supressio* foi decisiva **nas circunstâncias do caso** — não é automático que todo registro tardio derrube a via extrajudicial.

### ✅ REsp 1.949.182 — IPTU é do fiduciante até a IMISSÃO do credor

- **Identificação:** Rel. Min. **Teodoro Silva Santos**, julgado em **31/03/2025**, repetitivo.
- **Tese:** *"o credor fiduciário, antes da consolidação da propriedade e da imissão na posse do imóvel objeto da alienação fiduciária, não pode ser considerado sujeito passivo do IPTU, uma vez que não se enquadra em nenhuma das hipóteses previstas no artigo 34 do CTN"*.
- **A data-chave é a IMISSÃO NA POSSE**, não a consolidação isolada.
- **🟡** A tese foi lida em **notícia institucional**; o **número do Tema (1.158?) veio de busca**, não da ficha do portal — **não citar o número do Tema**. Trânsito e eventual modulação **não verificados**.

---

## 8. INTIMAÇÃO, NULIDADE E PREFERÊNCIA

### ✅ Súmula 478/STJ — preferência de rateio, NÃO responsabilidade do arrematante

- **Texto literal:** *"Na execução de crédito relativo a cotas condominiais, este tem preferência sobre o hipotecário."* (SÚMULA 478, SEGUNDA SEÇÃO, j. 13/06/2012, DJe 19/06/2012).
- **⚠️ Escopo:** trata de **ordem de preferência no rateio do produto**. **Não é fundamento para cobrar o arrematante.** Quem a usa nesse sentido está trocando o instituto.

### ✅ Súmula 128/STJ — restrita à EXECUÇÃO FISCAL

- **Texto literal:** *"Na execução fiscal haverá segundo leilão, se no primeiro não houver lanço superior a avaliação."* (SÚMULA 128, PRIMEIRA SEÇÃO, j. 14/03/1995, DJ 23/03/1995, p. 6730).
- **⚠️** Não é regra geral de duas praças para toda execução civil, e **não fixa percentual de preço vil**.

### ✅ A consequência correta da falta de intimação: INEFICÁCIA (CPC 804), não nulidade

O CPC art. 804 fala em **ineficácia** da alienação perante o credor com garantia real, o fiduciário, o promitente comprador e o usufrutuário **não intimados** — regime **distinto** do da nulidade, e que **não depende de demonstração de prejuízo**. O CPC art. 903, §1º, II é expresso ao listar a ineficácia entre as três hipóteses.

> **Para o arrematante isso é PIOR que a nulidade:** ele fica com o imóvel **e com o gravame**, porque o gravame não foi purgado perante quem não foi intimado.

### ⚠️ Intimação pessoal do fiduciante no extrajudicial — forte, mas com três recortes

A linha do STJ é firme quanto à necessidade de intimação pessoal do devedor fiduciante, e o art. 30, §único, da Lei 9.514/97 (redação da 14.711/2023) **excetua expressamente a exigência de notificação** da regra de "resolve-se em perdas e danos" — é a **única alegação que, pelo texto legal, obsta a reintegração**. Mas:

1. Há orientação de que a obrigatoriedade de intimar sobre a **data do leilão** se firmou **após 2017** — o marco temporal importa.
2. Há decisão de **24/08/2025** **dispensando** a intimação em leilão de **bem MÓVEL** com alienação fiduciária. A regra é de **imóvel** (Lei 9.514). **Confundir isso derruba a peça.**
3. As compilações de tribunais estaduais que consolidam a matéria citam AgInt cujo inteiro teor **não foi aberto** — ver §11.

> **Não generalizar "sempre nulo".** O que é seguro afirmar: a intimação é o **eixo único** que sobrou ao fiduciante (art. 30, §único Lei 9.514), e a intimação eletrônica do art. 26, §4º-B Lei 9.514 é hoje a tese de nulidade mais forte que restou.

---

## 9. ITBI NA ARREMATAÇÃO

### ✅ REsp 1.188.655/RS — base é o valor da hasta (turma, não repetitivo)

- **Identificação:** Rel. Min. **Luiz Fux**, **Primeira Turma**, j. **20/05/2010**.
- **Trecho:** *"a arrematação representa a aquisição do bem alienado judicialmente, considerando-se como base de cálculo do ITBI aquele alcançado na hasta pública."* Linha reiterada em AgInt no AREsp 2.050.401, AREsp 1.542.296 e AREsp 1.425.219, segundo notícia institucional do STJ.
- **⚠️ NÃO existe tese repetitiva sobre ITBI em arrematação.** E o **Tema 1.113 não é sobre arrematação** — ver §2.
- **Armadilha de sequência (CPC 901, §2º):** a carta de arrematação deve conter *"a prova de pagamento do imposto de transmissão"* — **o ITBI é pago ANTES de você ter o título**.

---

## 10. ⏳ PENDENTES — proibido citar como decidido

### 🔴 REsp 2.171.564/SP — o antigo AREsp 2.471.891, e o número MUDOU

O agravo foi **convertido em recurso especial** e **deixou de existir com o número antigo**. Fases literais da consulta processual: *"26/08/2024 — Conheço do agravo […] para determinar sua autuação como Recurso Especial"* · *"18/09/2024 — Classe Processual alterada para REsp (Classe anterior: AREsp 2471891)"*.

| Campo | Valor (consulta processual STJ) |
|---|---|
| **Número atual** | **REsp nº 2.171.564/SP** — registro **2023/0324078-8**, autuado em 04/10/2023 |
| Classe anterior | AREsp 2.471.891 |
| **Relatora atual** | Min. **DANIELA TEIXEIRA — TERCEIRA TURMA** |
| Relatores anteriores | Min. Marco Aurélio Bellizze → Min. Carlos Cini Marchionatti (des. convocado TJRS, 10/12/2024) → Min. Daniela Teixeira (05/03/2025, redistribuição por sucessão) |
| Recorrentes | a **instituição financeira credora** **e** o **leiloeiro** (litisconsórcio no polo ativo do recurso) |
| Assunto | Direito Civil — Contratos — **Alienação Fiduciária** |
| Origem | TJSP — processo 1037874-24.2018.8.26.0114 (**Campinas/SP**) |
| **Estado em 02/08/2026** | **No gabinete da Relatora desde 06/03/2025. Última fase: 24/06/2025** (juntada de certidão de retificação de autuação) — **mais de 13 meses de inércia** |

- **Objeto:** se os requisitos do edital do **leilão judicial** (CPC 886, VI — menção a ônus sobre o bem) se aplicam ao **leilão extrajudicial** da Lei 9.514/97. Caso concreto: imóvel com restrições ambientais (contaminação de solo e águas) **omitidas no edital**; o TJSP anulou o negócio por violação ao art. 886, VI; o leiloeiro recorreu alertando que ampliar as exigências *"pode colocar em xeque a segurança de milhares de leilões já feitos"*.
- **🚫 NÃO EXISTE tese do STJ estendendo o art. 886, VI, do CPC ao leilão extrajudicial.** Sem julgamento, sem acórdão, sem decisão monocrática de mérito, sem inclusão em pauta.
- **Como sustentar sem o precedente:** quem alegar nulidade de edital extrajudicial por omissão de ônus deve fundar-se no **dever de informação e na boa-fé objetiva** — **não** em precedente vinculante inexistente.
- **⚠️ Rastreamento:** quem procurar "AREsp 2.471.891" **não acha o andamento atual**. Procure **REsp 2.171.564/SP**.

### 🔴 Tema 1.266/STJ — AFETADO há mais de 2 anos, SEM suspensão nacional

- **Questão submetida (verbatim):** *"Definir se é possível penhorar o imóvel alienado fiduciariamente em decorrência de dívida condominial."*
- **Identificação:** **Segunda Seção**, Rel. Min. **João Otávio de Noronha** · REsp **1.874.133/SP** e **1.883.871/SP** (afetação 21/06/2024, sessão eletrônica de 12/06 a 18/06/2024) + REsp **2.222.937/RS** (afetação 10/09/2025). Vide Controvérsia n. 220/STJ. Campos "Julgado em", "Acórdão publicado em" e "Trânsito em Julgado": **VAZIOS**. Última atualização da ficha: 15/09/2025.
- **⚠️ NÃO HÁ SUSPENSÃO NACIONAL.** O portal registra expressamente a *"Não aplicação do disposto no inciso II do art. 1.037 do CPC e no art. 256-L do RISTJ (suspensão do trâmite dos processos pendentes)"* — os processos **seguem correndo**. Diferença prática relevante em relação ao Tema 1.288 (que teve suspensão).
- **🚫 É MATÉRIA DIVERSA da responsabilidade do arrematante por condomínio.** Não citar como saída (§2 e §4).

### 🔴 EDcl no AgInt nos EREsp 2.042.756/SP — pautado para 06/08/2026

Embargos de Declaração (Petição 521106/2026, protocolados em 25/05/2026) **incluídos em pauta na 2ª Seção, sessão virtual de 06/08/2026**. Incidem sobre **admissibilidade**, não sobre o mérito — mas é **o único movimento vivo da matéria** e o resultado entra na skill. Ver §12.

### 🔴 Vácuo declarado — não há jurisprudência sobre a hipoteca extrajudicial do art. 9º da 14.711

Não foi localizada tese repetitiva nem acórdão do STJ sobre a aplicação concreta do rito hipotecário do art. 9º da Lei 14.711/2023, do art. 27, §5º-A (saldo remanescente) ou do art. 27-A. O que existe é o controle **abstrato** já decidido (ADIs 7600/7601/7608).

> **Afirmação de ausência com ônus declarado:** foram feitas buscas dirigidas, **não** varredura exaustiva de acórdãos de turma. Trate como **"não localizado"**, não como "inexistente".

---

## 11. 🟡 BLOCO SEPARADO — LOCALIZADO MAS NÃO CONFIRMADO (não citar com número em peça)

> **Nada aqui entra em peça com número.** Cada item diz **o que falta** e **para onde rotear**. Isto não é fraqueza do plugin — é o comportamento que os 8 SaaS concorrentes não têm: eles dão resposta binária errada.

| # | Item | O que exatamente não está provado | O que fazer |
|---|---|---|---|
| 1 | **Evicção do arrematante** | **Nenhum julgado do STJ específico de hasta pública** foi localizado. Os dois destacados pela matéria especial do STJ (**AREsp 1.597.745/MT** e **REsp 1.779.055/SC**) tratam de **compra e venda** | A moldura é o **CC 447-457** — **lei, não jurisprudência confirmada**. Declarar o vácuo no corpo da peça. Nunca "o STJ decidiu que o arrematante evicto recebe X" |
| 2 | ***Pas de nullité sans grief* no leilão judicial** | Só snippets de busca; **nenhum acórdão aberto**. Há tensão real com a linha do extrajudicial (que anula pela simples falta de intimação) | **Não presumir o recorte** judicial × extrajudicial. Observe que o **CPC 804 fala em ineficácia**, regime que **não depende de grief** (§8) |
| 3 | **Número do Tema do IPTU do fiduciante ("1.158")** | O número veio de **resultado de busca**, não da ficha do portal de precedentes | Citar **REsp 1.949.182, Rel. Min. Teodoro Silva Santos, j. 31/03/2025** — **sem o número do Tema** |
| 4 | **Data da "publicação da ata de julgamento" do Tema 1.134** | Não consta do acórdão, da ficha do tema nem das fases processuais | Dizer "a praxe usa 24/10/2024, mas é convenção, não texto" (§3) |
| 5 | **"Edital omisso ⇒ arrematante não responde"** | Inferência ***a contrario***; nenhum acórdão do STJ afirma a proposição inversa. Há **REsp 1.299.081/SP** em sentido contrário (falimentar, inteiro teor **não aberto**) | **Tese de defesa bem fundamentada**, nunca regra pacífica (§4) |
| 6 | **Comissão acima de 5% no EXTRAJUDICIAL** | Nenhum julgado localizado. O raciocínio do RMS 65.084 **não se transporta** (não há juiz arbitrando) | Dizer que é a hipótese **mais exposta** ao art. 75, II, "a", da IN DREI 52/2022 (§5) |
| 7 | **Ato do DREI harmonizando o art. 75, II, "a" IN 52/2022** | **Inexistente** até onde se buscou. O risco disciplinar formal do leiloeiro **não está zerado** | Carregar como resíduo em toda skill de comissão (§5) |
| 8 | **Tese e dispositivo literais das ADIs 7600/7601/7608** | A notícia oficial **não transcreve** a tese na íntegra; a ressalva do Min. Dino (art. 8º-E do DL 911/69) não foi confirmada em fonte oficial aberta | Citar **as balizas de conduta** (verificáveis) — não a "tese literal" (§7) |
| 9 | **Números de REsp de fonte secundária** | **Nenhum inteiro teor aberto:** REsp 1.862.902/SP · AgInt no AREsp 1.655.751/RJ · AgInt no REsp 1.898.518/PE · REsp 1.909.196/SP · AgInt no REsp 1.718.272/SP · AgInt no REsp 1.672.508/SP · REsp 1.769.443 · REsp 1.299.081/SP · REsp 1.297.672/SP | Vieram de doutrina e compilações confiáveis. **Conferir antes de citar em peça.** Para o condomínio, o verbete que vale é o **REsp 2.042.756/SP** (§4), que é ✅ |
| 10 | **Prisão do leiloeiro como depositário remisso** (Dec. 21.981/32, art. 27, §4º) | Compatibilidade com a **SV 25/STF** **não verificada** | **Não usar em peça** |
| 11 | **Legitimidade do arrematante terceiro para cobrar a taxa de ocupação** (9.514, art. 37-A) | Não pesquisada | O art. 37-A é ✅ como **lei**; a legitimidade do terceiro é 🟡 |
| 12 | **Revogação da IN DNRC 113/2010** | O ato revogatório **não foi aberto** | O achado é a **desatualização da fundamentação** de editais de 2026, **não uma nulidade provada** |
| 13 | **Decisão do STF sobre exclusividade de leiloeiros públicos** em leilões judiciais | Apareceu em fonte de sindicato/blog; **fonte oficial do STF não aberta** | Não citar |
| 14 | **Dupla contagem da comissão no extrajudicial** (arrematante paga por fora × credor lança como despesa do art. 27, §3º, II Lei 9.514) | Nenhum julgado localizado sobre a dupla contagem | Argumento de **prestação de contas**, não de precedente |

---

## 12. 🔴 GATE DE CALENDÁRIO — conferir ANTES de publicar e a cada atendimento sensível

Três movimentos vivos podem alterar verbetes deste anexo. **Verificar o andamento antes de selar peça que dependa deles:**

| O que | Onde está | Efeito se mudar |
|---|---|---|
| **EDcl no AgInt nos EREsp 2.042.756/SP** — pautado para **06/08/2026** (2ª Seção, sessão virtual) | §4 e §10 | Incide sobre **admissibilidade**, não sobre o mérito — mas o resultado entra na skill de condomínio |
| **REsp 2.171.564/SP** (ex-AREsp 2.471.891) — no gabinete da Min. Daniela Teixeira | §10 | Se julgado e a resposta for "sim, o art. 886, VI se aplica ao extrajudicial", **abala editais já realizados** e cria tese nova de anulação |
| **Tema 1.266/STJ** — afetado, sem suspensão nacional | §2 e §10 | Se julgado, atualizar a **distinção** (penhora de imóvel em AF ≠ responsabilidade do arrematante) |

**Como conferir:** ficha do tema no portal de precedentes do STJ para os repetitivos; consulta processual eletrônica do STJ pelo **número atual** do recurso. Para o REsp 2.171.564/SP, **não** pesquisar pelo número antigo do AREsp.

---

## 13. MAPA — de qual verbete cada skill precisa

| Skill / camada | Verbetes deste anexo |
|---|---|
| `debitos-propter-rem` · `debitos-e-creditos-pos-arrematacao` | §3 (Tema 1.134 + modulação) · **§4 inteiro** (condomínio) · §8 (Súmula 478) · §9 (ITBI) |
| `risco-de-anulacao-do-certame` | §6 (preço vil · REsp 2.167.979) · §7 (Tema 982 · REsp 2.135.500) · §8 (CPC 804) · §10 (REsp 2.171.564 pendente) |
| `analise-de-edital` | §3 (modulação) · §4 (cláusula de condomínio) · §5 (percentual da comissão no edital) · §6 (REsp 2.167.979) |
| `custo-total-real-e-precificacao` | §5 (comissão sem teto) · §9 (ITBI) · §3 (tributo anterior = R$ 0 se pós-virada) |
| `preco-vil-como-tese` | **§6 inteiro** — as duas réguas e a trava da monocrática |
| `defesa-fiduciante-consolidacao-e-purga` · `anulatoria-de-leilao-extrajudicial` | §7 (Tema 1.288 · Tema 982 · REsp 2.135.500) · §8 (intimação) · §6 (preço vil) |
| `leiloeiro-comissao-e-prestacao-de-contas` | **§5 inteiro** + REsp 2.198.525 |
| `eviccao-e-desfazimento-da-arrematacao` | §11 item 1 — **o vácuo é o conteúdo**, declarado no corpo |
| `anti-alucinacao-leiloes` · `validador-leiloes` | §0 · **§2 LISTA NEGRA** · §11 · §12 |
