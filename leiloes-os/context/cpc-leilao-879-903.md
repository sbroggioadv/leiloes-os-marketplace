# Anexo — CPC/2015: leilão judicial (arts. 876-903) + 804 + 826 + 908 §1º

> **Anexo de legislação do `leiloes-os`.** É a âncora textual do leilão **judicial**: a expropriação
> da adjudicação ao art. 903. Toda skill que citar dispositivo do CPC fecha aqui — citar de cabeça
> reprova no `validador-leiloes`.
>
> **Fonte:** texto **compilado** do **CPC (Lei 13.105/2015)** capturado do Planalto em **2026-08-02** —
> `https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2015/lei/l13105.htm`. Transcrição **verbatim**,
> extraída por script da própria captura (não redigitada, não parafraseada).
>
> **Legenda:** ✅ conferido verbatim na fonte oficial · 🟡 não confirmado (não citar sem checar) ·
> 🔴 verdade dura / erro de mercado a bloquear · ⭐ eixo do domínio.

---

## ⚠️ AVISO 1 — grep o artigo e leia a faixa. NUNCA despeje o anexo inteiro

Este arquivo é **consulta pontual**, não leitura de contexto. **Faça `grep` do número do artigo e leia
só a faixa correspondente.** Carregar o anexo inteiro numa peça queima contexto e não melhora a
citação. Cada bloco traz: **artigo · texto literal · o que isso decide no leilão · quem usa**.

## ⚠️ AVISO 2 — vigência: a faixa 876-908 NÃO tem nota de alteração (conferido) ✅

Varredura feita na própria captura de 02/08/2026, no intervalo dos arts. 876 a 908: **zero**
ocorrências de `Redação dada`, `Incluído pela`, `Revogado` ou `Vigência`. Os dispositivos do leilão
judicial permanecem com a **redação original da Lei 13.105/2015**.

🔴 **Corolário que o plugin repete:** a **Lei 14.711/2023 não tocou no leilão judicial**. Ela alterou o
CPC apenas no art. 784 (inciso XI-A, seguro-garantia). Toda a mudança do Marco das Garantias está no
**extrajudicial** — ver `context/lei-9514-consolidada.md` e `context/lei-14711-2023.md`. Quem
"atualiza" o leilão judicial pela 14.711 está inventando alteração que não existe.

## ⚠️ AVISO 3 — a pegadinha de Planalto, e por que ela NÃO incide aqui

A página compilada do Planalto exibe, lado a lado, **redação revogada e redação vigente** (o padrão é
a antiga riscada/anotada e a nova com `(Redação dada pela Lei ...)`). Em outros diplomas deste plugin
isso já obrigou a travar o dispositivo — ver o **§1º do art. 63** no anexo de CPC do plugin agrário,
onde citar a redação de 2015 é citar texto superado.

**Na faixa 876-908 a armadilha não se materializa**, porque não há redação sucessiva: o texto exibido
é único. **Mas a disciplina permanece:** ao citar **qualquer** artigo do CPC fora desta faixa (219,
300, 1.015, 1.022…), conferir na página se há duas redações antes de transcrever. A ausência de
armadilha aqui é um **fato conferido**, não uma licença geral.

---

## 0. O mapa da expropriação — onde o leilão entra

O leilão é a **terceira** via, não a primeira:

1. **Adjudicação** (arts. 876-878) — o exequente ou os legitimados ficam com o bem.
2. **Alienação por iniciativa particular** (art. 880) — venda direta, por corretor ou leiloeiro.
3. **Leilão judicial** (arts. 881-903) — só se as duas anteriores não se efetivarem.

> **Art. 881.** A alienação far-se-á em leilão judicial se não efetivada a adjudicação ou a alienação por iniciativa particular.
>
> **§ 1º** O leilão do bem penhorado será realizado por leiloeiro público.
>
> **§ 2º** Ressalvados os casos de alienação a cargo de corretores de bolsa de valores, todos os demais bens serão alienados em leilão público.

⭐ **Primeira pergunta da due diligence:** um bem que chegou ao leilão passou por **duas janelas** em
que o credor podia tê-lo tomado e não tomou. Isso é **sinal, não garantia** — mas obriga a pergunta
*por que ninguém adjudicou?*. **Usa:** `mecanica-do-leilao-judicial` · `parecer-go-nogo-lote`.

---

## 1. Adjudicação e a segunda janela — arts. 876 a 878 ✅

> **Art. 876.** É lícito ao exequente, oferecendo preço não inferior ao da avaliação, requerer que lhe sejam adjudicados os bens penhorados.
>
> **§ 1º** Requerida a adjudicação, o executado será intimado do pedido:
>
> I - pelo Diário da Justiça, na pessoa de seu advogado constituído nos autos;
>
> II - por carta com aviso de recebimento, quando representado pela Defensoria Pública ou quando não tiver procurador constituído nos autos;
>
> III - por meio eletrônico, quando, sendo o caso do § 1º do art. 246, não tiver procurador constituído nos autos.
>
> **§ 2º** Considera-se realizada a intimação quando o executado houver mudado de endereço sem prévia comunicação ao juízo, observado o disposto no art. 274, parágrafo único.
>
> **§ 3º** Se o executado, citado por edital, não tiver procurador constituído nos autos, é dispensável a intimação prevista no § 1º.
>
> **§ 4º** Se o valor do crédito for:
>
> I - inferior ao dos bens, o requerente da adjudicação depositará de imediato a diferença, que ficará à disposição do executado;
>
> II - superior ao dos bens, a execução prosseguirá pelo saldo remanescente.
>
> **§ 5º** Idêntico direito pode ser exercido por aqueles indicados no art. 889, incisos II a VIII, pelos credores concorrentes que hajam penhorado o mesmo bem, pelo cônjuge, pelo companheiro, pelos descendentes ou pelos ascendentes do executado.
>
> **§ 6º** Se houver mais de um pretendente, proceder-se-á a licitação entre eles, tendo preferência, em caso de igualdade de oferta, o cônjuge, o companheiro, o descendente ou o ascendente, nessa ordem.
>
> **§ 7º** No caso de penhora de quota social ou de ação de sociedade anônima fechada realizada em favor de exequente alheio à sociedade, esta será intimada, ficando responsável por informar aos sócios a ocorrência da penhora, assegurando-se a estes a preferência.

> **Art. 877.** Transcorrido o prazo de 5 (cinco) dias, contado da última intimação, e decididas eventuais questões, o juiz ordenará a lavratura do auto de adjudicação.
>
> **§ 1º** Considera-se perfeita e acabada a adjudicação com a lavratura e a assinatura do auto pelo juiz, pelo adjudicatário, pelo escrivão ou chefe de secretaria, e, se estiver presente, pelo executado, expedindo-se:
>
> I - a carta de adjudicação e o mandado de imissão na posse, quando se tratar de bem imóvel;
>
> II - a ordem de entrega ao adjudicatário, quando se tratar de bem móvel.
>
> **§ 2º** A carta de adjudicação conterá a descrição do imóvel, com remissão à sua matrícula e aos seus registros, a cópia do auto de adjudicação e a prova de quitação do imposto de transmissão.
>
> **§ 3º** No caso de penhora de bem hipotecado, o executado poderá remi-lo até a assinatura do auto de adjudicação, oferecendo preço igual ao da avaliação, se não tiver havido licitantes, ou ao do maior lance oferecido.
>
> **§ 4º** Na hipótese de falência ou de insolvência do devedor hipotecário, o direito de remição previsto no § 3º será deferido à massa ou aos credores em concurso, não podendo o exequente recusar o preço da avaliação do imóvel.

> **Art. 878.** Frustradas as tentativas de alienação do bem, será reaberta oportunidade para requerimento de adjudicação, caso em que também se poderá pleitear a realização de nova avaliação.
>
> Subseção II
>
> Da Alienação

- **O que decide:** a adjudicação **não tem** a mecânica de invalidação do art. 903 (que é da
  *arrematação*). Não transportar o prazo de 10 dias para ela sem fundamentar.
- ⭐ **O art. 878 é a janela esquecida do credor:** frustrado o leilão, **reabre-se** a adjudicação
  **com direito a pedir nova avaliação**. Dispositivo de alto valor e baixíssimo uso.
- **§3º do art. 877 é uma das TRÊS remições** — ver §14 deste anexo, e não confundir com 826 e 902.
- **Usa:** `adjudicacao-e-as-tres-remicoes` · `mecanica-do-leilao-judicial`.

---

## 2. Alienação por iniciativa particular — art. 880 ✅

> **Art. 880.** Não efetivada a adjudicação, o exequente poderá requerer a alienação por sua própria iniciativa ou por intermédio de corretor ou leiloeiro público credenciado perante o órgão judiciário.
>
> **§ 1º** O juiz fixará o prazo em que a alienação deve ser efetivada, a forma de publicidade, o preço mínimo, as condições de pagamento, as garantias e, se for o caso, a comissão de corretagem.
>
> **§ 2º** A alienação será formalizada por termo nos autos, com a assinatura do juiz, do exequente, do adquirente e, se estiver presente, do executado, expedindo-se:
>
> I - a carta de alienação e o mandado de imissão na posse, quando se tratar de bem imóvel;
>
> II - a ordem de entrega ao adquirente, quando se tratar de bem móvel.
>
> **§ 3º** Os tribunais poderão editar disposições complementares sobre o procedimento da alienação prevista neste artigo, admitindo, quando for o caso, o concurso de meios eletrônicos, e dispor sobre o credenciamento dos corretores e leiloeiros públicos, os quais deverão estar em exercício profissional por não menos que 3 (três) anos.
>
> **§ 4º** Nas localidades em que não houver corretor ou leiloeiro público credenciado nos termos do § 3º, a indicação será de livre escolha do exequente.

- 🔴 **Distinção que muda a peça:** o adquirente por iniciativa particular recebe **carta de
  ALIENAÇÃO**, não carta de arrematação, e o negócio se aperfeiçoa por **termo nos autos**. A mecânica
  do art. 903 (10 dias, invalidação, desistência) está redigida para a **arrematação**.
- 🟡 **Não estender automaticamente o art. 903 à alienação particular.** É ponto em aberto (frente A,
  `needs-human`), não regra assentada. Skill que tocar nisso marca *"conferir antes de protocolar"*.
- O piso de **3 anos de exercício profissional** (§3º) reaparece literalmente no art. 2º da
  **Res. CNJ 236/2016** — ver `context/resolucao-cnj-236-2016.md`.
- **Usa:** `mecanica-do-leilao-judicial` · `triagem-leiloes`.

---

## 3. Quem conduz — arts. 879, 882 e 883 ✅

> **Art. 879.** A alienação far-se-á:
>
> I - por iniciativa particular;
>
> II - em leilão judicial eletrônico ou presencial.

> **Art. 882.** Não sendo possível a sua realização por meio eletrônico, o leilão será presencial.
>
> **§ 1º** A alienação judicial por meio eletrônico será realizada, observando-se as garantias processuais das partes, de acordo com regulamentação específica do Conselho Nacional de Justiça.
>
> **§ 2º** A alienação judicial por meio eletrônico deverá atender aos requisitos de ampla publicidade, autenticidade e segurança, com observância das regras estabelecidas na legislação sobre certificação digital.
>
> **§ 3º** O leilão presencial será realizado no local designado pelo juiz.

> **Art. 883.** Caberá ao juiz a designação do leiloeiro público, que poderá ser indicado pelo exequente.

- **O que decide:** o eletrônico é a via **ordinária** e o presencial a **subsidiária justificada** — o
  art. 882 só o admite quando o eletrônico "não for possível". **Não afirmar que a lei "obriga" o
  eletrônico em termos absolutos.**
- O **§1º do art. 882 é o gancho legal da Res. CNJ 236/2016** — é dele que a Resolução tira competência.
- **Usa:** `mecanica-do-leilao-judicial` · `base-legal-leilao-judicial` · `estrategia-de-lance-e-habilitacao`.

---

## 4. Deveres do leiloeiro e a COMISSÃO — art. 884 ✅ ⭐

> **Art. 884.** Incumbe ao leiloeiro público:
>
> I - publicar o edital, anunciando a alienação;
>
> II - realizar o leilão onde se encontrem os bens ou no lugar designado pelo juiz;
>
> III - expor aos pretendentes os bens ou as amostras das mercadorias;
>
> IV - receber e depositar, dentro de 1 (um) dia, à ordem do juiz, o produto da alienação;
>
> V - prestar contas nos 2 (dois) dias subsequentes ao depósito.
>
> **Parágrafo único.** O leiloeiro tem o direito de receber do arrematante a comissão estabelecida em lei ou arbitrada pelo juiz.

- 🔴 **O CPC NÃO fixa percentual.** Diz "comissão estabelecida em lei ou arbitrada pelo juiz". Escrever
  *"a comissão é de 5% por força do CPC"* é **erro travado** (correção nº 4 do BUILD-CONTRACT). Os 5%
  vêm do **art. 24, §único, do Decreto 21.981/1932** e do **art. 7º da Res. CNJ 236/2016**
  ("**no mínimo** 5%") — ver `context/leiloeiro-decreto-21981-in-drei-52.md` e
  `context/resolucao-cnj-236-2016.md`.
- ⭐ **A comissão é do ARREMATANTE: soma-se ao lance, não sai dele.** Um lance de R$ 1.000.000 custa
  **R$ 1.050.000** só de lance + comissão a 5%, antes de ITBI, emolumentos, carrego e desocupação. A
  prova textual está no **art. 901, §1º** (§15 deste anexo). Conta completa em
  `context/custo-total-do-arrematante.md`.
- **Prazos operacionais do leiloeiro:** depósito em **1 dia** (IV), contas em **2 dias** (V).
- **Usa:** `custo-total-real-e-precificacao` · `leiloeiro-comissao-e-prestacao-de-contas` ·
  `analise-de-edital` · `arrematacao-auto-e-carta`.

---

## 5. Preço mínimo — art. 885 ✅

> **Art. 885.** O juiz da execução estabelecerá o preço mínimo, as condições de pagamento e as garantias que poderão ser prestadas pelo arrematante.

- ⭐ **A articulação 885 × 891 é a mais mal contada do mercado.** O preço mínimo é **decisão judicial**;
  sua **presença ou ausência** é o que aciona a régua em cascata do preço vil (§10 deste anexo).
- **Usa:** `preco-vil-como-tese` · `mecanica-do-leilao-judicial` · `analise-de-edital`.

---

## 6. Conteúdo obrigatório do edital — art. 886 ✅ ⭐⭐ (o gatilho da desistência)

> **Art. 886.** O leilão será precedido de publicação de edital, que conterá:
>
> I - a descrição do bem penhorado, com suas características, e, tratando-se de imóvel, sua situação e suas divisas, com remissão à matrícula e aos registros;
>
> II - o valor pelo qual o bem foi avaliado, o preço mínimo pelo qual poderá ser alienado, as condições de pagamento e, se for o caso, a comissão do leiloeiro designado;
>
> III - o lugar onde estiverem os móveis, os veículos e os semoventes e, tratando-se de créditos ou direitos, a identificação dos autos do processo em que foram penhorados;
>
> IV - o sítio, na rede mundial de computadores, e o período em que se realizará o leilão, salvo se este se der de modo presencial, hipótese em que serão indicados o local, o dia e a hora de sua realização;
>
> V - a indicação de local, dia e hora de segundo leilão presencial, para a hipótese de não haver interessado no primeiro;
>
> VI - menção da existência de ônus, recurso ou processo pendente sobre os bens a serem leiloados.
>
> **Parágrafo único.** No caso de títulos da dívida pública e de títulos negociados em bolsa, constará do edital o valor da última cotação.

- ⭐⭐ **O par 886, VI × 903, §5º, I é o eixo da defesa do arrematante.** O edital **deve** mencionar
  ônus, recurso ou processo pendente. Não mencionou, e o arrematante prova o ônus nos **10 dias**
  seguintes? Ele **desiste e recebe o depósito de volta imediatamente**. É a saída mais forte que ele
  tem — e **caduca em 10 dias**.
- **Inciso II:** havendo comissão fixada, ela **deve constar do edital**. Comissão que só aparece no
  regulamento da plataforma e **não** no edital é ponto de impugnação.
- **Auditoria cláusula a cláusula:** `context/clausulas-armadilha-de-edital.md` (as 16 armadilhas).
- **Usa:** `analise-de-edital` ⭐ · `invalidacao-embargos-e-desistencia-903` ·
  `risco-de-anulacao-do-certame` · `parecer-go-nogo-lote`.

---

## 7. Publicidade e adiamento — arts. 887 e 888 ✅

> **Art. 887.** O leiloeiro público designado adotará providências para a ampla divulgação da alienação.
>
> **§ 1º** A publicação do edital deverá ocorrer pelo menos 5 (cinco) dias antes da data marcada para o leilão.
>
> **§ 2º** O edital será publicado na rede mundial de computadores, em sítio designado pelo juízo da execução, e conterá descrição detalhada e, sempre que possível, ilustrada dos bens, informando expressamente se o leilão se realizará de forma eletrônica ou presencial.
>
> **§ 3º** Não sendo possível a publicação na rede mundial de computadores ou considerando o juiz, em atenção às condições da sede do juízo, que esse modo de divulgação é insuficiente ou inadequado, o edital será afixado em local de costume e publicado, em resumo, pelo menos uma vez em jornal de ampla circulação local.
>
> **§ 4º** Atendendo ao valor dos bens e às condições da sede do juízo, o juiz poderá alterar a forma e a frequência da publicidade na imprensa, mandar publicar o edital em local de ampla circulação de pessoas e divulgar avisos em emissora de rádio ou televisão local, bem como em sítios distintos do indicado no § 2º.
>
> **§ 5º** Os editais de leilão de imóveis e de veículos automotores serão publicados pela imprensa ou por outros meios de divulgação, preferencialmente na seção ou no local reservados à publicidade dos respectivos negócios.
>
> **§ 6º** O juiz poderá determinar a reunião de publicações em listas referentes a mais de uma execução.

> **Art. 888.** Não se realizando o leilão por qualquer motivo, o juiz mandará publicar a transferência, observando-se o disposto no art. 887.
>
> **Parágrafo único.** O escrivão, o chefe de secretaria ou o leiloeiro que culposamente der causa à transferência responde pelas despesas da nova publicação, podendo o juiz aplicar-lhe a pena de suspensão por 5 (cinco) dias a 3 (três) meses, em procedimento administrativo regular.

- 🔴 **Três "5 dias" diferentes — não confundir:** (a) **887, §1º** = antecedência da **publicação** do
  edital; (b) **art. 11 da Res. CNJ 236** = abertura do **sistema para lances**; (c) **889** =
  **cientificação de pessoas determinadas**. Mesmo número, funções distintas.
- **Usa:** `analise-de-edital` · `risco-de-anulacao-do-certame` · `mecanica-do-leilao-judicial`.

---

## 8. Quem deve ser cientificado — art. 889 ✅ ⭐ (o coração das nulidades)

> **Art. 889.** Serão cientificados da alienação judicial, com pelo menos 5 (cinco) dias de antecedência:
>
> I - o executado, por meio de seu advogado ou, se não tiver procurador constituído nos autos, por carta registrada, mandado, edital ou outro meio idôneo;
>
> II - o coproprietário de bem indivisível do qual tenha sido penhorada fração ideal;
>
> III - o titular de usufruto, uso, habitação, enfiteuse, direito de superfície, concessão de uso especial para fins de moradia ou concessão de direito real de uso, quando a penhora recair sobre bem gravado com tais direitos reais;
>
> IV - o proprietário do terreno submetido ao regime de direito de superfície, enfiteuse, concessão de uso especial para fins de moradia ou concessão de direito real de uso, quando a penhora recair sobre tais direitos reais;
>
> V - o credor pignoratício, hipotecário, anticrético, fiduciário ou com penhora anteriormente averbada, quando a penhora recair sobre bens com tais gravames, caso não seja o credor, de qualquer modo, parte na execução;
>
> VI - o promitente comprador, quando a penhora recair sobre bem em relação ao qual haja promessa de compra e venda registrada;
>
> VII - o promitente vendedor, quando a penhora recair sobre direito aquisitivo derivado de promessa de compra e venda registrada;
>
> VIII - a União, o Estado e o Município, no caso de alienação de bem tombado.
>
> **Parágrafo único.** Se o executado for revel e não tiver advogado constituído, não constando dos autos seu endereço atual ou, ainda, não sendo ele encontrado no endereço constante do processo, a intimação considerar-se-á feita por meio do próprio edital de leilão.

### A consequência correta: art. 804 — INEFICÁCIA relativa, não nulidade ✅ ⭐

> **Art. 804.** A alienação de bem gravado por penhor, hipoteca ou anticrese será ineficaz em relação ao credor pignoratício, hipotecário ou anticrético não intimado.
>
> **§ 1º** A alienação de bem objeto de promessa de compra e venda ou de cessão registrada será ineficaz em relação ao promitente comprador ou ao cessionário não intimado.
>
> **§ 2º** A alienação de bem sobre o qual tenha sido instituído direito de superfície, seja do solo, da plantação ou da construção, será ineficaz em relação ao concedente ou ao concessionário não intimado.
>
> **§ 3º** A alienação de direito aquisitivo de bem objeto de promessa de venda, de promessa de cessão ou de alienação fiduciária será ineficaz em relação ao promitente vendedor, ao promitente cedente ou ao proprietário fiduciário não intimado.
>
> **§ 4º** A alienação de imóvel sobre o qual tenha sido instituída enfiteuse, concessão de uso especial para fins de moradia ou concessão de direito real de uso será ineficaz em relação ao enfiteuta ou ao concessionário não intimado.
>
> **§ 5º** A alienação de direitos do enfiteuta, do concessionário de direito real de uso ou do concessionário de uso especial para fins de moradia será ineficaz em relação ao proprietário do respectivo imóvel não intimado.
>
> **§ 6º** A alienação de bem sobre o qual tenha sido instituído usufruto, uso ou habitação será ineficaz em relação ao titular desses direitos reais não intimado.

- 🔴🔴 **"Ineficaz" ≠ "nulo".** O art. 903, §1º separa **três** destinos: **invalidada** (preço vil ou
  outro vício), **ineficaz** (art. 804 — falta de intimação de titular de direito real) e **resolvida**
  (preço não pago). Na ineficácia **o bem continua arrematado**, mas o gravame **não é purgado**
  perante quem não foi intimado.
- ⭐ **Para o arrematante isso é PIOR que a nulidade:** ele fica com o imóvel **e com o gravame em
  cima**. Conferir se **todos** os credores com garantia registrada foram intimados é item obrigatório
  da due diligence — cruzar com `leitura-de-matricula`.
- 🔴 **O art. 889 NÃO lista o cônjuge do executado.** São **8 incisos fechados**. A intimação do cônjuge
  tem sede na disciplina da **penhora de imóvel**, não aqui. Material que diga *"o art. 889 exige
  intimação do cônjuge sob pena de nulidade"* cita o dispositivo errado (correção nº 5 do
  BUILD-CONTRACT).
- **Usa:** `intimacoes-art-889-e-ineficacia` ⭐ · `nulidades-de-intimacao-e-notificacao` ·
  `risco-de-anulacao-do-certame` · `leitura-de-matricula` · `anulatoria-de-arrematacao-judicial`.

---

## 9. Quem NÃO pode dar lance — art. 890 ✅

> **Art. 890.** Pode oferecer lance quem estiver na livre administração de seus bens, com exceção:
>
> I - dos tutores, dos curadores, dos testamenteiros, dos administradores ou dos liquidantes, quanto aos bens confiados à sua guarda e à sua responsabilidade;
>
> II - dos mandatários, quanto aos bens de cuja administração ou alienação estejam encarregados;
>
> III - do juiz, do membro do Ministério Público e da Defensoria Pública, do escrivão, do chefe de secretaria e dos demais servidores e auxiliares da justiça, em relação aos bens e direitos objeto de alienação na localidade onde servirem ou a que se estender a sua autoridade;
>
> IV - dos servidores públicos em geral, quanto aos bens ou aos direitos da pessoa jurídica a que servirem ou que estejam sob sua administração direta ou indireta;
>
> V - dos leiloeiros e seus prepostos, quanto aos bens de cuja venda estejam encarregados;
>
> VI - dos advogados de qualquer das partes.

- ⭐ **Inciso VI — o advogado de QUALQUER das partes não arremata.** Vale para o do exequente e para o
  do executado. Vedação frequentemente ignorada, e contamina a arrematação.
- **Inciso V** espelha o art. 3º da Res. CNJ 236/2016 (leiloeiro e prepostos não ofertam).
- **Usa:** `risco-de-anulacao-do-certame` · `anulatoria-de-arrematacao-judicial` ·
  `estrategia-de-lance-e-habilitacao`.

---

## 10. PREÇO VIL — art. 891 ✅ ⭐⭐ (régua em cascata)

> **Art. 891.** Não será aceito lance que ofereça preço vil.
>
> **Parágrafo único.** Considera-se vil o preço inferior ao mínimo estipulado pelo juiz e constante do edital, e, não tendo sido fixado preço mínimo, considera-se vil o preço inferior a cinquenta por cento do valor da avaliação.

🔴 **A régua é em CASCATA e o "50%" é SUPLETIVO:**

| Cenário | Piso do preço vil |
|---|---|
| Juiz **fixou** preço mínimo no edital (art. 885) | **O mínimo do edital** — vil é o que fica abaixo dele |
| Juiz **não fixou** preço mínimo | **50% da avaliação** (regra supletiva) |

**Três erros que o guard bloqueia:**

1. *"O CPC fixa 50%"* como regra geral — **não fixa**; 50% é supletivo.
2. *"O piso de 50% vale só para a 1ª praça"* — **o CPC não separa praças** na régua do preço vil. O que
   muda entre elas é o **preço de aceitação** da proposta parcelada (art. 895, I e II).
3. **Transportar os 50% do CPC para o extrajudicial** — lá a régua é **própria** (Lei 9.514, art. 27,
   §2º; Lei 14.711, art. 9º, §6º), e o "50%" é **faculdade do credor**, não piso de vileza. Ver
   `context/lei-9514-consolidada.md`.

⚠️ **Piso especial:** imóvel de **incapaz** tem régua própria de **80% do valor da avaliação** (art. 896, **caput** — seção 13 deste anexo).

- **Usa:** `preco-vil-como-tese` ⭐ · `mecanica-do-leilao-judicial` · `risco-de-anulacao-do-certame` ·
  `anulatoria-de-arrematacao-judicial`.

---

## 11. Pagamento, licitação e preferências — arts. 892 a 894 ✅

> **Art. 892.** Salvo pronunciamento judicial em sentido diverso, o pagamento deverá ser realizado de imediato pelo arrematante, por depósito judicial ou por meio eletrônico.
>
> **§ 1º** Se o exequente arrematar os bens e for o único credor, não estará obrigado a exibir o preço, mas, se o valor dos bens exceder ao seu crédito, depositará, dentro de 3 (três) dias, a diferença, sob pena de tornar-se sem efeito a arrematação, e, nesse caso, realizar-se-á novo leilão, à custa do exequente.
>
> **§ 2º** Se houver mais de um pretendente, proceder-se-á entre eles à licitação, e, no caso de igualdade de oferta, terá preferência o cônjuge, o companheiro, o descendente ou o ascendente do executado, nessa ordem.
>
> **§ 3º** No caso de leilão de bem tombado, a União, os Estados e os Municípios terão, nessa ordem, o direito de preferência na arrematação, em igualdade de oferta.

> **Art. 893.** Se o leilão for de diversos bens e houver mais de um lançador, terá preferência aquele que se propuser a arrematá-los todos, em conjunto, oferecendo, para os bens que não tiverem lance, preço igual ao da avaliação e, para os demais, preço igual ao do maior lance que, na tentativa de arrematação individualizada, tenha sido oferecido para eles.

> **Art. 894.** Quando o imóvel admitir cômoda divisão, o juiz, a requerimento do executado, ordenará a alienação judicial de parte dele, desde que suficiente para o pagamento do exequente e para a satisfação das despesas da execução.
>
> **§ 1º** Não havendo lançador, far-se-á a alienação do imóvel em sua integridade.
>
> **§ 2º** A alienação por partes deverá ser requerida a tempo de permitir a avaliação das glebas destacadas e sua inclusão no edital, e, nesse caso, caberá ao executado instruir o requerimento com planta e memorial descritivo subscritos por profissional habilitado.

- 🔴 **A preferência do 892, §2º só incide em IGUALDADE DE OFERTA.** Não é direito de cobrir o lance
  vencedor. **Não confundir** com o **direito de preferência do fiduciante** (Lei 9.514, art. 27,
  §2º-B), que é instituto distinto, em procedimento distinto — erro grave de cálculo e de tese.
- **Art. 894 é tese de redução do dano** pouco usada pelo executado: vender só a parte necessária.
  Exige planta e memorial descritivo e **tem de ser requerido a tempo de entrar no edital**.
- **Usa:** `mecanica-do-leilao-judicial` · `estrategia-de-lance-e-habilitacao` ·
  `adjudicacao-e-as-tres-remicoes`.

---

## 12. Arrematação PARCELADA — art. 895 ✅ ⭐ (a via alavancada, e seus três venenos)

> **Art. 895.** O interessado em adquirir o bem penhorado em prestações poderá apresentar, por escrito:
>
> I - até o início do primeiro leilão, proposta de aquisição do bem por valor não inferior ao da avaliação;
>
> II - até o início do segundo leilão, proposta de aquisição do bem por valor que não seja considerado vil.
>
> **§ 1º** A proposta conterá, em qualquer hipótese, oferta de pagamento de pelo menos vinte e cinco por cento do valor do lance à vista e o restante parcelado em até 30 (trinta) meses, garantido por caução idônea, quando se tratar de móveis, e por hipoteca do próprio bem, quando se tratar de imóveis.
>
> **§ 2º** As propostas para aquisição em prestações indicarão o prazo, a modalidade, o indexador de correção monetária e as condições de pagamento do saldo.
>
> **§ 3º** (VETADO).
>
> **§ 4º** No caso de atraso no pagamento de qualquer das prestações, incidirá multa de dez por cento sobre a soma da parcela inadimplida com as parcelas vincendas.
>
> **§ 5º** O inadimplemento autoriza o exequente a pedir a resolução da arrematação ou promover, em face do arrematante, a execução do valor devido, devendo ambos os pedidos ser formulados nos autos da execução em que se deu a arrematação.
>
> **§ 6º** A apresentação da proposta prevista neste artigo não suspende o leilão.
>
> **§ 7º** A proposta de pagamento do lance à vista sempre prevalecerá sobre as propostas de pagamento parcelado.
>
> **§ 8º** Havendo mais de uma proposta de pagamento parcelado:
>
> I - em diferentes condições, o juiz decidirá pela mais vantajosa, assim compreendida, sempre, a de maior valor;
>
> II - em iguais condições, o juiz decidirá pela formulada em primeiro lugar.
>
> **§ 9º** No caso de arrematação a prazo, os pagamentos feitos pelo arrematante pertencerão ao exequente até o limite de seu crédito, e os subsequentes, ao executado.

🔴 **Os três venenos que o investidor precisa ouvir antes de montar a operação:**

| § | O veneno |
|---|---|
| **§7º** | **Qualquer lance à vista SEMPRE prevalece** sobre a proposta parcelada — por menor que seja a diferença |
| **§6º** | A proposta **NÃO suspende o leilão** — ela não reserva o bem |
| **§4º** | Multa de 10% sobre a parcela inadimplida **SOMADA ÀS VINCENDAS** — não sobre a parcela isolada |

- **Estrutura:** mínimo **25% à vista** + saldo em até **30 meses**, garantido por **hipoteca do próprio
  imóvel** (imóveis) ou caução idônea (móveis).
- **A diferença entre praças aparece aqui:** no **1º** leilão a proposta tem de ser **≥ avaliação**
  (inciso I); no **2º**, basta **não ser vil** (inciso II).
- 🟡 **Ponto prático sem resposta na lei:** se a comissão do leiloeiro incide sobre o **lance total** ou
  sobre a **parcela à vista** — o CPC não diz (frente A, `needs-human`). Skill que precificar
  parcelamento marca *"conferir antes de protocolar"*.
- **Usa:** `arrematacao-parcelada-895` ⭐ · `custo-total-real-e-precificacao` ·
  `estrategia-de-lance-e-habilitacao`.

---

## 13. Imóvel de INCAPAZ — art. 896 ✅

> **Art. 896.** Quando o imóvel de incapaz não alcançar em leilão pelo menos oitenta por cento do valor da avaliação, o juiz o confiará à guarda e à administração de depositário idôneo, adiando a alienação por prazo não superior a 1 (um) ano.
>
> **§ 1º** Se, durante o adiamento, algum pretendente assegurar, mediante caução idônea, o preço da avaliação, o juiz ordenará a alienação em leilão.
>
> **§ 2º** Se o pretendente à arrematação se arrepender, o juiz impor-lhe-á multa de vinte por cento sobre o valor da avaliação, em benefício do incapaz, valendo a decisão como título executivo.
>
> **§ 3º** Sem prejuízo do disposto nos §§ 1º e 2º, o juiz poderá autorizar a locação do imóvel no prazo do adiamento.
>
> **§ 4º** Findo o prazo do adiamento, o imóvel será submetido a novo leilão.

- ⭐ **Piso próprio de 80% da avaliação** — não os 50% do art. 891. Arrematar imóvel de incapaz abaixo
  de 80% é **vício estrutural**, não questão de conveniência.
- O **§2º** pune o arrependimento do pretendente com multa de **20% da avaliação**, em benefício do
  incapaz, valendo a decisão como **título executivo**.
- **Usa:** `mecanica-do-leilao-judicial` · `risco-de-anulacao-do-certame` · `parecer-go-nogo-lote`.

---

## 14. Arrematante remisso, fiador e suspensão — arts. 897 a 900 ✅

> **Art. 897.** Se o arrematante ou seu fiador não pagar o preço no prazo estabelecido, o juiz impor-lhe-á, em favor do exequente, a perda da caução, voltando os bens a novo leilão, do qual não serão admitidos a participar o arrematante e o fiador remissos.

> **Art. 898.** O fiador do arrematante que pagar o valor do lance e a multa poderá requerer que a arrematação lhe seja transferida.

> **Art. 899.** Será suspensa a arrematação logo que o produto da alienação dos bens for suficiente para o pagamento do credor e para a satisfação das despesas da execução.

> **Art. 900.** O leilão prosseguirá no dia útil imediato, à mesma hora em que teve início, independentemente de novo edital, se for ultrapassado o horário de expediente forense.

- ⭐ **Não pagar não é "perder o sinal": é EXCLUSÃO.** O art. 897 impõe a perda da caução **e bane o
  arrematante e o fiador remissos do novo leilão daquele bem**.
- **Usa:** `estrategia-de-lance-e-habilitacao` · `custo-total-real-e-precificacao` ·
  `invalidacao-embargos-e-desistencia-903`.

---

## 15. Auto de arrematação e CARTA — art. 901 ✅ ⭐

> **Art. 901.** A arrematação constará de auto que será lavrado de imediato e poderá abranger bens penhorados em mais de uma execução, nele mencionadas as condições nas quais foi alienado o bem.
>
> **§ 1º** A ordem de entrega do bem móvel ou a carta de arrematação do bem imóvel, com o respectivo mandado de imissão na posse, será expedida depois de efetuado o depósito ou prestadas as garantias pelo arrematante, bem como realizado o pagamento da comissão do leiloeiro e das demais despesas da execução.
>
> **§ 2º** A carta de arrematação conterá a descrição do imóvel, com remissão à sua matrícula ou individuação e aos seus registros, a cópia do auto de arrematação e a prova de pagamento do imposto de transmissão, além da indicação da existência de eventual ônus real ou gravame.

- ⭐ **O §1º é a prova textual de que comissão e despesas NÃO estão dentro do lance** — são pagamento
  adicional e **condição para a carta sair**. A sequência trava aqui: sem depósito + comissão +
  despesas, **não há carta nem mandado de imissão**.
- ⭐ **O §2º inverte a sequência tributária:** a carta contém a **prova de pagamento do ITBI** — ou
  seja, **o ITBI é pago ANTES do título**, não depois do registro.
- **O §2º também exige que a carta INDIQUE ônus real ou gravame remanescente.** Carta que silencia
  sobre gravame conhecido é documento defeituoso.
- 🔴 **Assimetria de desocupação, contra o judicial:** aqui **não há prazo nem qualificação liminar**, e
  o mandado só sai depois de pagos preço, comissão, despesas e ITBI. No extrajudicial, a Lei 9.514,
  art. 30 dá **liminar expressa + 60 dias**. Ver `context/lei-9514-consolidada.md`.
- **Usa:** `arrematacao-auto-e-carta` · `imissao-na-posse-do-arrematante` ⭐ ·
  `registro-regularizacao-e-itbi` · `custo-total-real-e-precificacao`.

---

## 16. As TRÊS remições — arts. 826, 877 §3º e 902 ✅ ⭐ (não podem ser confundidas)

> **Art. 902.** No caso de leilão de bem hipotecado, o executado poderá remi-lo até a assinatura do auto de arrematação, oferecendo preço igual ao do maior lance oferecido.
>
> **Parágrafo único.** No caso de falência ou insolvência do devedor hipotecário, o direito de remição previsto no caput defere-se à massa ou aos credores em concurso, não podendo o exequente recusar o preço da avaliação do imóvel.

> **Art. 826.** Antes de adjudicados ou alienados os bens, o executado pode, a todo tempo, remir a execução, pagando ou consignando a importância atualizada da dívida, acrescida de juros, custas e honorários advocatícios.
>
> Seção II
>
> Da Citação do Devedor e do Arresto

| Remição | Dispositivo | Até quando | Quanto se paga |
|---|---|---|---|
| **Da execução** | **art. 826** | A todo tempo, **antes** de adjudicados ou alienados os bens | A **dívida atualizada** + juros, custas e honorários |
| **Do bem hipotecado (leilão)** | **art. 902** | Até a **assinatura do auto de arrematação** | Preço **igual ao maior lance** oferecido |
| **Na adjudicação** | **art. 877, §3º** | Até a assinatura do **auto de adjudicação** | **Avaliação** se não houve licitantes; senão, o **maior lance** |

- 🔴 **Marcos temporais e valores DIFERENTES.** Misturá-los erra o cálculo e a via.
- ⭐ **Consequência que o mercado esquece:** o leiloeiro **faz jus à comissão** quando o acordo ou a
  remição são **posteriores à alienação** (Res. CNJ 236/2016, **art. 7º, §3º**). Ver
  `context/resolucao-cnj-236-2016.md` e `context/jurisprudencia-leiloes.md`.
- **Usa:** `adjudicacao-e-as-tres-remicoes` ⭐ · `leiloeiro-comissao-e-prestacao-de-contas` ·
  `defesa-fiduciante-consolidacao-e-purga` (para contrastar com a **purga** do extrajudicial, que é
  instituto diverso).

---

## 17. Art. 903 — O RELÓGIO DO ARREMATANTE ✅ ⭐⭐ (o dispositivo mais importante do anexo)

> **Art. 903.** Qualquer que seja a modalidade de leilão, assinado o auto pelo juiz, pelo arrematante e pelo leiloeiro, a arrematação será considerada perfeita, acabada e irretratável, ainda que venham a ser julgados procedentes os embargos do executado ou a ação autônoma de que trata o § 4º deste artigo, assegurada a possibilidade de reparação pelos prejuízos sofridos.
>
> **§ 1º** Ressalvadas outras situações previstas neste Código, a arrematação poderá, no entanto, ser:
>
> I - invalidada, quando realizada por preço vil ou com outro vício;
>
> II - considerada ineficaz, se não observado o disposto no art. 804;
>
> III - resolvida, se não for pago o preço ou se não for prestada a caução.
>
> **§ 2º** O juiz decidirá acerca das situações referidas no § 1º, se for provocado em até 10 (dez) dias após o aperfeiçoamento da arrematação.
>
> **§ 3º** Passado o prazo previsto no § 2º sem que tenha havido alegação de qualquer das situações previstas no § 1º, será expedida a carta de arrematação e, conforme o caso, a ordem de entrega ou mandado de imissão na posse.
>
> **§ 4º** Após a expedição da carta de arrematação ou da ordem de entrega, a invalidação da arrematação poderá ser pleiteada por ação autônoma, em cujo processo o arrematante figurará como litisconsorte necessário.
>
> **§ 5º** O arrematante poderá desistir da arrematação, sendo-lhe imediatamente devolvido o depósito que tiver feito:
>
> I - se provar, nos 10 (dez) dias seguintes, a existência de ônus real ou gravame não mencionado no edital;
>
> II - se, antes de expedida a carta de arrematação ou a ordem de entrega, o executado alegar alguma das situações previstas no § 1º ;
>
> III - uma vez citado para responder a ação autônoma de que trata o § 4º deste artigo, desde que apresente a desistência no prazo de que dispõe para responder a essa ação.
>
> **§ 6º** Considera-se ato atentatório à dignidade da justiça a suscitação infundada de vício com o objetivo de ensejar a desistência do arrematante, devendo o suscitante ser condenado, sem prejuízo da responsabilidade por perdas e danos, ao pagamento de multa, a ser fixada pelo juiz e devida ao exequente, em montante não superior a vinte por cento do valor atualizado do bem.

### 17.1 A linha do tempo (é ela que decide a via — e é irreversível)

| Momento | O que já aconteceu | Quem ataca, e como |
|---|---|---|
| **Antes** da assinatura do auto | Nada é definitivo | Impugnação livre nos autos; remição (826/902) ainda possível |
| **Assinado o auto** | Arrematação **perfeita, acabada e irretratável** (caput) | Só as **3 hipóteses do §1º**, provocadas em **10 dias** (§2º) |
| **Passados os 10 dias** sem alegação | Expede-se **carta + mandado de imissão** (§3º) | A via nos autos **se fecha** |
| **Após a carta** / ordem de entrega | Título formado | Só **ação autônoma** (§4º), com o arrematante como **litisconsorte necessário** |

### 17.2 As TRÊS portas de saída do arrematante (§5º) — cada uma com gatilho próprio

| Inciso | Gatilho | Prazo |
|---|---|---|
| **I** ⭐ | Ônus real ou gravame **não mencionado no edital** (viola o **886, VI**) | Provar nos **10 dias** seguintes |
| **II** | O **executado** alega vício do §1º | Antes de expedida a carta |
| **III** | Arrematante **citado** na ação autônoma do §4º | No prazo de resposta |

### 17.3 Os três cuidados que o plugin repete

1. 🔴 **A irretratabilidade é forte, mas não é absoluta.** O caput mantém a arrematação **ainda que
   procedentes** os embargos ou a ação autônoma, resolvendo-se em **reparação** — isso protege o
   arrematante de boa-fé. Mas o §1º ressalva "outras situações previstas neste Código" e admite
   invalidação. **Afirmar "arrematação nunca cai" é erro; afirmar "cai como qualquer negócio" também.**
2. ⭐⭐ **Os 10 dias do §2º correm do APERFEIÇOAMENTO — a assinatura do auto —, não da ciência do
   vício.** É por isso que o **gate de due diligence é PRÉ-lance**: due diligence feita depois do lance
   chega tarde **por construção da lei**, não por pedagogia.
3. ⭐ **O §6º é a arma CONTRA quem alega de má-fé.** Suscitar vício infundado para forçar a desistência
   do arrematante é **ato atentatório à dignidade da justiça**, com multa de até **20% do valor atualizado do bem**. Limita a estratégia de "alegar qualquer coisa para desfazer o negócio" — e é
   ressalva obrigatória nas skills de defesa.

- **Usa:** `invalidacao-embargos-e-desistencia-903` ⭐ · `anulatoria-de-arrematacao-judicial` ·
  `triagem-leiloes` (a **fase** decide a via) · `suprema-corte-leiloes` (R3) · `parecer-go-nogo-lote`.

---

## 18. Créditos propter rem sub-rogam-se no PREÇO — art. 908, §1º ✅ ⭐

> **Art. 908.** Havendo pluralidade de credores ou exequentes, o dinheiro lhes será distribuído e entregue consoante a ordem das respectivas preferências.
>
> **§ 1º** No caso de adjudicação ou alienação, os créditos que recaem sobre o bem, inclusive os de natureza propter rem, sub-rogam-se sobre o respectivo preço, observada a ordem de preferência.
>
> **§ 2º** Não havendo título legal à preferência, o dinheiro será distribuído entre os concorrentes, observando-se a anterioridade de cada penhora.

- ⭐ **É a âncora legal da tese do arrematante contra débito anterior:** o crédito com preferência
  (inclusive o **propter rem**) **sub-roga-se sobre o preço**, no concurso — não persegue o bem nas
  mãos de quem arrematou. No **tributário**, isso está fechado a favor do arrematante (**CTN 130,
  §único** + **Tema 1.134/STJ**).
- 🟡🔴 **No CONDOMINIAL a leitura NÃO é livre.** Ver `context/jurisprudencia-leiloes.md`: quando o
  **edital INFORMA** a dívida condominial, a orientação está **consolidada** contra o arrematante
  (2ª Seção, unânime) — **é proibido escrever "a matéria está em aberto no STJ"**. A leitura *a
  contrario* do 908, §1º só serve para o **edital OMISSO**, como **tese de defesa bem fundamentada**,
  jamais como regra pacífica.
- **Usa:** `debitos-propter-rem` ⭐ · `debitos-e-creditos-pos-arrematacao` · `analise-de-edital` ·
  `custo-total-real-e-precificacao`.

---

## 19. Contagem do prazo — art. 219 ✅ (com a ressalva honesta)

> **Art. 219.** Na contagem de prazo em dias, estabelecido por lei ou pelo juiz, computar-se-ão somente os dias úteis.
>
> **Parágrafo único.** O disposto neste artigo aplica-se somente aos prazos processuais.

- **O que decide:** prazo **processual** conta em **dias úteis**. É a leitura natural para os **10 dias
  do art. 903, §2º**.
- 🟡 **Ressalva obrigatória:** a contagem dos 10 dias do 903, §2º (úteis × corridos) e o *dies a quo*
  exato **não foram confirmados em jurisprudência** (frente A, `needs-human`). Skill que calcular esse
  prazo escreve *"🟡 conferir o inteiro teor antes de protocolar"* e roteia para `validador-leiloes`.
- 🔴 **Não migrar o art. 219 para o EXTRAJUDICIAL.** Os prazos da Lei 9.514 e da Lei 14.711 (15 / 60 /
  15 / 30 / 180 dias) são de **direito material e procedimento cartorário**, não prazos processuais —
  o art. 219 **não** os converte em dias úteis. Mesmo raciocínio para os **90 dias do art. 8º da Lei
  8.245** (denúncia da locação).
- **Usa:** `suprema-corte-leiloes` (R3) · `triagem-leiloes` · `invalidacao-embargos-e-desistencia-903` ·
  `memoria-de-caso-leilao`.

---

## 20. GUARD — o que este anexo proíbe

1. Citar dispositivo do CPC **sem grep neste anexo**. Número de cabeça reprova no `validador-leiloes`.
2. Escrever que **"o CPC fixa 5% de comissão"** (art. 884, §único **não fixa percentual**).
3. Escrever que **"o CPC fixa 50%"** como regra geral de preço vil (é **supletivo** — art. 891, §único).
4. Afirmar que o **art. 889 exige intimação do cônjuge** (são 8 incisos fechados e ele não está lá).
5. Chamar de **nulidade** a falta de intimação de titular de direito real (é **ineficácia** — art. 804
   c/c 903, §1º, II).
6. Transportar a régua de preço vil do CPC para o **extrajudicial** (lá a régua é própria).
7. Contar os **10 dias do art. 903, §2º** a partir da **ciência do vício** (correm do
   **aperfeiçoamento**).
8. Opinar sobre lance sem o **gate de due diligence** completo — o motivo é o **art. 903, §2º**.

Toda peça fecha por **`suprema-corte-leiloes`** (R1-R4) **+ `validador-leiloes`**.

---

## Fonte e verificação

- **CPC — texto compilado:** `https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2015/lei/l13105.htm`
  — capturado em **2026-08-02**, transcrição verbatim por script.
- **Vigência:** varredura na captura confirmou **zero** notas de alteração/revogação na faixa
  **arts. 876 a 908**.
- **Anexos irmãos:** `context/resolucao-cnj-236-2016.md` (o regulamento do art. 882, §1º) ·
  `context/lei-9514-consolidada.md` e `context/lei-14711-2023.md` (o extrajudicial) ·
  `context/jurisprudencia-leiloes.md` · `context/clausulas-armadilha-de-edital.md` ·
  `context/custo-total-do-arrematante.md`.
