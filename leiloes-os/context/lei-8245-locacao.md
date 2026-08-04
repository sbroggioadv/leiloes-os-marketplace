# Anexo — Lei 8.245/91 (Locações) na parte que o leilão toca

> **Anexo de legislação do `leiloes-os`.** Responde a **uma pergunta que o corpus não sabia responder**:
> quando o imóvel arrematado vem **com inquilino dentro**, quanto tempo o arrematante tem, **contado
> de quê**, e o que acontece se perder o prazo. Cobre o **art. 8º** (denúncia por alienação), a
> **preferência do locatário** (arts. 27-34 Lei 8.245), as **benfeitorias** (arts. 35-36), a **via** (art. 5º) e
> os **prazos de desocupação** (arts. 59, 63, 64, 46, 47, 57, 51, 74 Lei 8.245).
>
> **Fonte:** texto **compilado** da **Lei 8.245/1991** capturado do Planalto em **2026-08-02** —
> `https://www.planalto.gov.br/ccivil_03/leis/l8245.htm`. Transcrição **verbatim**, conferida por
> script (33 asserções, 0 falha — ver §14).
>
> **Marco temporal:** ⭐ a última alteração da Lei 8.245 é de **2012** (Lei 12.744). **Nenhuma lei
> 13.x, 14.x ou 15.x tocou esta lei** — conferido por varredura de todas as notas de alteração da
> página (§14). Aqui **não há surpresa pós-cutoff**: o art. 8º está na **redação original de 1991**.
>
> **Legenda:** ✅ vigente conferido · 🟡 não confirmado · 🔴 verdade dura / correção · ⭐ eixo.

---

## ⚠️ AVISO 1 — grep o artigo e leia a faixa. NUNCA despeje o anexo inteiro

Consulta pontual. **`grep` do número do artigo e leia só a faixa.** Quem precisa só do prazo tem a
tabela-resumo no §13; quem vai escrever peça lê a faixa do dispositivo.

## ⚠️ AVISO 2 — 🔴 PEGADINHA DE PLANALTO **TRAVADA** (e a única normalização feita)

A página compilada exibe **redação revogada ao lado da vigente**, como nas irmãs. Nesta lei a
incidência é **baixa e concentrada** — mas as duas que existem estão exatamente onde o arrematante
calcula prazo e custo. Descartadas nesta captura:

| Artigo | O que a página exibe a mais | Redação **vigente** |
|---|---|---|
| **art. 63** | a redação **original de 1991** ("o juiz fixará prazo de trinta dias") | **Lei 12.112/2009** — "determinará a **expedição de mandado de despejo**, que conterá o prazo de **30 dias**" |
| **art. 64** | a original: caução de **12 a 18 meses** | **Lei 12.112/2009** — caução de **6 a 12 meses** |
| **art. 32, §único** | **duas** exibições do **mesmo texto** (MP 2.223/2001 e Lei 10.931/2004) | citar pela **Lei 10.931/2004** (lei de conversão) |
| **arts. 4º, 12, 40 II, 53, 62** | redações antigas ao lado | fora do escopo deste anexo — não transcritas |

🔴 **A pegadinha do art. 32, §único é do tipo que já mordeu três vezes neste build.** O texto
normativo das duas exibições é **byte a byte idêntico** (conferido: a mesma frase aparece **2 vezes**
no arquivo) — muda **só a atribuição**. Diferente da Lei 9.514, aqui **a MP 2.223/2001 foi
efetivamente convertida** e o dispositivo **saiu no mesmo endereço**: não houve mudança de artigo.
**Cite "art. 32, parágrafo único (Lei 10.931/2004)"** e ignore a linha da MP.

🔴 **O art. 8º NÃO tem redação dupla.** Caput, §1º e §2º aparecem **uma única vez**, sem nota de
alteração — é a redação **originária de 1991**, nunca emendada. Quem "não achou a versão nova" não
achou porque **não existe**.

### Normalização declarada (2 artefatos de PÁGINA, nenhuma palavra alterada)

A página é um HTML de 1991 e carrega dois artefatos tipográficos que **não são da lei**. Este anexo os
normaliza, e declara:

1. **NBSP** (`U+00A0`) no lugar de espaço comum — **46 ocorrências**. Normalizado para espaço.
2. **Hífen enclítico marcado como `<i>-</i>` na fonte**, que renderiza `presumindo - se`. Normalizado
   para `presumindo-se`, `entende-se`, `conceder-se-á` etc.

⚠️ **Por que isso importa na prática:** quem copiar da página crua e colar em peça escreve
*"presumindo - se"*; e quem der `grep "Art. 63. Julgada" (Lei 8.245)` no texto cru **não acha nada**, porque entre
`63.` e `Julgada` há um NBSP. Nenhuma palavra, número ou pontuação foi alterada — só os dois
artefatos acima. A conferência do §14 roda sobre o texto normalizado, que é **exatamente** o
transcrito aqui.

## ⚠️ AVISO 3 — 🔴🔴 A CORREÇÃO CENTRAL DESTE ANEXO: **o marco dos 90 dias**

O corpus afirmava — e três anexos ainda afirmam — que o arrematante tem **"90 dias contados da
alienação"** para denunciar a locação. **A lei não diz isso em lugar nenhum.** Conferido por prova
positiva e negativa (§14): a expressão *"contados da alienação"* **não existe** no texto da Lei 8.245.

O que existe são **dois prazos de 90 dias diferentes, no mesmo artigo**, que o corpus fundiu em um só:

| | **Prazo para DENUNCIAR** | **Prazo para DESOCUPAR** |
|---|---|---|
| Onde está | **art. 8º, §2º** | **art. 8º, caput** |
| Quanto | 90 dias | 90 dias |
| **Contado de** | ⭐ **do REGISTRO da venda ou do compromisso** | da **denúncia** (é o prazo dado ao locatário para sair) |
| Quem observa | o **adquirente** (sob pena de preclusão) | o **locatário** |
| Se estourar | **presume-se a concordância** com a manutenção da locação | o adquirente ajuíza **despejo** (art. 5º) |

🔴 **Consequência de produto — é a classe de erro mais cara do domínio.** Dizer ao arrematante que o
relógio começou **na alienação** (arrematação, auto, carta) faz o plugin **declarar morto um prazo que
ainda corre**, porque o **registro é sempre posterior** ao ato de alienação. Pior: o marco é
**registral**, e **quem controla a data do registro é o próprio arrematante**. Na leitura literal, o
arrematante não só tem mais tempo do que o corpus dizia — ele **decide quando o relógio começa**.

⭐ **E há um segundo erro embutido:** ao fundir os dois prazos, o corpus fazia o arrematante planejar
**90 dias** até o imóvel vazio. O horizonte literal do art. 8º é **90 + 90 = até 180 dias** contados
do registro — e isso **antes** de qualquer ação de despejo, se o locatário não sair.

**Skills afetadas** (todas as que escrevem o marco): `suprema-corte-leiloes` (R3) ·
`anti-alucinacao-leiloes` (verdade 20) · `memoria-de-caso-leilao` (tabela de marcos) ·
`base-legal-alienacao-fiduciaria` · `triagem-leiloes` · e, quando forem construídas,
`situacao-possessoria`, `desocupacao-locacao-e-ocupantes` e `defesa-contra-imissao-e-embargos-de-terceiro`.

🔴 **Anexos que ainda carregam a asserção errada** (medido em 02/08, 3 arquivos / **5 sites**) —
corrigir antes do publish: `context/clausulas-armadilha-de-edital.md` (1) ·
`context/custo-total-do-arrematante.md` (1) · `context/metodologia-leiloes.md` (3, incluindo o
callout 🚨 "os dois marcos que mais derrubam peça", que é o mais enfático de todos).

---

## 1. O ARTIGO 8º — integral, verbatim ✅ 🔴⭐⭐ (o eixo deste anexo)

> **Art. 8º** Se o imóvel for alienado durante a locação, o adquirente poderá denunciar o contrato, com o prazo de noventa dias para a desocupação, salvo se a locação for por tempo determinado e o contrato contiver cláusula de vigência em caso de alienação e estiver averbado junto à matrícula do imóvel.
>
> **§ 1º** Idêntico direito terá o promissário comprador e o promissário cessionário, em caráter irrevogável, com imissão na posse do imóvel e título registrado junto à matrícula do mesmo.
>
> **§ 2º** A denúncia deverá ser exercitada no prazo de noventa dias contados do registro da venda ou do compromisso, presumindo-se, após esse prazo, a concordância na manutenção da locação.

### 1.1 ⭐ O "salvo" do caput são **TRÊS requisitos CUMULATIVOS** — e todos se leem na matrícula

A locação **só resiste** à alienação se, **ao mesmo tempo**:

1. for **por tempo determinado**; **e**
2. o contrato contiver **cláusula de vigência em caso de alienação**; **e**
3. estiver **averbado junto à matrícula do imóvel**.

⭐ **Falhando UM dos três, o adquirente pode denunciar.** É item de due diligence de custo zero: os
requisitos 2 e 3 se verificam **na própria matrícula** — locação não averbada **não** blinda o
inquilino, por melhor que seja a cláusula do contrato dele. Contrato averbado, ao contrário, é
**bandeira vermelha de precificação**: pode significar imóvel ocupado até o fim do prazo.

⚠️ **Limite honesto:** o caput fala em **alienação**, não em **arrematação**. Ver os 🟡 do §1.3 antes
de cravar a aplicação ao leilão.

### 1.2 O §2º e a presunção

O §2º faz **duas** coisas: fixa o **marco** (registro) e cria a **consequência** (presunção de
concordância com a manutenção da locação). A parte que o corpus sempre acertou é a segunda — *"perdido
o prazo, presume-se concordância com a manutenção do contrato"* está **correto e é quase literal**.

🟡 **O que a lei NÃO diz:** se a presunção é **absoluta** (não admite prova em contrário) ou
**relativa**. O texto diz apenas "presumindo-se". Skill que afirmar que o arrematante **pode** ou
**não pode** derrubar a presunção está afirmando o que a lei não afirmou → ressalva obrigatória e
rota ao `validador-leiloes`.

### 1.3 🟡 Os dois pontos que a lei NÃO resolve para o leilão — ressalva obrigatória

1. 🟡 **A arrematação é "alienação" para o art. 8º?** O caput diz "se o imóvel for **alienado**"; não
   menciona arrematação, hasta pública nem leilão. Aplicar o art. 8º ao arrematante é a leitura
   corrente e é a que este plugin adota — mas **não é literal**, e não foi confirmada em
   jurisprudência nesta captura.
2. 🟡 **O registro da carta de arrematação é o "registro da venda" do §2º?** O §2º fala em "registro
   da **venda** ou do **compromisso**". Se o título do arrematante (carta de arrematação, ou a
   escritura no extrajudicial) equivale a "venda" para efeito do marco **não está dito na lei**.

⭐ **Postura operacional segura, que sobrevive aos dois 🟡:** **denuncie cedo e registre as duas
datas.** Uma denúncia feita logo após a aquisição é boa sob **qualquer** das leituras possíveis do
marco; uma denúncia tardia depende de vencer os dois 🟡 ao mesmo tempo. Grave sempre **a data da
alienação E a data do registro** (`memoria-de-caso-leilao`) — o cálculo muda conforme o 🟡 se
resolva.

- **Usa:** `desocupacao-locacao-e-ocupantes` ⭐⭐ · `situacao-possessoria` ⭐ ·
  `defesa-contra-imissao-e-embargos-de-terceiro` · `suprema-corte-leiloes` (R3) ·
  `leitura-de-matricula` ⭐ (os requisitos 2 e 3 do "salvo") · `custo-total-real-e-precificacao` ·
  `memoria-de-caso-leilao` · `validador-leiloes`.

---

## 2. O art. 7º — o paralelo que **confirma** a leitura do §2º ✅ ⭐

> **Art. 7º** Nos casos de extinção de usufruto ou de fideicomisso, a locação celebrada pelo usufrutuário ou fiduciário poderá ser denunciada, com o prazo de trinta dias para a desocupação, salvo se tiver havido aquiescência escrita do nuproprietário ou do fideicomissário, ou se a propriedade estiver consolidada em mãos do usufrutuário ou do fiduciário.
>
> **Parágrafo único.** A denúncia deverá ser exercitada no prazo de noventa dias contados da extinção do fideicomisso ou da averbação da extinção do usufruto, presumindo-se, após esse prazo, a concordância na manutenção da locação.

⭐ **Não é curiosidade — é reforço de interpretação.** O art. 7º tem a **mesma arquitetura** do art. 8º:
o **caput** dá o prazo de **desocupação** (aqui 30 dias), e o **parágrafo** dá o prazo de **90 dias
para exercer a denúncia**, contado de um **evento de publicidade registral** ("averbação da extinção
do usufruto"). Dois artigos seguidos, mesma técnica: **o prazo de exercício conta do ato registral,
nunca do fato econômico.** Quem lê os dois juntos não erra o marco do art. 8º.

---

## 3. ⭐⭐ AS TRÊS ROTAS NÃO SE MISTURAM — a tabela que decide qual regra aplicar

Este é o cruzamento que o plugin precisa fazer **antes** de citar prazo de locação. **Rota errada =
prazo errado, marco errado e prazo de desocupação errado.**

| | **Alienação em geral / arrematação judicial** | **AF extrajudicial (Lei 9.514)** | **Locação longa sem anuência (Lei 9.514)** |
|---|---|---|---|
| Fundamento | **8.245, art. 8º** | **9.514, art. 27, §7º** | **9.514, art. 37-B** |
| Quem denuncia | o **adquirente** | o **fiduciário** (e sucessores) | — (a locação é **ineficaz**) |
| Prazo para **denunciar** | **90 dias** | **90 dias** | — |
| ⭐ **Marco** | **registro** da venda ou do compromisso | **consolidação** da propriedade | — |
| Prazo para **desocupar** | **90 dias** | ⚠️ **30 dias** | — |
| Não se aplica se | prazo determinado **+** cláusula de vigência **+** averbada | houve **aquiescência por escrito** do fiduciário | locação de **até 1 ano**, ou com anuência escrita |
| Exigência de forma | — | cláusula específica com **destaque gráfico** | anuência **por escrito** |

🔴 **Os dois erros que esta tabela existe para impedir:**

1. **Aplicar os 30 dias do 9.514 art. 27, §7º a uma arrematação judicial** — na rota judicial o prazo
   de desocupação é de **90 dias** (art. 8º, caput), não 30.
2. **Aplicar o marco "consolidação" a uma arrematação judicial** — consolidação é instituto da
   **alienação fiduciária**; em leilão judicial ela **não existe**. O marco é **registral**.

⚠️ **E a recíproca:** no extrajudicial da 9.514 o marco **é** a consolidação, por texto expresso —
não se transporta o "registro" do art. 8º para lá. Ver `context/lei-9514-consolidada.md` §5 (art. 27 Lei 9.514,
§7º) e §11 (art. 37-B Lei 9.514).

- **Usa:** `desocupacao-locacao-e-ocupantes` ⭐⭐ · `triagem-leiloes` ⭐ (a rota decide tudo) ·
  `situacao-possessoria` · `suprema-corte-leiloes` (R4 — via e regime).

---

## 4. A VIA é o DESPEJO — art. 5º ✅ 🔴⭐ (e a assimetria que encarece a rota judicial)

> **Art. 5º** Seja qual for o fundamento do término da locação, a ação do locador para reaver o imóvel é a de despejo.
>
> **Parágrafo único.** O disposto neste artigo não se aplica se a locação termina em decorrência de desapropriação, com a imissão do expropriante na posse do imóvel.

🔴 **Denunciada a locação e não saindo o locatário, o caminho é AÇÃO DE DESPEJO** — não é petição nos
autos da execução, não é mandado de imissão contra o inquilino. "Seja qual for o fundamento" é
categórico.

🔴🔴 **E aqui está a pior notícia honesta deste anexo: esse despejo NÃO tem liminar.** O rol de
liminares do **art. 59, §1º** é de **fundamento exclusivo** e tem **nove incisos** (§7) — e **nenhum
deles é a denúncia por alienação do art. 8º**. Conferido por prova negativa (§14).

⭐ **A assimetria, em uma linha:**

| | **Arrematação judicial com locatário** | **AF extrajudicial (9.514, art. 30)** |
|---|---|---|
| Contra o **locatário** | **despejo**, rito ordinário, **sem liminar** no rol do 59 §1º | reintegração **liminar por lei**, 60 dias |
| Prazo após a sentença | **30 dias** (art. 63 Lei 8.245) | 60 dias da liminar |

**Consequência de precificação:** lote judicial **com locação viva** é caro em tempo, e o custo não
aparece no edital. Quem compara judicial × extrajudicial sem esse item compara errado.

🟡 **O que a lei não resolve:** se o arrematante pode, em lugar do despejo, obter **tutela de urgência
genérica** ou usar a **imissão na posse** contra o locatário. O art. 5º não abre exceção e o rol do
59 §1º não contempla a hipótese — mas isso é leitura de texto, **não** jurisprudência confirmada.
Ressalva obrigatória + rota ao `validador-leiloes`.

- **Usa:** `imissao-na-posse-do-arrematante` ⭐ · `desocupacao-locacao-e-ocupantes` ⭐ ·
  `custo-total-real-e-precificacao` ⭐ · `defesa-contra-imissao-e-embargos-de-terceiro` ·
  `analise-de-edital`.

---

## 5. PREFERÊNCIA DO LOCATÁRIO — arts. 27 a 34 Lei 8.245 ✅ 🔴⭐⭐ (o que **não** alcança o leilão)

> **Art. 27 (Lei 8.245).** No caso de venda, promessa de venda, cessão ou promessa de cessão de direitos ou dação em pagamento, o locatário tem preferência para adquirir o imóvel locado, em igualdade de condições com terceiros, devendo o locador dar-lhe conhecimento do negócio mediante notificação judicial, extrajudicial ou outro meio de ciência inequívoca.
>
> **Parágrafo único.** A comunicação deverá conter todas as condições do negócio e, em especial, o preço, a forma de pagamento, a existência de ônus reais, bem como o local e horário em que pode ser examinada a documentação pertinente.

> **Art. 28.** O direito de preferência do locatário caducará se não manifestada, de maneira inequívoca, sua aceitação integral à proposta, no prazo de trinta dias.

> **Art. 31.** Em se tratando de alienação de mais de uma unidade imobiliária, o direito de preferência incidirá sobre a totalidade dos bens objeto da alienação.

> **Art. 32.** O direito de preferência não alcança os casos de perda da propriedade ou venda por decisão judicial, permuta, doação, integralização de capital, cisão, fusão e incorporação.
>
> **Parágrafo único.** Nos contratos firmados a partir de 1o de outubro de 2001, o direito de preferência de que trata este artigo não alcançará também os casos de constituição da propriedade fiduciária e de perda da propriedade ou venda por quaisquer formas de realização de garantia, inclusive mediante leilão extrajudicial, devendo essa condição constar expressamente em cláusula contratual específica, destacando-se das demais por sua apresentação gráfica. **(Incluído pela Lei nº 10.931, de 2004)**

> **Art. 33.** O locatário preterido no seu direito de preferência poderá reclamar do alienante as perdas e danos ou, depositando o preço e demais despesas do ato de transferência, haver para si o imóvel locado, se o requerer no prazo de seis meses, a contar do registro do ato no cartório de imóveis, desde que o contrato de locação esteja averbado pelo menos trinta dias antes da alienação junto à matrícula do imóvel.
>
> **Parágrafo único.** A averbação far-se-á à vista de qualquer das vias do contrato de locação desde que subscrito também por duas testemunhas.

### 5.1 ⭐⭐ O art. 32 é a blindagem do arrematante — e o corpus não a tinha

🔴 **No leilão JUDICIAL o locatário não tem preferência.** O art. 32, **caput**, é expresso: a
preferência "não alcança os casos de **perda da propriedade ou venda por decisão judicial**". Não é
tese — é letra da lei.

🔴 **No leilão EXTRAJUDICIAL de realização de garantia, idem** — pelo **parágrafo único**, que fala
literalmente em "venda por quaisquer formas de realização de garantia, **inclusive mediante leilão
extrajudicial**", para contratos firmados **a partir de 1º/10/2001**.

⭐ **Por que isso é ouro para o arrematante:** sem o art. 32, o **art. 33** deixaria o locatário
preterido **tomar o imóvel para si** depositando o preço, dentro de **6 meses contados do registro**.
Esse é um risco de desfazimento que **não** existe na aquisição em leilão — e é exatamente o tipo de
munição que uma peça de defesa da arrematação deve ter à mão.

### 5.2 🟡 O limite honesto do parágrafo único — não transformar em bala de prata

O parágrafo único condiciona o afastamento da preferência a que "essa condição conste expressamente
em **cláusula contratual específica**, destacando-se das demais por sua **apresentação gráfica**".

🟡 **A lei não diz em QUAL contrato a cláusula tem de estar** — no contrato de **locação** (que é o
"contrato firmado a partir de 1º/10/2001" mencionado no início do dispositivo) ou no contrato de
**garantia/alienação fiduciária** (leitura que espelha o 9.514, art. 27, §7º). O texto é ambíguo e
**não foi resolvido em jurisprudência nesta captura**. Skill que afirmar uma das duas leituras como
certa está inventando → ressalva obrigatória e rota ao `validador-leiloes`.

⚠️ **Mas repare na assimetria útil:** a ressalva do 🟡 atinge **apenas o parágrafo único**
(extrajudicial de garantia). O **caput** — que cobre o **leilão judicial** — é incondicionado: não
exige cláusula nenhuma. **No judicial, a blindagem é ✅ limpa.**

- **Usa:** `defesa-contra-imissao-e-embargos-de-terceiro` ⭐ · `situacao-possessoria` ⭐ ·
  `analise-de-edital` · `leitura-de-matricula` (a averbação do art. 33 é visível na matrícula) ·
  `eviccao-e-desfazimento-da-arrematacao` · `validador-leiloes`.

---

## 6. BENFEITORIAS — arts. 35 e 36 ✅ ⭐ (o crédito que o inquilino pode ter contra o arrematante)

> **Art. 35.** Salvo expressa disposição contratual em contrário, as benfeitorias necessárias introduzidas pelo locatário, ainda que não autorizadas pelo locador, bem como as úteis, desde que autorizadas, serão indenizáveis e permitem o exercício do direito de retenção.

> **Art. 36.** As benfeitorias voluptuárias não serão indenizáveis, podendo ser levantadas pelo locatário, finda a locação, desde que sua retirada não afete a estrutura e a substância do imóvel.

⭐ **Leia o art. 35 como uma equação de três variáveis, porque é isso que ele é:**

| Benfeitoria | Autorização necessária? | Indeniza? | **Retém o imóvel?** |
|---|---|---|---|
| **Necessária** | **não** — "ainda que não autorizadas" | ✅ sim | ✅ **sim** |
| **Útil** | ✅ **sim**, autorizada | ✅ sim | ✅ **sim** |
| **Útil não autorizada** | — | ❌ não | ❌ não |
| **Voluptuária** (art. 36) | — | ❌ não (pode **levantar**) | ❌ não |

🔴 **"Salvo expressa disposição contratual em contrário" é a primeira coisa a procurar.** A renúncia
contratual à indenização e à retenção é **admitida pelo próprio caput** — e é cláusula de estilo em
contrato de locação. **Ler o contrato do inquilino antes de precificar a saída dele.**

⚠️ **O direito de RETENÇÃO é o que dói:** não é só uma conta a pagar — é uma **defesa possessória**
que segura o imóvel enquanto não indenizado. Um arrematante que ignora benfeitorias necessárias pode
descobrir que o prazo de desocupação de 90 dias do art. 8º não termina em imóvel vazio.

🟡 **Não confirmado:** se o **arrematante** responde por benfeitorias feitas **antes** da aquisição, ou
se a obrigação fica com o alienante/executado. O art. 35 fala em indenização sem dizer **por quem**
na cadeia de sucessão. Ressalva obrigatória + rota ao `validador-leiloes`.

- **Usa:** `custo-total-real-e-precificacao` ⭐ · `desocupacao-locacao-e-ocupantes` ·
  `debitos-e-creditos-pos-arrematacao` · `defesa-contra-imissao-e-embargos-de-terceiro` ⭐ (a retenção
  é matéria de defesa de quem está dentro) · `situacao-possessoria`.

---

## 7. LIMINAR DE DESPEJO — art. 59, §1º ✅ 🔴 (nove incisos, e o art. 8º não é um deles)

> **§ 1º** Conceder-se-á liminar para desocupação em quinze dias, independentemente da audiência da parte contrária e desde que prestada a caução no valor equivalente a três meses de aluguel, nas ações que tiverem por fundamento exclusivo:
>
> I - o descumprimento do mútuo acordo (art. 9º, inciso I), celebrado por escrito e assinado pelas partes e por duas testemunhas, no qual tenha sido ajustado o prazo mínimo de seis meses para desocupação, contado da assinatura do instrumento;
>
> II - o disposto no inciso II do art. 47, havendo prova escrita da rescisão do contrato de trabalho ou sendo ela demonstrada em audiência prévia;
>
> III - o término do prazo da locação para temporada, tendo sido proposta a ação de despejo em até trinta dias após o vencimento do contrato;
>
> IV - a morte do locatário sem deixar sucessor legítimo na locação, de acordo com o referido no inciso I do art. 11, permanecendo no imóvel pessoas não autorizadas por lei;
>
> V - a permanência do sublocatário no imóvel, extinta a locação, celebrada com o locatário.
>
> VI – o disposto no inciso IV do art. 9o, havendo a necessidade de se produzir reparações urgentes no imóvel, determinadas pelo poder público, que não possam ser normalmente executadas com a permanência do locatário, ou, podendo, ele se recuse a consenti-las; **(Incluído pela Lei nº 12.112, de 2009)**
>
> VII – o término do prazo notificatório previsto no parágrafo único do art. 40, sem apresentação de nova garantia apta a manter a segurança inaugural do contrato; **(Incluído pela Lei nº 12.112, de 2009)**
>
> VIII – o término do prazo da locação não residencial, tendo sido proposta a ação em até 30 (trinta) dias do termo ou do cumprimento de notificação comunicando o intento de retomada; **(Incluído pela Lei nº 12.112, de 2009)**
>
> IX – a falta de pagamento de aluguel e acessórios da locação no vencimento, estando o contrato desprovido de qualquer das garantias previstas no art. 37, por não ter sido contratada ou em caso de extinção ou pedido de exoneração dela, independentemente de motivo. **(Incluído pela Lei nº 12.112, de 2009)**

🔴 **São NOVE incisos, o rol é de "fundamento EXCLUSIVO", e a denúncia por alienação (art. 8º) não
está entre eles.** Conferido por prova negativa. Skill que prometer "despejo liminar" ao arrematante
que denunciou a locação está prometendo o que a lei não dá.

⭐ **O que o arrematante PODE aproveitar do rol,** quando o caso se encaixa por outro fundamento:
**inciso VIII** (locação **não residencial** com prazo terminado, ação em até 30 dias do termo ou da
notificação de retomada) e **inciso IX** (falta de pagamento com contrato **sem garantia**). Ambos
exigem **caução de 3 meses de aluguel** e dão **15 dias** para desocupar. ⚠️ No inciso IX o locatário
**elide a liminar** depositando o total devido dentro dos 15 dias (§3º).

- **Usa:** `desocupacao-locacao-e-ocupantes` ⭐ · `imissao-na-posse-do-arrematante` ·
  `custo-total-real-e-precificacao` · `suprema-corte-leiloes` (R4).

---

## 8. PRAZOS DA SENTENÇA E DA PROVISÓRIA — arts. 63 e 64 Lei 8.245 ✅ 🔴

> **Art. 63.** Julgada procedente a ação de despejo, o juiz determinará a expedição de mandado de despejo, que conterá o prazo de 30 (trinta) dias para a desocupação voluntária, ressalvado o disposto nos parágrafos seguintes. **(Redação dada pela Lei nº 12.112, de 2009)**
>
> **§ 1º** O prazo será de quinze dias se:
> a) entre a citação e a sentença de primeira instância houverem decorrido mais de quatro meses; ou
> b) o despejo houver sido decretado com fundamento no art. 9o ou no § 2o do art. 46. **(Redação dada pela Lei nº 12.112, de 2009)**

> **Art. 64.** Salvo nas hipóteses das ações fundadas no art. 9o, a execução provisória do despejo dependerá de caução não inferior a 6 (seis) meses nem superior a 12 (doze) meses do aluguel, atualizado até a data da prestação da caução. **(Redação dada pela Lei nº 12.112, de 2009)**

🔴 **Duas armadilhas de redação antiga nesta faixa** (as duas descartadas no AVISO 2):
citar o art. 63 Lei 8.245 como *"o juiz fixará prazo de trinta dias"* (redação de 1991, sem o mandado) e citar
o art. 64 Lei 8.245 com **"12 a 18 meses"** de caução — o vigente é **6 a 12**.

⭐ **O §1º, "a", é gratuito e quase sempre esquecido:** passados **mais de 4 meses** entre citação e
sentença, o prazo de desocupação cai de 30 para **15 dias**. Em despejo de arrematante, esse marco
costuma estar cumprido — pedir a redução na própria inicial não custa nada.

- **Usa:** `desocupacao-locacao-e-ocupantes` · `custo-total-real-e-precificacao` ⭐ ·
  `imissao-na-posse-do-arrematante`.

---

## 9. PERDI OS 90 DIAS — e agora? arts. 46, 47 e 57 ✅ ⭐

Cenário real: estourou o prazo do §2º, presume-se a manutenção da locação, e o arrematante virou
**locador** de um contrato que não escolheu. A saída não é imediata, mas existe — e **depende do tipo
e do prazo do contrato**.

> **Art. 46.** Nas locações ajustadas por escrito e por prazo igual ou superior a trinta meses, a resolução do contrato ocorrerá findo o prazo estipulado, independentemente de notificação ou aviso.
>
> **§ 1º** Findo o prazo ajustado, se o locatário continuar na posse do imóvel alugado por mais de trinta dias sem oposição do locador, presumir-se-á prorrogada a locação por prazo indeterminado, mantidas as demais cláusulas e condições do contrato.
>
> **§ 2º** Ocorrendo a prorrogação, o locador poderá denunciar o contrato a qualquer tempo, concedido o prazo de trinta dias para desocupação.

> **Art. 47.** Quando ajustada verbalmente ou por escrito e como prazo inferior a trinta meses, findo o prazo estabelecido, a locação prorroga-se automaticamente, por prazo indeterminado, somente podendo ser retomado o imóvel:
> I - Nos casos do art. 9º;
> II - em decorrência de extinção do contrato de trabalho, se a ocupação do imóvel pelo locatário relacionada com o seu emprego;
> III - se for pedido para uso próprio, de seu cônjuge ou companheiro, ou para uso residencial de ascendente ou descendente que não disponha, assim como seu cônjuge ou companheiro, de imóvel residencial próprio;
> IV - se for pedido para demolição e edificação licenciada ou para a realização de obras aprovadas pelo Poder Público, que aumentem a área construída, em, no mínimo, vinte por cento ou, se o imóvel for destinado a exploração de hotel ou pensão, em cinqüenta por cento;
> V - se a vigência ininterrupta da locação ultrapassar cinco anos.

> **Art. 57.** O contrato de locação por prazo indeterminado pode ser denunciado por escrito, pelo locador, concedidos ao locatário trinta dias para a desocupação.

🔴 **A diferença entre 30 meses e menos de 30 meses decide tudo.** Residencial **≥ 30 meses** que
prorrogou: denúncia **vazia**, a qualquer tempo, 30 dias (art. 46, §2º). Residencial **< 30 meses**:
**não** há denúncia vazia — só se retoma nas hipóteses do rol do art. 47, e a mais acessível para
quem só quer o imóvel livre é o **inciso V** (5 anos ininterruptos de locação). **Não residencial**
por prazo indeterminado: 30 dias (art. 57).

⚠️ **Nas retomadas dos incisos III e IV do art. 47, o locatário que concorda ganha SEIS MESES** para
sair, contados da citação (art. 61) — e o autor ainda arca com custas e honorários se não o fizer no
prazo. Custo real de calendário.

- **Usa:** `desocupacao-locacao-e-ocupantes` ⭐ · `custo-total-real-e-precificacao` ⭐ ·
  `situacao-possessoria`.

---

## 10. LOCAÇÃO COMERCIAL — a renovatória é o pior cenário do arrematante ✅ ⚠️

> **Art. 51.** Nas locações de imóveis destinados ao comércio, o locatário terá direito a renovação do contrato, por igual prazo, desde que, cumulativamente:
> I - o contrato a renovar tenha sido celebrado por escrito e com prazo determinado;
> II - o prazo mínimo do contrato a renovar ou a soma dos prazos ininterruptos dos contratos escritos seja de cinco anos;
> III - o locatário esteja explorando seu comércio, no mesmo ramo, pelo prazo mínimo e ininterrupto de três anos.
>
> **§ 5º** Do direito a renovação decai aquele que não propuser a ação no interregno de um ano, no máximo, até seis meses, no mínimo, anteriores à data da finalização do prazo do contrato em vigor.

> **Art. 74.** Não sendo renovada a locação, o juiz determinará a expedição de mandado de despejo, que conterá o prazo de 30 (trinta) dias para a desocupação voluntária, se houver pedido na contestação. **(Redação dada pela Lei nº 12.112, de 2009)**

⚠️ **Ponto de vistoria em lote comercial:** locatário com **5 anos** de contrato e **3 anos** no mesmo
ramo tem **direito à renovação por igual prazo**. Os três requisitos são **cumulativos** — e o **§5º**
dá uma **janela de decadência estreita** (de 1 ano a 6 meses antes do fim do contrato) que, perdida
pelo locatário, extingue o direito.

🟡 **A lei não diz** como a renovatória interage com a **denúncia do art. 8º** feita pelo arrematante
— se a cláusula de vigência averbada é pressuposto, se a ação renovatória em curso obsta a denúncia,
ou o contrário. Nada disso está no texto. Ressalva obrigatória + rota ao `validador-leiloes`.

- **Usa:** `situacao-possessoria` ⭐ · `desocupacao-locacao-e-ocupantes` · `analise-de-edital` ·
  `custo-total-real-e-precificacao`.

---

## 11. O FIADOR PODE SUMIR NA ALIENAÇÃO — art. 40, VII ✅ ⚠️ (detalhe que ninguém lembra)

> **Art. 40.** O locador poderá exigir novo fiador ou a substituição da modalidade de garantia, nos seguintes casos:
> (…) **VII - desapropriação ou alienação do imóvel.**
>
> **Parágrafo único.** O locador poderá notificar o locatário para apresentar nova garantia locatícia no prazo de 30 (trinta) dias, sob pena de desfazimento da locação. **(Incluído pela Lei nº 12.112, de 2009)**

⚠️ **O arrematante que herda a locação pode herdá-la SEM garantia.** A alienação do imóvel é, por
texto expresso, causa para **exigir novo fiador**. Ler junto com o **parágrafo único**: notificado o
locatário e não apresentada nova garantia em **30 dias**, a sanção é o **desfazimento da locação**.

⭐ **Isso é uma segunda porta de saída** para quem perdeu os 90 dias do art. 8º — e ela **também**
destrava o **inciso VII do art. 59, §1º**, que é hipótese de **liminar** (§7). Caminho: notificar →
30 dias sem garantia → despejo **com liminar**. É a rota mais rápida que a lei oferece ao arrematante
que ficou com o inquilino, e depende de um fato objetivo (ausência de garantia nova), não de tese.

- **Usa:** `desocupacao-locacao-e-ocupantes` ⭐⭐ · `imissao-na-posse-do-arrematante` ·
  `custo-total-real-e-precificacao`.

---

## 12. COMO SE CONTA o prazo de 90 dias 🔴

Os prazos desta lei aqui tratados (90 dias do art. 8º, 30 dias do art. 57, 6 meses do art. 33) são de
**direito material** — exercidos por **notificação**, fora do processo. **Não são prazos processuais**
e, portanto, **não** entram na contagem em dias úteis do **CPC, art. 219**, cujo parágrafo único
limita a regra aos prazos processuais.

🔴 **Isto já está travado no anexo irmão** `context/cpc-leilao-879-903.md`, que proíbe expressamente
migrar o art. 219 para prazos materiais e cita, nominalmente, "os 90 dias do art. 8º da Lei 8.245".
**Não reabrir a discussão nem contar em dias úteis.**

> **Fora de escopo (ponteiro):** garantias locatícias (arts. 37 a 42), ação revisional (arts. 68 a
> 70), consignatória (art. 67), purgação da mora do art. 62 e o rito da renovatória (arts. 71 a 75)
> **não** são transcritos aqui — o plugin só os alcança se o arrematante virar locador e o caso sair
> do escopo de leilões. Nesse ponto, `context/metodologia-leiloes.md` §11 manda parar e rotear.

---

## 13. Tabela-resumo — todo prazo desta lei que o leilão toca

| Prazo | Do quê | ⭐ Contado de | Âncora |
|---|---|---|---|
| **90 dias** ⭐ | o adquirente **exercer a denúncia** | 🔴 **REGISTRO da venda ou do compromisso** | **art. 8º, §2º** |
| **90 dias** | o locatário **desocupar**, após a denúncia | da **denúncia** | art. 8º, caput |
| até **180 dias** | horizonte total até o imóvel vazio (90 + 90) | do **registro** | art. 8º, caput + §2º |
| 90 dias (AF) | denúncia no extrajudicial da 9.514 | **CONSOLIDAÇÃO** (regra diversa) | 9.514, art. 27, §7º |
| 30 dias (AF) | desocupação no extrajudicial da 9.514 | da denúncia | 9.514, art. 27, §7º |
| **30 dias** | preferência: caducidade da aceitação do locatário | da proposta | art. 28 |
| **6 meses** | locatário preterido **haver o imóvel para si** | **registro do ato** no cartório | art. 33 |
| **30 dias** | antecedência mínima da averbação da locação (requisito do art. 33) | antes da **alienação** | art. 33 |
| **15 dias** | desocupação na **liminar** de despejo (9 hipóteses) | da liminar | art. 59, §1º |
| **30 dias** | desocupação voluntária após sentença de despejo | do mandado | art. 63 Lei 8.245 |
| **15 dias** | idem, se >4 meses entre citação e sentença | do mandado | art. 63, §1º, "a" Lei 8.245 |
| **6 a 12 meses** de aluguel | caução da execução provisória do despejo | — | art. 64 Lei 8.245 |
| **30 dias** | denúncia vazia na locação prorrogada (≥30 meses) | da denúncia | art. 46, §2º |
| **5 anos** | vigência ininterrupta que permite retomada (<30 meses) | — | art. 47, V |
| **30 dias** | denúncia da não residencial por prazo indeterminado | da denúncia | art. 57 |
| **30 dias** | apresentar nova garantia, sob pena de desfazimento | da notificação | art. 40, §único |
| **5 anos + 3 anos** | requisitos da renovatória comercial | — | art. 51, II e III |
| **1 ano a 6 meses antes** | janela para propor a renovatória (decadência) | do fim do contrato | art. 51, §5º |
| **6 meses** | desocupação quando o locatário concorda (art. 47, III e IV) | da **citação** | art. 61 |

---

## GUARD — o que este anexo proíbe

1. 🔴 Escrever que os **90 dias correm "da alienação"**, "da arrematação", "da carta" ou "da imissão" —
   o **art. 8º, §2º** diz **"contados do registro da venda ou do compromisso"**. A expressão
   *"contados da alienação"* **não existe** nesta lei.
2. 🔴 **Fundir os dois prazos de 90 dias** do art. 8º. Um é para **denunciar** (§2º, do registro); o
   outro é para **desocupar** (caput, da denúncia). O horizonte é **até 180 dias**, não 90.
3. Afirmar que a **presunção do §2º** é absoluta **ou** relativa — a lei só diz "presumindo-se" (🟡).
4. Tratar como ✅ que a **arrematação é "alienação"** do art. 8º e que a **carta registrada é "registro
   da venda"** — são as duas leituras que este plugin adota, mas ambas são **🟡** (§1.3). Denunciar
   cedo e gravar as duas datas.
5. Aplicar os **30 dias** de desocupação do **9.514, art. 27, §7º** a uma **arrematação judicial** — lá
   o prazo é **90 dias**; e não aplicar o marco **"consolidação"** fora da alienação fiduciária.
6. Prometer **despejo liminar** ao arrematante que denunciou pelo art. 8º — o rol do **art. 59, §1º**
   é de **fundamento exclusivo**, tem **nove incisos** e **não** contempla a denúncia por alienação.
7. Dizer que o **locatário tem preferência** no leilão — o **art. 32, caput** exclui a **venda por
   decisão judicial** e o **parágrafo único** exclui o **leilão extrajudicial** de garantia.
8. Usar o **art. 32, parágrafo único** como se fosse incondicionado: ele exige **cláusula específica
   com destaque gráfico**, e **em qual contrato** ela deve estar é **🟡**. (O **caput**, que cobre o
   judicial, é incondicionado — esse é ✅.)
9. Citar o **art. 32, §único pela MP 2.223/2001** — a página exibe as duas; a atribuição vigente é a
   **Lei 10.931/2004**, mesmo endereço e mesmo texto.
10. Citar o **art. 63 Lei 8.245** com "o juiz **fixará** prazo de trinta dias" (redação de 1991) ou o **art. 64 Lei 8.245**
    com caução de **12 a 18 meses** — vigentes: **mandado de despejo** com 30 dias, e **6 a 12 meses**.
11. Ignorar o **direito de retenção** por benfeitorias (art. 35) ao prometer imóvel vazio — e ignorar
    que o próprio caput admite **renúncia contratual** a ele.
12. Contar qualquer prazo deste anexo em **dias úteis** pelo **CPC 219** — são prazos de direito
    material (§12).
13. Afirmar que a Lei 8.245 mudou depois de **2012** — não mudou; **nenhuma lei 13.x/14.x/15.x** a
    alterou (§14).

Toda peça fecha por **`suprema-corte-leiloes`** (R1-R4) **+ `validador-leiloes`**.

---

## 14. Fonte e verificação

- **Lei 8.245/1991 — texto compilado:** `https://www.planalto.gov.br/ccivil_03/leis/l8245.htm`
  (captura **2026-08-02**, 108.750 bytes). Conversão local do HTML (`ISO-8859-1` → UTF-8), sem
  passar por resumidor.
- **Conferência por script:** **33 asserções, 0 falha**, rodadas sobre o texto normalizado —
  transcrição integral do art. 8º (caput, §1º, §2º), do art. 7º, §único, dos arts. 5º, 32, 33, 35,
  36, 40 VII, 46 §2º, 47, 51, 57, 59 §1º, 63, 64 e 74; mais **provas negativas** de que
  *"contados da alienação"*, *"90 dias contados da alienação"* e *"contados da arrematação"* têm
  **zero ocorrência** na lei.
- **Vigência:** varredura de **todas** as notas de alteração da página — a mais recente é a **Lei
  12.744/2012**. Zero ocorrências de "Lei nº 13.x / 14.x / 15.x" e zero de "de 202x".
- **Duas armadilhas de página travadas:** art. 63 e art. 64 Lei 8.245 exibem a redação **original ao lado da
  vigente**; art. 32, §único aparece **duas vezes** (MP 2.223/2001 e Lei 10.931/2004) com **texto
  normativo idêntico** — muda só a atribuição.
- **Anexos irmãos:** `context/lei-9514-consolidada.md` (art. 27 §7º e art. 37-B Lei 9.514 — o regime da AF, que
  **não** se mistura com este) · `context/cpc-leilao-879-903.md` (contagem de prazos) ·
  `context/metodologia-leiloes.md` · `context/custo-total-do-arrematante.md` ·
  `context/clausulas-armadilha-de-edital.md`.
