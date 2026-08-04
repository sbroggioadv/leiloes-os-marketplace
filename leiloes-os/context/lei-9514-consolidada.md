# Anexo — Lei 9.514/97 consolidada pós-Lei 14.711/2023 (alienação fiduciária de imóvel)

> **Anexo de legislação do `leiloes-os`.** É o corpo do **leilão extrajudicial** da alienação
> fiduciária: consolidação, intimação, os dois leilões, purga × preferência, saldo remanescente e
> reintegração. **Toda transcrição abaixo é a REDAÇÃO VIGENTE**, selecionada dispositivo a dispositivo.
>
> **Fonte:** texto **compilado** da **Lei 9.514/1997** capturado do Planalto em **2026-08-02** —
> `https://www.planalto.gov.br/ccivil_03/leis/l9514.htm`. Transcrição **verbatim** por script.
>
> **Marco temporal:** a **Lei 14.711/2023** (Marco das Garantias) está em vigor desde **31/10/2023**.
>
> **Legenda:** ✅ vigente conferido · 🟡 não confirmado · 🔴 verdade dura / mudança pós-cutoff · ⭐ eixo.

---

## ⚠️ AVISO 1 — grep o artigo e leia a faixa. NUNCA despeje o anexo inteiro

Consulta pontual. **`grep` do número do artigo e leia só a faixa.**

## ⚠️ AVISO 2 — 🔴 PEGADINHA DE PLANALTO **TRAVADA** (esta é a lei onde ela mais morde)

A página compilada da Lei 9.514 exibe **a redação revogada AO LADO da vigente** — e aqui não é uma
exceção pontual: é a regra. Contagem feita na captura de 02/08/2026, de redações **superadas**
descartadas por dispositivo:

| Artigo | Redações superadas na página | Quantas versões o caput tem |
|---|---|---|
| **art. 26** | 8 | 2 (original × Lei 14.711/2023) |
| **art. 27 Lei 9.514** | 11 | 2 (prazo de **30 dias** × **60 dias**) |
| **art. 39** | 5 | 3 |
| **art. 37-A** | 2 | **4** (MP 2.223/2001 → Lei 10.931/2004 → Lei 13.465/2017 → Lei 14.711/2023) |
| **art. 30** | 2 | 2 |
| **art. 24** | 4 | — (incisos I, V e VII trocados) |

🔴 **Quem lê a página de cima para baixo e copia a primeira ocorrência copia TEXTO REVOGADO.** Os dois
erros mais prováveis, e que este anexo existe para impedir:

- citar o **art. 27, caput Lei 9.514** com **"prazo de trinta dias"** — o prazo vigente é de **60 dias**;
- citar o **art. 37-A** com **"desde a data da alienação em leilão"** — o termo inicial vigente é a
  **data da CONSOLIDAÇÃO**.

**Neste anexo a seleção foi feita por script**, mantendo por dispositivo a **última redação anotada**
(`Redação dada` / `Incluído`), e as superadas foram descartadas. Ao conferir na fonte, **role até o
fim do dispositivo**: a redação vigente é a **última**, e traz a nota de alteração.

## ⚠️ AVISO 3 — 🔴🔴 A CORREÇÃO MAIS IMPORTANTE DESTE ANEXO: o IPTU/condomínio **NÃO** é texto morto

O BUILD-CONTRACT (correção nº 11) e o design-spec dizem que a regra que põe **IPTU e taxas
condominiais a cargo do fiduciante** seria "dispositivo da MP 1.162/2023 que não vingou" e que citá-la
é "citar texto morto". **A conclusão está certa pela METADE, e a razão está errada.** Conferido na
fonte em 02/08/2026:

1. ❌ **A MP 1.162/2023 NÃO "deixou de vingar".** A página do Planalto diz, no cabeçalho:
   **"Convertida na Lei nº 14.620, de 2023"**
   (`https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2023/mpv/mpv1162.htm`). Argumentar em peça que
   "a MP não foi convertida" é afirmação **falsa e facilmente refutável** pela parte contrária.
2. ✅ **O que morreu foi o ENDEREÇO, não a regra.** A MP inseriu o dispositivo no **art. 24, §2º**. A lei
   de conversão (**Lei 14.620/2023, art. 28**) o promulgou em **outro artigo**: o **art. 23, §2º**. Na
   Lei 9.514 compilada, o **parágrafo único do art. 24** (Lei 13.465/2017) aparece **restaurado**, e os
   "§§1º e 2º do art. 24" ficam com atribuição **apenas da MP** — ou seja, sem eficácia.
3. 🔴 **Portanto: "art. 24, §2º" = citação morta. Mas a REGRA ESTÁ VIVA no art. 23, §2º**, incluído
   pela Lei 14.620/2023 (§1 deste anexo).

⭐ **Consequência de produto:** dizer ao usuário que **"não existe dispositivo legal pondo IPTU e
condomínio no fiduciante"** é **ERRO** — existe, e está em vigor. O que não existe é no art. 24.
Skills afetadas: `debitos-propter-rem`, `custo-total-real-e-precificacao`,
`debitos-e-creditos-pos-arrematacao`, `base-legal-alienacao-fiduciaria`.

---

## 1. Constituição da propriedade fiduciária e o ENCARGO DO FIDUCIANTE — art. 23 ✅ 🔴⭐

> **Art. 23.** Constitui-se a propriedade fiduciária de coisa imóvel mediante registro, no competente Registro de Imóveis, do contrato que lhe serve de título.
>
> **§ 1º** Parágrafo único. Com a constituição da propriedade fiduciária, dá-se o desdobramento da posse, tornando-se o fiduciante possuidor direto e o fiduciário possuidor indireto da coisa imóvel. (Incluído pela Lei nº 14.620, de 2023)
>
> **§ 2º** Caberá ao fiduciante a obrigação de arcar com o custo do pagamento do Imposto sobre a Propriedade Predial e Territorial Urbana (IPTU) incidente sobre o bem e das taxas condominiais existentes. (Incluído pela Lei nº 14.620, de 2023)

🔴 **Leia a estrutura com cuidado — a página tem um artefato de renumeração.** A Lei 14.620/2023
**transformou o antigo parágrafo único em §1º** (mesmo texto: desdobramento da posse) **e acrescentou o
§2º**. Por isso a página exibe o rótulo antigo "Parágrafo único." dentro do que hoje é o **§1º**. O
dispositivo vigente é **§1º**, não "parágrafo único".

⭐⭐ **O §2º é o dispositivo que o mercado inteiro procura no lugar errado:**

| | Onde o mercado procura | Onde ESTÁ |
|---|---|---|
| IPTU + taxas condominiais a cargo do **fiduciante** | ❌ art. 24, §2º (MP 1.162 — **sem eficácia**) | ✅ **art. 23, §2º** (Lei 14.620/2023) |

⚠️ **Limite honesto de leitura — não transformar o §2º em bala de prata.** O §2º regula a relação
**fiduciante × fiduciário** (quem arca com o custo **no contrato**). Ele **não** decide, por si, a
responsabilidade do **arrematante** perante o município ou o condomínio, que é matéria de **obrigação
propter rem** e de **CPC 908, §1º** / **CTN 130, §único** — ver `context/jurisprudencia-leiloes.md`.
Usar o art. 23, §2º como se resolvesse a dívida do arrematante é erro de nível oposto ao anterior.

- **Usa:** `base-legal-alienacao-fiduciaria` · `debitos-propter-rem` ⭐ ·
  `custo-total-real-e-precificacao` · `debitos-e-creditos-pos-arrematacao` · `leitura-de-matricula`.

---

## 2. Requisitos do contrato e o valor para leilão — art. 24 ✅

> **Art. 24.** O contrato que serve de título ao negócio fiduciário conterá:
>
> I - o valor da dívida, sua estimação ou seu valor máximo; (Redação dada pela Lei nº 14.711, de 2023)
>
> II - o prazo e as condições de reposição do empréstimo ou do crédito do fiduciário;
>
> III - a taxa de juros e os encargos incidentes;
>
> IV - a cláusula de constituição da propriedade fiduciária, com a descrição do imóvel objeto da alienação fiduciária e a indicação do título e modo de aquisição;
>
> V - a cláusula que assegure ao fiduciante a livre utilização, por sua conta e risco, do imóvel objeto da alienação fiduciária, exceto a hipótese de inadimplência; (Redação dada pela Lei nº 14.711, de 2023)
>
> VI - a indicação, para efeito de venda em público leilão, do valor do imóvel e dos critérios para a respectiva revisão;
>
> VII - a cláusula que disponha sobre os procedimentos de que tratam os arts. 26-A, 27 e 27-A desta Lei. (Redação dada pela Lei nº 14.711, de 2023)
>
> **Parágrafo único.** Caso o valor do imóvel convencionado pelas partes nos termos do inciso VI do caput deste artigo seja inferior ao utilizado pelo órgão competente como base de cálculo para a apuração do imposto sobre transmissão inter vivos, exigível por força da consolidação da propriedade em nome do credor fiduciário, este último será o valor mínimo para efeito de venda do imóvel no primeiro leilão. (Incluído pela Lei nº 13.465, de 2017)

- ⭐ **O parágrafo único é a régua do 1º leilão:** se o valor convencionado (inciso VI) for **inferior à
  base de cálculo do ITBI**, prevalece a **base do ITBI** como mínimo do **primeiro** leilão. Item
  obrigatório da precificação — o piso pode ser **maior** do que o contrato diz.
- **Inciso VII (Lei 14.711/2023):** o contrato deve dispor sobre os **arts. 26-A, 27 e 27-A**. Contrato
  antigo que só menciona o art. 27 Lei 9.514 está **desatualizado em relação ao rito** — ponto de due diligence.
- **Incisos I e V** também ganharam redação nova em 2023.

### 🔴 TEXTO MORTO — NÃO CITAR (fica registrado para reconhecer, não para usar)

A página exibe, atribuídos **apenas à MP 1.162/2023**, um "§1º" (repetindo o parágrafo único) e um
"§2º" (IPTU e taxas condominiais). **Nenhum dos dois está em vigor como art. 24.** A regra do IPTU foi
promulgada pela lei de conversão **no art. 23, §2º** (§1 deste anexo).

> ~~"§ 2º Nos contratos firmados com cláusula de alienação fiduciária em garantia, caberá ao fiduciante
> a obrigação de arcar com o custo do pagamento do Imposto sobre a Propriedade Predial e Territorial
> Urbana - IPTU incidente sobre o bem e das taxas condominiais existentes."~~
> — **(Incluído pela Medida Provisória nº 1.162, de 2023) — SEM EFICÁCIA COMO ART. 24.**

- **Usa:** `base-legal-alienacao-fiduciaria` · `custo-total-real-e-precificacao` ·
  `analise-de-edital` · `validador-leiloes` (bloqueia a citação de "art. 24, §2º").

---

## 3. Constituição em mora e INTIMAÇÃO do fiduciante — art. 26 Lei 9.514 ✅ ⭐⭐ (o eixo da defesa)

> **Art. 26.** Vencida e não paga a dívida, no todo ou em parte, e constituídos em mora o devedor e, se for o caso, o terceiro fiduciante, será consolidada, nos termos deste artigo, a propriedade do imóvel em nome do fiduciário. (Redação dada pela Lei nº 14.711, de 2023)
>
> **§ 1º** Para fins do disposto neste artigo, o devedor e, se for o caso, o terceiro fiduciante serão intimados, a requerimento do fiduciário, pelo oficial do registro de imóveis competente, a satisfazer, no prazo de 15 (quinze) dias, a prestação vencida e aquelas que vencerem até a data do pagamento, os juros convencionais, as penalidades e os demais encargos contratuais, os encargos legais, inclusive os tributos, as contribuições condominiais imputáveis ao imóvel e as despesas de cobrança e de intimação. (Redação dada pela Lei nº 14.711, de 2023)
>
> **§ 1º-A** Na hipótese de haver imóveis localizados em mais de uma circunscrição imobiliária em garantia da mesma dívida, a intimação para purgação da mora poderá ser requerida a qualquer um dos registradores competentes e, uma vez realizada, importa em cumprimento do requisito de intimação em todos os procedimentos de excussão, desde que informe a totalidade da dívida e dos imóveis passíveis de consolidação de propriedade. (Incluído pela Lei nº 14.711, de 2023)
>
> **§ 2º** O contrato poderá estabelecer o prazo de carência, após o qual será expedida a intimação. (Redação dada pela Lei nº 14.711, de 2023)
>
> **§ 2º-A** Quando não for estabelecido o prazo de carência no contrato de que trata o § 2º deste artigo, este será de 15 (quinze) dias. (Incluído pela Lei nº 14.711, de 2023)
>
> **§ 3º** A intimação será feita pessoalmente ao devedor e, se for o caso, ao terceiro fiduciante, que por esse ato serão cientificados de que, se a mora não for purgada no prazo legal, a propriedade será consolidada no patrimônio do credor e o imóvel será levado a leilão nos termos dos arts. 26-A, 27 e 27-A desta Lei, conforme o caso, hipótese em que a intimação poderá ser promovida por solicitação do oficial do registro de imóveis, por oficial de registro de títulos e documentos da comarca da situação do imóvel ou do domicílio de quem deva recebê-la, ou pelo correio, com aviso de recebimento, situação em que se aplica, no que couber, o disposto no art. 160 da Lei nº 6.015, de 31 de dezembro de 1973 (Lei de Registros Públicos). (Redação dada pela Lei nº 14.711, de 2023)
>
> **§ 3o-A**. Quando, por duas vezes, o oficial de registro de imóveis ou de registro de títulos e documentos ou o serventuário por eles credenciado houver procurado o intimando em seu domicílio ou residência sem o encontrar, deverá, havendo suspeita motivada de ocultação, intimar qualquer pessoa da família ou, em sua falta, qualquer vizinho de que, no dia útil imediato, retornará ao imóvel, a fim de efetuar a intimação, na hora que designar, aplicando-se subsidiariamente o disposto nos arts. 252, 253 e 254 da Lei no 13.105, de 16 de março de 2015 (Código de Processo Civil). (Incluído pela Lei nº 13.465, de 2017)
>
> **§ 3o-B**. Nos condomínios edilícios ou outras espécies de conjuntos imobiliários com controle de acesso, a intimação de que trata o § 3o-A poderá ser feita ao funcionário da portaria responsável pelo recebimento de correspondência. (Incluído pela Lei nº 13.465, de 2017)
>
> **§ 4º** Quando o devedor ou, se for o caso, o terceiro fiduciante, o cessionário, o representante legal ou o procurador regularmente constituído encontrar-se em local ignorado, incerto ou inacessível, o fato será certificado pelo serventuário encarregado da diligência e informado ao oficial de registro de imóveis, que, à vista da certidão, promoverá a intimação por edital publicado pelo período mínimo de 3 (três) dias em jornal de maior circulação local ou em jornal de comarca de fácil acesso, se o local não dispuser de imprensa diária, contado o prazo para purgação da mora da data da última publicação do edital. (Redação dada pela Lei nº 14.711, de 2023)
>
> **§ 4º-A** É responsabilidade do devedor e, se for o caso, do terceiro fiduciante informar ao credor fiduciário sobre a alteração de seu domicílio. (Incluído pela Lei nº 14.711, de 2023)
>
> **§ 4º-B** Presume-se que o devedor e, se for o caso, o terceiro fiduciante encontram-se em lugar ignorado quando não forem encontrados no local do imóvel dado em garantia nem no endereço que tenham fornecido por último, observado que, na hipótese de o devedor ter fornecido contato eletrônico no contrato, é imprescindível o envio da intimação por essa via com, no mínimo, 15 (quinze) dias de antecedência da realização de intimação edilícia. (Incluído pela Lei nº 14.711, de 2023)
>
> **§ 4º-C** Para fins do disposto no § 4º deste artigo, considera-se lugar inacessível: (Incluído pela Lei nº 14.711, de 2023)
>
> I - aquele em que o funcionário responsável pelo recebimento de correspondência se recuse a atender a pessoa encarregada pela intimação; ou (Incluído pela Lei nº 14.711, de 2023)
>
> II - aquele em que não haja funcionário responsável pelo recebimento de correspondência para atender a pessoa encarregada pela intimação. (Incluído pela Lei nº 14.711, de 2023)
>
> **§ 5º** Purgada a mora no Registro de Imóveis, convalescerá o contrato de alienação fiduciária.
>
> **§ 6º** O oficial do Registro de Imóveis, nos três dias seguintes à purgação da mora, entregará ao fiduciário as importâncias recebidas, deduzidas as despesas de cobrança e de intimação.
>
> **§ 7º** Decorrido o prazo de que trata o § 1º sem a purgação da mora, o oficial do competente Registro de Imóveis, certificando esse fato, promoverá a averbação, na matrícula do imóvel, da consolidação da propriedade em nome do fiduciário, à vista da prova do pagamento por este, do imposto de transmissão inter vivos e, se for o caso, do laudêmio. (Redação dada pela Lei nº 10.931, de 2004)
>
> **§ 8o** O fiduciante pode, com a anuência do fiduciário, dar seu direito eventual ao imóvel em pagamento da dívida, dispensados os procedimentos previstos no art. 27. (Incluído pela Lei nº 10.931, de 2004)

🔴 **O §4º-B é a tese de nulidade mais forte que restou ao fiduciante.** Texto literal: havendo
**contato eletrônico no contrato**, é **"imprescindível"** o envio da intimação por essa via com **no
mínimo 15 dias de antecedência** da intimação por edital. Intimação editalícia feita sem esse envio,
em contrato que trazia e-mail, é **vício de procedimento** — e é a **única** matéria que o **art. 30,
§único** ressalva da trava "resolve-se em perdas e danos" (§8 deste anexo). **Combinação decisiva.**

⚠️ **O mesmo §4º-B também FECHA uma porta ao devedor:** quem sumiu do imóvel e do último endereço
informado é **presumidamente** "em lugar ignorado". Somado ao **§4º-A** (dever de informar mudança de
domicílio), a tese "não fui encontrado, logo houve nulidade" ficou **bem mais difícil** do que era.
Skill de defesa que ignorar isso vende ilusão.

**Marcos operacionais:** purga em **15 dias** (§1º) · carência supletiva de **15 dias** quando o
contrato silencia (§2º-A) · edital por **3 dias** em jornal (§4º) · purga devolvida ao fiduciário em
**3 dias** (§6º) · averbação da consolidação mediante prova de **ITBI e laudêmio** (§7º).

- **Usa:** `consolidacao-da-propriedade-e-intimacao` ⭐ · `defesa-fiduciante-consolidacao-e-purga` ⭐ ·
  `nulidades-de-intimacao-e-notificacao` ⭐ · `vicios-do-procedimento-extrajudicial` ·
  `risco-de-anulacao-do-certame` · `anulatoria-de-leilao-extrajudicial`.

---

## 4. Regime do IMÓVEL RESIDENCIAL do devedor — art. 26-A ✅ 🔴 ⭐⭐

> **Art. 26-A.** Os procedimentos de cobrança, purgação de mora, consolidação da propriedade fiduciária e leilão decorrentes de financiamentos para aquisição ou construção de imóvel residencial do devedor, exceto as operações do sistema de consórcio de que trata a Lei nº 11.795, de 8 de outubro de 2008, estão sujeitos às normas especiais estabelecidas neste artigo. (Redação dada pela Lei nº 14.711, de 2023)
>
> **§ 1o** A consolidação da propriedade em nome do credor fiduciário será averbada no registro de imóveis trinta dias após a expiração do prazo para purgação da mora de que trata o § 1o do art. 26 desta Lei. (Incluído pela Lei nº 13.465, de 2017)
>
> **§ 2º** Até a data da averbação da consolidação da propriedade fiduciária, é assegurado ao devedor e, se for o caso, ao terceiro fiduciante pagar as parcelas da dívida vencidas e as despesas de que trata o inciso II do § 3º do art. 27 desta Lei, hipótese em que convalescerá o contrato de alienação fiduciária. (Redação dada pela Lei nº 14.711, de 2023)
>
> **§ 3º** No segundo leilão, será aceito o maior lance oferecido desde que seja igual ou superior ao valor integral da dívida garantida pela alienação fiduciária mais antiga vigente sobre o bem, das despesas, inclusive emolumentos cartorários, dos prêmios de seguro, dos encargos legais, inclusive tributos, e das contribuições condominiais. (Incluído pela Lei nº 14.711, de 2023)
>
> **§ 4º** Se no segundo leilão não houver lance que atenda ao referencial mínimo para arrematação estabelecido no § 3º deste artigo, a dívida será considerada extinta, com recíproca quitação, hipótese em que o credor ficará investido da livre disponibilidade. (Incluído pela Lei nº 14.711, de 2023)
>
> **§ 5º** A extinção da dívida no excedente ao referencial mínimo para arrematação configura condição resolutiva inerente à dívida e, por isso, estende-se às hipóteses em que o credor tenha preferido o uso da via judicial para executar a dívida. (Incluído pela Lei nº 14.711, de 2023)

🔴 **Deixou de ser regra de MCMV/habitacional.** O caput alcança **todo financiamento para aquisição ou
construção de imóvel residencial do devedor**, exceto consórcio. **Identificar se o caso é art. 26-A é
a PRIMEIRA pergunta da triagem do extrajudicial** — muda purga, muda saldo, muda tudo.

| | Fora do art. 26-A | **Dentro do art. 26-A** |
|---|---|---|
| Purga da mora | Até o fim do prazo do art. 26, §1º Lei 9.514 | ⭐ **Até a AVERBAÇÃO da consolidação** (§2º), com os **30 dias** extras do §1º |
| O que se paga na purga | — | **"as parcelas da dívida vencidas"** — purga da mora, **não** antecipação do saldo |
| 2º leilão negativo | Devedor **continua obrigado** pelo saldo (art. 27, §5º-A Lei 9.514) | ⭐ **Dívida EXTINTA, com recíproca quitação** (§4º) |
| Alcance da extinção | — | 🔴 **§5º: "condição resolutiva inerente à dívida"**, que **se estende à via JUDICIAL** |

🔴 **O §5º é peça de defesa poderosa e pouco conhecida:** o credor **não escapa** do efeito extintivo
migrando para a execução judicial. Ler junto com o art. 27, §5º-A Lei 9.514, que **ressalva expressamente** o
art. 26-A, §4º.

⚠️ **Diferença de referencial:** o mínimo do 2º leilão aqui (§3º) é calculado sobre a **alienação
fiduciária MAIS ANTIGA** vigente sobre o bem — não sobre a dívida do exequente da vez.

- **Usa:** `regime-do-imovel-residencial-26a` ⭐ · `triagem-leiloes` ⭐ ·
  `defesa-fiduciante-consolidacao-e-purga` · `saldo-remanescente-e-quitacao` ⭐ ·
  `os-dois-leiloes-da-alienacao-fiduciaria`.

---

## 5. OS DOIS LEILÕES — art. 27 Lei 9.514 ✅ ⭐⭐ (o núcleo do extrajudicial)

> **Art. 27.** Consolidada a propriedade em seu nome, o fiduciário promoverá leilão público para a alienação do imóvel, no prazo de 60 (sessenta) dias, contado da data do registro de que trata o § 7º do art. 26 desta Lei. (Redação dada pela Lei nº 14.711, de 2023)
>
> **§ 1o** Se no primeiro leilão público o maior lance oferecido for inferior ao valor do imóvel, estipulado na forma do inciso VI e do parágrafo único do art. 24 desta Lei, será realizado o segundo leilão nos quinze dias seguintes. (Redação dada pela Lei nº 13.465, de 2017)
>
> **§ 2º** No segundo leilão, será aceito o maior lance oferecido, desde que seja igual ou superior ao valor integral da dívida garantida pela alienação fiduciária, das despesas, inclusive emolumentos cartorários, dos prêmios de seguro, dos encargos legais, inclusive tributos, e das contribuições condominiais, podendo, caso não haja lance que alcance referido valor, ser aceito pelo credor fiduciário, a seu exclusivo critério, lance que corresponda a, pelo menos, metade do valor de avaliação do bem. (Redação dada pela Lei nº 14.711, de 2023)
>
> **§ 2º-A** Para fins do disposto nos §§ 1º e 2º deste artigo, as datas, os horários e os locais dos leilões serão comunicados ao devedor e, se for o caso, ao terceiro fiduciante, por meio de correspondência dirigida aos endereços constantes do contrato, inclusive ao endereço eletrônico. (Redação dada pela Lei nº 14.711, de 2023)
>
> **§ 2º-B** Após a averbação da consolidação da propriedade fiduciária no patrimônio do credor fiduciário e até a data da realização do segundo leilão, é assegurado ao fiduciante o direito de preferência para adquirir o imóvel por preço correspondente ao valor da dívida, somado às despesas, aos prêmios de seguro, aos encargos legais, às contribuições condominiais, aos tributos, inclusive os valores correspondentes ao imposto sobre transmissão inter vivos e ao laudêmio, se for o caso, pagos para efeito de consolidação da propriedade fiduciária no patrimônio do credor fiduciário, e às despesas inerentes aos procedimentos de cobrança e leilão, hipótese em que incumbirá também ao fiduciante o pagamento dos encargos tributários e das despesas exigíveis para a nova aquisição do imóvel, inclusive das custas e dos emolumentos. (Redação dada pela Lei nº 14.711, de 2023)
>
> **§ 3º** Para os fins do disposto neste artigo, entende-se por:
>
> I - dívida: o saldo devedor da operação de alienação fiduciária, na data do leilão, nele incluídos os juros convencionais, as penalidades e os demais encargos contratuais;
>
> II - despesas: a soma das importâncias correspondentes aos encargos e às custas de intimação e daquelas necessárias à realização do leilão público, compreendidas as relativas aos anúncios e à comissão do leiloeiro; e (Redação dada pela Lei nº 14.711, de 2023)
>
> III - encargos do imóvel: os prêmios de seguro e os encargos legais, inclusive tributos e contribuições condominiais. (Incluído pela Lei nº 14.711, de 2023)
>
> **§ 4º** Nos 5 (cinco) dias que se seguirem à venda do imóvel no leilão, o credor entregará ao fiduciante a importância que sobejar, nela compreendido o valor da indenização de benfeitorias, depois de deduzidos os valores da dívida, das despesas e dos encargos de que trata o § 3º deste artigo, o que importará em recíproca quitação, hipótese em que não se aplica o disposto na parte final do art. 516 da Lei nº 10.406, de 10 de janeiro de 2002 (Código Civil). (Redação dada pela Lei nº 14.711, de 2023)
>
> **§ 5º** Se no segundo leilão não houver lance que atenda ao referencial mínimo para arrematação estabelecido no § 2º, o fiduciário ficará investido na livre disponibilidade do imóvel e exonerado da obrigação de que trata o § 4º deste artigo. (Redação dada pela Lei nº 14.711, de 2023)
>
> **§ 5º-A** Se o produto do leilão não for suficiente para o pagamento integral do montante da dívida, das despesas e dos encargos de que trata o § 3º deste artigo, o devedor continuará obrigado pelo pagamento do saldo remanescente, que poderá ser cobrado por meio de ação de execução e, se for o caso, excussão das demais garantias da dívida, ressalvada a hipótese de extinção do saldo devedor remanescente prevista no § 4º do art. 26-A desta Lei. (Incluído pela Lei nº 14.711, de 2023)
>
> **§ 6º** (Revogado). (Redação dada pela Lei nº 14.711, de 2023)
>
> **§ 6º-A** Na hipótese de que trata o § 5º, para efeito de cálculo do saldo remanescente de que trata o § 5º-A, será deduzido o valor correspondente ao referencial mínimo para arrematação do valor atualizado da dívida, conforme estabelecido no § 2º deste artigo, incluídos os encargos e as despesas de cobrança. (Incluído pela Lei nº 14.711, de 2023)
>
> **§ 7º** Se o imóvel estiver locado, a locação poderá ser denunciada com o prazo de trinta dias para desocupação, salvo se tiver havido aquiescência por escrito do fiduciário, devendo a denúncia ser realizada no prazo de noventa dias a contar da data da consolidação da propriedade no fiduciário, devendo essa condição constar expressamente em cláusula contratual específica, destacando-se das demais por sua apresentação gráfica. (Incluído pela Lei nº 10.931, de 2004)
>
> **§ 8º** Responde o fiduciante pelo pagamento dos impostos, taxas, contribuições condominiais e quaisquer outros encargos que recaiam ou venham a recair sobre o imóvel, cuja posse tenha sido transferida para o fiduciário, nos termos deste artigo, até a data em que o fiduciário vier a ser imitido na posse. (Incluído pela Lei nº 10.931, de 2004)
>
> **§ 9º** O disposto no § 2º-B deste artigo aplica-se à consolidação da propriedade fiduciária de imóveis do FAR, na forma prevista na Lei no 11.977, de 7 de julho de 2009. (Incluído pela Lei nº 13.465, de 2017)
>
> **§ 10 **Os leilões e a publicação dos respectivos editais poderão ser realizados por meio eletrônico. (Incluído pela Lei nº 14.620, de 2023)
>
> **§ 11**. Os direitos reais de garantia ou constrições, inclusive penhoras, arrestos, bloqueios e indisponibilidades de qualquer natureza, incidentes sobre o direito real de aquisição do fiduciante não obstam a consolidação da propriedade no patrimônio do credor fiduciário e a venda do imóvel para realização da garantia. (Incluído pela Lei nº 14.711, de 2023)
>
> **§ 12**. Na hipótese prevista no § 11 deste artigo, os titulares dos direitos reais de garantia ou constrições sub-rogam-se no direito do fiduciante à percepção do saldo que eventualmente restar do produto da venda. (Incluído pela Lei nº 14.711, de 2023)

### 5.1 🔴 Purga × preferência — a distinção que o mercado erra e que virou tese repetitiva

Depois da **averbação da consolidação** (fora do art. 26-A), o fiduciante **não purga mais a mora**. O
que lhe resta é o **direito de preferência do §2º-B** — coisa diferente e **muito mais cara**:

| | **Purga da mora** | **Preferência (§2º-B)** |
|---|---|---|
| Quando | Até o fim do prazo do art. 26, §1º Lei 9.514 (no 26-A, até a averbação) | **Após** a averbação e **até** o 2º leilão |
| Quanto se paga | As **prestações vencidas** + encargos | **Toda a dívida** + despesas + seguros + encargos + tributos + **ITBI e laudêmio já pagos pelo credor** + despesas de cobrança e leilão |
| Efeito | O contrato **convalesce** — volta a ser financiamento | **Nova aquisição** — ainda paga tributos e emolumentos da nova transmissão |

⭐ **Chamar o §2º-B de "purga tardia" é erro material com impacto direto no cálculo.** E a distinção
**deixou de ser doutrina**: é o **Tema 1.288/STJ** ("resta ao fiduciante **tão somente** o direito de
preferência"). Ver `context/jurisprudencia-leiloes.md`, inclusive a ressalva de que o Tema é
**precedente vivo sobre texto morto** (versava o art. 39, II, hoje revogado).

### 5.2 As quatro mudanças de 2023 que invertem conselhos antigos

1. 🔴 **Prazo do leilão: 30 → 60 dias** (caput). A "primeira ocorrência" na página ainda diz trinta.
2. 🔴 **No 2º leilão o credor PODE aceitar 50% da avaliação** (§2º) — **"a seu exclusivo critério"**. É
   **faculdade do credor**, **jamais direito do arrematante**. Aumenta o volume de bens efetivamente
   arrematados e abre janela de negociação com o credor.
3. 🔴🔴 **Leilão negativo deixou de quitar a dívida como regra** (§5º-A): fora do art. 26-A, o devedor
   **continua obrigado pelo saldo remanescente**, cobrável por **execução** e com **excussão das demais
   garantias**. Inversão frontal da regra anterior. O **§6º** (termo de quitação em 5 dias) foi
   **REVOGADO**, coerentemente. Cálculo do saldo: **§6º-A**.
4. 🔴 **Penhora não trava mais o leilão** (§11): penhoras, arrestos, bloqueios e indisponibilidades
   **sobre o direito real de aquisição do fiduciante** **não obstam** consolidação nem venda; os
   titulares **sub-rogam-se no saldo** (§12). ⚠️ **Limite literal:** o §11 fala do direito **do
   fiduciante**. Constrição sobre a **propriedade**, ou originada de outra relação, **não está coberta**
   pela literalidade — e constrição averbada **antes** da AF é lacuna real (🟡).

### 5.3 Detalhes que entram na conta

- **§3º, II — a comissão do leiloeiro é DESPESA dedutível** no extrajudicial (entra no mínimo do 2º
  leilão e no que sobra ao devedor). **Regime oposto ao judicial**, onde a comissão é paga **pelo
  arrematante por fora** (CPC 901, §1º). **Não transportar um regime para o outro.**
- **§4º — sobra devolvida em 5 dias** (no rito hipotecário da 14.711 são **15**; não confundir).
- **§7º — locação:** denúncia com **30 dias** para desocupação, **desde que** a denúncia ocorra em
  **90 dias** da consolidação **e** o contrato tenha cláusula específica com **destaque gráfico**.
- **§8º — encargos do fiduciante até a IMISSÃO** do fiduciário na posse.
- **§9º** estende o §2º-B às consolidações de imóveis do **FAR**.
- **§10 — leilões e editais podem ser eletrônicos** (Lei 14.620/2023).

- **Usa:** `os-dois-leiloes-da-alienacao-fiduciaria` ⭐⭐ · `saldo-remanescente-e-quitacao` ⭐ ·
  `leitura-de-matricula` ⭐ (o §11 muda a leitura) · `preco-vil-como-tese` ·
  `defesa-fiduciante-consolidacao-e-purga` · `custo-total-real-e-precificacao`.

---

## 6. Excussão de VÁRIOS imóveis — art. 27-A ✅ 🔴 (artigo inteiramente novo)

> **Art. 27-A.** Nas operações de crédito garantidas por alienação fiduciária de 2 (dois) ou mais imóveis, na hipótese de não ser convencionada a vinculação de cada imóvel a 1 (uma) parcela da dívida, o credor poderá promover a excussão em ato simultâneo, por meio de consolidação da propriedade e leilão de todos os imóveis em conjunto, ou em atos sucessivos, por meio de consolidação e leilão de cada imóvel em sequência, à medida do necessário para satisfação integral do crédito. (Incluído pela Lei nº 14.711, de 2023)
>
> **§ 1º** Na hipótese de excussão em atos sucessivos, caberá ao credor fiduciário a indicação dos imóveis a serem excutidos em sequência, exceto se houver disposição em sentido contrário expressa no contrato, situação em que a consolidação da propriedade dos demais ficará suspensa. (Incluído pela Lei nº 14.711, de 2023)
>
> **§ 2º** A cada leilão, o credor fiduciário promoverá nas matrículas dos imóveis não leiloados a averbação do demonstrativo do resultado e o encaminhará ao devedor e, se for o caso, aos terceiros fiduciantes, por meio de correspondência dirigida aos endereços físico e eletrônico informados no contrato. (Incluído pela Lei nº 14.711, de 2023)
>
> **§ 3º** Na hipótese de não se alcançar a quantia suficiente para satisfação do crédito, a cada leilão realizado, o credor recolherá o imposto sobre transmissão inter vivos e, se for o caso, o laudêmio, relativos ao imóvel a ser excutido em seguida, requererá a averbação da consolidação da propriedade e, no prazo de 30 (trinta) dias, realizará os procedimentos de leilão nos termos do art. 27 desta Lei. (Incluído pela Lei nº 14.711, de 2023)
>
> **§ 4º** Satisfeito integralmente o crédito com o produto dos leilões realizados sucessivamente, o credor fiduciário entregará ao devedor e, se for o caso, aos terceiros fiduciantes, o termo de quitação e a autorização de cancelamento do registro da propriedade fiduciária de eventuais imóveis que restem a ser desonerados. (Incluído pela Lei nº 14.711, de 2023)

- ⭐ **Alavanca contratual real para quem redige do lado do devedor (§1º):** o credor escolhe a ordem
  dos imóveis **"exceto se houver disposição em sentido contrário expressa no contrato"** — e, havendo,
  a consolidação dos demais **fica suspensa**. Cláusula barata de negociar e cara de esquecer.
- ⚠️ **Prazo diferente no §3º:** na excussão **sucessiva**, o leilão do imóvel seguinte é em **30 dias**
  (não 60). Divergência interna da lei, a ser respeitada como está.
- **Usa:** `excussao-multipla-e-concurso-de-credores` ⭐ · `defesa-fiduciante-consolidacao-e-purga` ·
  `leitura-de-matricula`.

---

## 7. Cessão e transmissão — arts. 28 e 29 ✅

> **Art. 28.** A cessão do crédito objeto da alienação fiduciária implicará a transferência, ao cessionário, de todos os direitos e obrigações inerentes à propriedade fiduciária em garantia.

> **Art. 29 (Lei 9.514).** O fiduciante, com anuência expressa do fiduciário, poderá transmitir os direitos de que seja titular sobre o imóvel objeto da alienação fiduciária em garantia, assumindo o adquirente as respectivas obrigações.

---

## 8. REINTEGRAÇÃO DE POSSE — art. 30 ✅ ⭐⭐ (e a trava que comprimiu a defesa)

> **Art. 30.** É assegurada ao fiduciário, ao seu cessionário ou aos seus sucessores, inclusive ao adquirente do imóvel por força do leilão público de que tratam os arts. 26-A, 27 e 27-A, a reintegração na posse do imóvel, que será concedida liminarmente, para desocupação no prazo de 60 (sessenta) dias, desde que comprovada a consolidação da propriedade em seu nome, na forma prevista no art. 26 desta Lei. (Redação dada pela Lei nº 14.711, de 2023)
>
> **Parágrafo único.** Arrematado o imóvel ou consolidada definitivamente a propriedade no caso de frustração dos leilões, as ações judiciais que tenham por objeto controvérsias sobre as estipulações contratuais ou os requisitos procedimentais de cobrança e leilão, excetuada a exigência de notificação do devedor e, se for o caso, do terceiro fiduciante, não obstarão a reintegração de posse de que trata este artigo e serão resolvidas em perdas e danos. (Redação dada pela Lei nº 14.711, de 2023)

⭐ **Para o ARREMATANTE, este é o artigo que torna o extrajudicial operacionalmente melhor que o
judicial:** a reintegração é **liminar por lei**, com **60 dias** para desocupação, e é assegurada
**expressamente ao adquirente em leilão**. No judicial, o CPC 901, §1º **não tem prazo nem qualificação
liminar**, e o mandado só sai depois de pagos preço, comissão, despesas e **ITBI**.

🔴 **A ampliação do parágrafo único é enorme e passa despercebida.** Na redação anterior (Lei
13.465/2017) a trava valia **apenas** para financiamento imobiliário/MCMV/FAR. A **Lei 14.711/2023
tirou o recorte**: hoje vale para **qualquer** caso em que o imóvel tenha sido arrematado ou a
propriedade definitivamente consolidada. Material que diga *"a trava só vale no financiamento
habitacional"* está **desatualizado**.

⭐⭐ **A defesa do fiduciante foi comprimida a UM EIXO.** A **única** matéria que ainda obsta a
reintegração é a **exigência de notificação** do devedor / terceiro fiduciante. Cláusulas, avaliação,
publicidade, valor do lance — **tudo vira perdas e danos**. Estratégia do executado:
**atacar a intimação, não o preço** (e é aí que entram os §§4º-B e 4º-C do art. 26 Lei 9.514).

- **Usa:** `imissao-na-posse-do-arrematante` ⭐ · `defesa-contra-imissao-e-embargos-de-terceiro` ·
  `vicios-do-procedimento-extrajudicial` ⭐ · `anulatoria-de-leilao-extrajudicial` ·
  `nulidades-de-intimacao-e-notificacao` · `reparacao-por-leilao-irregular`.

---

## 9. Sub-rogação, insolvência e regime supletivo — arts. 31 a 33 ✅

> **Art. 31.** O fiador ou terceiro interessado que pagar a dívida ficará sub-rogado, de pleno direito, no crédito e na propriedade fiduciária.
>
> **Parágrafo único.** Nos casos de transferência de financiamento para outra instituição financeira, o pagamento da dívida à instituição credora original poderá ser feito, a favor do mutuário, pela nova instituição credora. (Incluído pela Lei nº 12.810, de 2013)

> **Art. 32.** Na hipótese de insolvência do fiduciante, fica assegurada ao fiduciário a restituição do imóvel alienado fiduciariamente, na forma da legislação pertinente.

> **Art. 33.** Aplicam-se à propriedade fiduciária, no que couber, as disposições dos arts. 647 e 648 do Código Civil.

> **Fora de escopo (ponteiro):** os **arts. 33-A a 33-F** tratam de **portabilidade de crédito
> imobiliário** (transferência da dívida entre credores) — **não** de leilão. Não transcritos aqui.

---

## 10. TAXA DE OCUPAÇÃO — art. 37-A ✅ ⭐ (o crédito que o arrematante esquece que tem)

> **Art. 37-A.** O fiduciante pagará ao credor fiduciário ou ao seu sucessor, a título de taxa de ocupação do imóvel, por mês ou fração, valor correspondente a 1% (um por cento) do valor de que trata o inciso VI do caput ou o parágrafo único do art. 24 desta Lei, computado e exigível desde a data da consolidação da propriedade fiduciária no patrimônio do credor fiduciário até a data em que este ou seu sucessor vier a ser imitido na posse do imóvel. (Redação dada pela Lei nº 14.711, de 2023)
>
> **Parágrafo único.** O disposto no caput deste artigo aplica-se às operações do Programa Minha Casa, Minha Vida, instituído pela Lei nº 11.977, de 7 de julho de 2009, com recursos advindos da integralização de cotas no Fundo de Arrendamento Residencial (FAR). (Incluído pela Lei nº 13.465, de 2017)

- ⭐ **1% ao mês, contado da CONSOLIDAÇÃO** (não da alienação em leilão, não da imissão) **até a
  imissão na posse**, sobre o valor do art. 24, VI (ou do parágrafo único, se maior).
- 🔴 **A pegadinha das quatro redações:** este artigo teve **4 versões**. Quem cita *"desde a data da
  alienação em leilão"* está **duas gerações atrás** (redação da MP 2.223/2001).
- ⭐ **Vira CRÉDITO do arrematante, não custo:** o texto diz "ao credor fiduciário **ou ao seu
  sucessor**". O arrematante é sucessor — logo a taxa de ocupação do período é **obrigação do
  fiduciante em favor dele**. 🟡 **Ressalva obrigatória:** a **legitimidade do arrematante terceiro**
  para cobrá-la **não foi pesquisada** em jurisprudência (item 🟡 do BUILD-CONTRACT). Afirmar o
  direito, marcar *"conferir o inteiro teor antes de protocolar"* e rotear ao `validador-leiloes`.
- **Usa:** `debitos-e-creditos-pos-arrematacao` ⭐ · `imissao-na-posse-do-arrematante` ·
  `custo-total-real-e-precificacao` · `desocupacao-locacao-e-ocupantes`.

---

## 11. Locação ineficaz e editais eletrônicos — arts. 37-B e 37-C Lei 9.514 ✅

> **Art. 37-B.** Será considerada ineficaz, e sem qualquer efeito perante o fiduciário ou seus sucessores, a contratação ou a prorrogação de locação de imóvel alienado fiduciariamente por prazo superior a um ano sem concordância por escrito do fiduciário. (Incluído pela Lei nº 10.931, de 2004)

> **Art. 37-C.** Os editais previstos nesta Lei poderão ser publicados de forma eletrônica. (Incluído pela Lei nº 14.620, de 2023)

- ⭐ **Due diligence:** locação de **até um ano** **não** é atingida pelo art. 37-B Lei 9.514. Acima de um ano
  **sem anuência escrita** do fiduciário, a ineficácia vale perante ele **e seus sucessores** — o que
  inclui o arrematante. ⚠️ **Mas ineficácia se DECLARA, não se executa sozinha:** ainda é preciso agir.
- ⚠️ **Cruzar com a armadilha dos 90 dias** do art. 8º da Lei 8.245 (denúncia da locação) e com o
  art. 27, §7º Lei 9.514 (30/90 dias). Ver `context/metodologia-leiloes.md`.
- **Usa:** `situacao-possessoria` ⭐ · `desocupacao-locacao-e-ocupantes` ⭐ ·
  `defesa-contra-imissao-e-embargos-de-terceiro`.

---

## 12. Revogações e o que restou do art. 39 ✅ 🔴

> **Art. 39.** As disposições da Lei nº 4.380, de 21 de agosto de 1964, e as demais disposições legais referentes ao Sistema Financeiro da Habitação não se aplicam às operações de crédito compreendidas no sistema de financiamento imobiliário a que se refere esta Lei. (Redação dada pela Lei nº 14.711, de 2023)
>
> I - (revogado); (Redação dada pela Lei nº 14.711, de 2023)
>
> II - (revogado). (Redação dada pela Lei nº 14.711, de 2023)

🔴 **O art. 39, II era o dispositivo que mandava aplicar os arts. 29 a 41 do DL 70/66** à execução de
créditos garantidos por hipoteca. **Revogado** pela Lei 14.711/2023 (art. 18, V, "b"). Hoje os dois
incisos aparecem como **"(revogado)"** e o caput tem redação nova e enxuta.

**Revogações expressas da Lei 14.711/2023 na Lei 9.514 (art. 18, V):** `a)` **§6º do art. 27**;
`b)` **incisos I e II do art. 39**. Ver `context/lei-14711-2023.md`.

⚠️ **Precedente vivo sobre texto morto:** o **Tema 1.288/STJ** versava justamente o **art. 39, II**.
O Tema **vale** (resolve o intertemporal), mas **não serve** para sustentar que o art. 39, II está em
vigor. Ver `context/jurisprudencia-leiloes.md`.

---

## 13. Tabela-resumo: o que mudou em 31/10/2023 🔴

| Ponto | Antes (até 30/10/2023) | **Vigente** | Âncora |
|---|---|---|---|
| Prazo para levar a leilão | **30 dias** da consolidação | **60 dias** | art. 27, caput Lei 9.514 |
| 2º leilão sem lance que cubra a dívida | Dívida **extinta** (regra geral) | Credor **pode aceitar**, a seu exclusivo critério, **≥ 50% da avaliação** | art. 27, §2º Lei 9.514 |
| Saldo após leilão insuficiente | Extinto | **Devedor continua obrigado**, cobrável por execução | art. 27, §5º-A Lei 9.514 |
| Exceção ao saldo | — | Imóvel **residencial do devedor**: dívida extinta, e a extinção **alcança a via judicial** | art. 26-A, §§4º-5º |
| Penhora sobre o direito do fiduciante | Fonte de litígio | **Não obsta** consolidação nem venda; sub-rogação no **saldo** | art. 27, §§11-12 Lei 9.514 |
| Vários imóveis na mesma dívida | Sem disciplina | Excussão **simultânea ou sucessiva** | art. 27-A |
| Ações do devedor × reintegração | Trava só no financiamento imobiliário/FAR | **Regra geral**; só a **notificação** obsta | art. 30, §único |
| Alcance do art. 26-A | MCMV / habitacional | **Todo financiamento de imóvel residencial do devedor** (exceto consórcio) | art. 26-A, caput |
| Intimação eletrônica | Inexistente | **Imprescindível**, 15 dias antes do edital | art. 26, §4º-B Lei 9.514 |
| IPTU/condomínio do fiduciante | Sem previsão expressa | ✅ **art. 23, §2º** (Lei 14.620/2023) — **não** art. 24, §2º | art. 23, §2º |
| Termo de quitação em 5 dias (2º leilão negativo) | Existia | **§6º REVOGADO** | art. 18, V, "a" da 14.711 |

---

## GUARD — o que este anexo proíbe

1. Citar **art. 27, caput Lei 9.514, com "trinta dias"** — o prazo vigente é **60 dias**.
2. Citar **art. 37-A com "desde a data da alienação em leilão"** — o termo inicial é a **CONSOLIDAÇÃO**.
3. Citar **"art. 24, §2º"** para IPTU/condomínio — **sem eficácia**. A regra vive no **art. 23, §2º**.
4. Dizer que **"a MP 1.162/2023 não foi convertida"** — **foi**, na **Lei 14.620/2023**. O que não
   vingou foi o **endereço** do dispositivo.
5. Dizer que **"não existe dispositivo pondo IPTU e condomínio no fiduciante"** — **existe** (art. 23,
   §2º). E também **não** usar o art. 23, §2º como se resolvesse a dívida do **arrematante**.
6. Dizer que **"leilão negativo sempre quita a dívida"** — fora do art. 26-A, o **§5º-A** mantém o
   devedor obrigado.
7. Tratar o **"50% no 2º leilão"** como **direito do arrematante** — é **faculdade do credor**, "a seu
   exclusivo critério".
8. Chamar o **§2º-B de "purga tardia"** — é **preferência**, com custo integral (Tema 1.288: "tão
   somente").
9. Afirmar que a trava do **art. 30, §único** só vale no **financiamento habitacional** — a 14.711
   **generalizou**.
10. Transportar a **comissão como despesa dedutível** (§3º, II) para o **judicial**, onde ela é paga
    **pelo arrematante por fora** (CPC 901, §1º) — e vice-versa.
11. Estender o **§11** a constrição sobre a **propriedade** ou de outra relação — a literalidade fala do
    direito **do fiduciante**.

Toda peça fecha por **`suprema-corte-leiloes`** (R1-R4) **+ `validador-leiloes`**.

---

## Fonte e verificação

- **Lei 9.514/1997 — texto compilado:** `https://www.planalto.gov.br/ccivil_03/leis/l9514.htm`
  (captura 2026-08-02). Seleção da **redação vigente** por script; superadas descartadas.
- **MP 1.162/2023 — status:** *"Convertida na Lei nº 14.620, de 2023"*
  (`https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2023/mpv/mpv1162.htm`).
- **Lei 14.620/2023, art. 28** — promulgou o IPTU/condomínio no **art. 23, §2º** da Lei 9.514
  (`https://www.planalto.gov.br/ccivil_03/_ato2023-2026/2023/lei/l14620.htm`).
- **Anexos irmãos:** `context/lei-14711-2023.md` (rito hipotecário novo + revogações) ·
  `context/cpc-leilao-879-903.md` (o regime judicial, que **não** se mistura com este) ·
  `context/jurisprudencia-leiloes.md` · `context/custo-total-do-arrematante.md`.
