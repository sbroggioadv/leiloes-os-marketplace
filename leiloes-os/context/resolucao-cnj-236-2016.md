# Anexo — Resolução CNJ 236/2016 (os 36 artigos) + ficha oficial do ato

> **Anexo de legislação do `leiloes-os`.** É o **regulamento do art. 882, §1º, do CPC** — a norma que
> credencia leiloeiros, fixa o **piso de 5%** da comissão e disciplina a mecânica do pregão eletrônico
> (prorrogação de 3 min, vedação de lance por e-mail, rastreamento de IP). Sem ela, metade das
> respostas sobre leilão judicial eletrônico sai errada.
>
> **Legenda:** ✅ conferido verbatim na fonte oficial · 🟡 não confirmado · 🔴 verdade dura ·
> ⭐ eixo do domínio.

---

## ⚠️ AVISO 1 — grep o artigo e leia a faixa. NUNCA despeje o anexo inteiro

Consulta pontual, não leitura de contexto. **`grep` do número do artigo e leia só a faixa.**

## ⚠️ AVISO 2 — PROVENIÊNCIA: de onde veio este texto, e por que NÃO veio do PDF 🔴

A frente A cita como fonte o **PDF oficial** em
`https://atos.cnj.jus.br/files/resolucao_236_13072016_15072016155240.pdf`.

**Esse PDF é um DOCUMENTO ESCANEADO e não tem camada de texto.** Verificado na captura de
**2026-08-02**: `Creator: PFU ScanSnap Manager`, `Producer: Adobe PDF Scan Library`, **zero fontes
embutidas**, e `pdftotext` devolve **0 byte** nas 12 páginas. Ou seja: **é impossível transcrever a
Resolução verbatim a partir daquele PDF** sem OCR — e OCR introduziria erro justamente onde o plugin
não pode errar (números de artigo, percentuais, prazos).

**A transcrição abaixo foi extraída da própria página oficial do ato**, no mesmo domínio do CNJ —
`https://atos.cnj.jus.br/atos/detalhar/2313` —, que **renderiza o inteiro teor no HTML** (server-side).
Conferência feita: os **36 artigos** aparecem, **cada um exatamente uma vez** (não há concatenação de
duas versões na página). O PDF escaneado permanece como **fac-símile de conferência visual**; a fonte
**textual** é a página do ato.

## ⚠️ AVISO 3 — vigência: "Vigente", com o campo **Alteração VAZIO** ✅

A ficha oficial do ato foi lida na captura. **Campo `Alteração`: em branco** — a Resolução **nunca foi
alterada** desde 2016. É o que autoriza citá-la direto, sem checar redação sucessiva. **Reconferir a
ficha antes de publicar** é item do gate de calendário.

---

## 0. FICHA OFICIAL DO ATO (verbatim dos campos) ✅

| Campo | Conteúdo |
|---|---|
| **Identificação** | Resolução Nº 236 de 13/07/2016 |
| **Ementa** | "Regulamenta, no âmbito do Poder Judiciário, procedimentos relativos à alienação judicial por meio eletrônico, na forma preconizada pelo art. 882, § 1º, do novo Código de Processo Civil (Lei 13.105/2015)." |
| **Situação** | ✅ **Vigente** |
| **Situação STF** | --- |
| **Origem** | Presidência |
| **Fonte** | DJe/CNJ, nº 121, de 15/07/2016, p. 2-5. |
| **Alteração** | ⭐ **(vazio — nenhuma alteração registrada)** |
| **Legislação Correlata** | CPC (Lei 13.105/2015) · CLT art. 888, §3º · Resolução nº 198 |
| **Vigência** | 90 dias após a publicação (art. 36) → em vigor desde **13/10/2016** |
| **Assinatura** | Ministro Ricardo Lewandowski |

> 🟡 **Divergência interna da fonte, sem impacto no domínio:** a *Legislação Correlata* da ficha grafa
> "Resolução nº 198, de 1º de **julho** de 2014", enquanto o **CONSIDERANDO** do próprio texto grafa
> "Resolução CNJ 198, de 1º de **setembro** de 2014". Registrado por honestidade de captura; a Res. 198
> é norma de **gestão estratégica** e não é citada em peça deste plugin.

---

# CAPÍTULO I — Seção I: Dos Leiloeiros Judiciais e Corretores

## Art. 1º — credencia-se o LEILOEIRO, não a plataforma ✅ ⭐

> **Art. 1º** Os leilões judiciais serão realizados exclusivamente por leiloeiros credenciados perante o órgão judiciário, conforme norma local (art. 880, caput e § 3º), e deverão atender aos requisitos da ampla publicidade, autenticidade e segurança, com observância das regras estabelecidas na legislação sobre certificação digital.
>
> **Parágrafo único.** As alienações particulares poderão ser realizadas por corretor ou leiloeiro público, conforme valor mínimo fixado pelo juiz.

- 🔴 **Credencia-se o leiloeiro PESSOA FÍSICA.** A "plataforma" é atividade-meio do leiloeiro
  matriculado na Junta (IN DREI 52/2022, art. 60). **Due diligence se faz por nome + matrícula**,
  cruzando a lista do tribunal com a da Junta Comercial. **Procurar "a empresa" na Junta não devolve
  nada.** Ver `context/leiloeiro-decreto-21981-in-drei-52.md`.
- **Usa:** `estrategia-de-lance-e-habilitacao` · `leiloeiro-responsabilidade-e-regularidade` ·
  `risco-de-anulacao-do-certame`.

## Art. 2º — 3 anos de exercício e a vedação societária ✅

> **Art. 2º** Caberá ao juiz a designação (art. 883), constituindo requisito mínimo para o credenciamento de leiloeiros públicos e corretores o exercício profissional por não menos que 3 (três) anos, sem prejuízo de disposições complementares editadas pelos tribunais (art. 880, § 3º).
>
> **§ 1º** O leiloeiro público, por ocasião do credenciamento, deverá apresentar declaração de que:
>
> I - dispõe de propriedade, ou por contrato de locação com vigência durante o período de validade do cadastramento, de imóvel destinado à guarda e à conservação dos bens removidos, com informações sobre a área e endereço atualizado completo (logradouro, número, bairro, município e código de endereçamento postal), no qual deverá ser mantido atendimento ao público;
>
> II - possui sistema informatizado para controle dos bens removidos, com fotos e especificações, para consulta on-line pelo Tribunal, assim como de que dispõe de equipamentos de gravação ou filmagem do ato público de venda judicial dos bens ou contrato com terceiros que possuam tais equipamentos;
>
> III - possui condições para ampla divulgação da alienação judicial, com a utilização dos meios possíveis de comunicação, especialmente publicação em jornais de grande circulação, rede mundial de computadores e material de divulgação impresso;
>
> IV - possui infraestrutura para a realização de leilões judiciais eletrônicos, bem como de que adota medidas reconhecidas pelas melhores práticas do mercado de tecnologia da informação para garantir a privacidade, a confidencialidade, a disponibilidade e a segurança das informações de seus sistemas informatizados, submetida à homologação pelo Tribunal respectivo;
>
> V - não possui relação societária com outro leiloeiro público ou corretor credenciado.
>
> **§ 2º** Os tribunais poderão criar Comissões Provisórias de Credenciamento de Leiloeiros para definição e análise do cumprimento das disposições editalícias e normativas, em especial os requisitos tecnológicos mencionados neste dispositivo.

- **§1º, V é critério de impugnação pouco usado:** o leiloeiro declara **não possuir relação societária
  com outro leiloeiro público ou corretor credenciado**. Relação societária cruzada entre credenciados
  é vício de credenciamento.
- Os **3 anos** espelham o art. 880, §3º, do CPC — ver `context/cpc-leilao-879-903.md`.
- **Usa:** `leiloeiro-responsabilidade-e-regularidade` · `risco-de-anulacao-do-certame`.

## Arts. 3º e 4º — impedimentos e descredenciamento ✅

> **Art. 3º** Na forma dos impedimentos elencados no art. 890 e incisos do Código de Processo Civil, os leiloeiros públicos, assim como seus respectivos prepostos, não poderão oferecer lances quanto aos bens de cuja venda estejam encarregados.

> **Art. 4º** O credenciamento de novos leiloeiros e corretores públicos será realizado por meio de requerimento dos interessados, conforme procedimento definido pelo Tribunal correspondente.
>
> **Parágrafo único.** O descredenciamento de leiloeiros públicos e corretores ocorrerá a qualquer tempo, a pedido da parte interessada ou pelo descumprimento de dispositivos desta Resolução, mediante ampla defesa e contraditório.
>
> Seção II
>
> Das Responsabilidades

- **Art. 3º espelha o art. 890, V, do CPC** (leiloeiro e prepostos não ofertam lance). O Decreto
  21.981/32, art. 36 trata a autocompra com **multa**, não destituição — ver o anexo do leiloeiro.
- **Usa:** `leiloeiro-responsabilidade-e-regularidade` · `anulatoria-de-arrematacao-judicial`.

---

# CAPÍTULO I — Seção II: Das Responsabilidades

## Art. 5º — o termo de credenciamento e os deveres de divulgação ✅

> **Art. 5º** Mediante a celebração do Termo de Credenciamento e Compromisso, em modelo aprovado pelo órgão jurisdicional, o leiloeiro público assumirá, além das obrigações definidas em lei, as seguintes responsabilidades:
>
> I - remoção dos bens penhorados, arrestados ou sequestrados, em poder do executado ou de terceiro, para depósito sob sua responsabilidade, assim como a guarda e a conservação dos referidos bens, na condição de depositário judicial, mediante nomeação pelo juízo competente, independentemente da realização pelo leiloeiro público depositário do leilão do referido bem;
>
> II - divulgação do edital dos leilões de forma ampla ao público em geral, por meio de material impresso, mala direta, publicações em jornais e na rede mundial de computadores, inclusive com imagens reais dos bens nesse canal de comunicação, para melhor aferição de suas características e de seu estado de conservação;
>
> III - exposição dos bens sob sua guarda, mantendo atendimento ao público em imóvel destinado aos bens removidos no horário ininterrupto das 8h às 18h, nos dias úteis, ou por meio de serviço de agendamento de visitas;
>
> IV - responder ou justificar sua impossibilidade, de imediato, a todas as indagações formuladas pelo juízo da execução;
>
> V - comparecer ao local da hasta pública com antecedência necessária ao planejamento das atividades;
>
> VI - comprovar, documentalmente, as despesas decorrentes de remoção, guarda e conservação dos bens;
>
> VII - excluir bens da hasta pública sempre que assim determinar o juízo da execução;
>
> VIII - comunicar, imediatamente, ao juízo da execução, qualquer dano, avaria ou deterioração do bem removido;
>
> IX - comparecer ou nomear preposto igualmente credenciado para participar de reuniões convocadas pelos órgãos judiciais onde atuam ou perante o Tribunal correspondente;
>
> X - manter seus dados cadastrais atualizados;
>
> XI - criar e manter, na rede mundial de computadores, endereço eletrônico e ambiente web para viabilizar a realização de alienação judicial eletrônica e divulgar as imagens dos bens ofertados.

- ⭐ **O inciso II obriga divulgação AMPLA** (impresso, mala direta, jornal, internet, **com imagens
  reais dos bens**). Leilão anunciado só na página do leiloeiro, sem as imagens, é matéria de
  impugnação de publicidade — cruzar com o **art. 887 do CPC**.
- **Usa:** `risco-de-anulacao-do-certame` · `analise-de-edital` · `leiloeiro-responsabilidade-e-regularidade`.

## Art. 6º ✅

> **Art. 6º** O leiloeiro público deverá comunicar ao juízo, com antecedência, a impossibilidade de promover a alienação judicial por meio eletrônico, a fim de que a autoridade possa designar, se for o caso, servidor para a realização do leilão.
>
> **§ 1º** Na hipótese do caput, remanescerá ao leiloeiro público a obrigação de disponibilizar equipe e estrutura de apoio para a realização da modalidade eletrônica do leilão, sob pena de descredenciamento sumário, observados o direito à ampla defesa e ao contraditório.
>
> **§ 2º** A ausência do leiloeiro oficial público deverá ser justificada documentalmente no prazo máximo e improrrogável de 5 (cinco) dias após a realização do leilão, sob pena de descredenciamento, cabendo ao juízo da execução, conforme o caso, por decisão fundamentada, aceitar ou não a justificativa.

## Art. 7º — A COMISSÃO ✅ ⭐⭐ (o artigo mais citado do anexo)

> **Art. 7º** Além da comissão sobre o valor de arrematação, a ser fixada pelo magistrado (art. 884, parágrafo único), no mínimo de 5% (cinco por cento) sobre o valor da arrematação (art. 24, parágrafo único, do Decreto 21.981/1932), a cargo do arrematante, fará jus o leiloeiro público ao ressarcimento das despesas com a remoção, guarda e conservação dos bens, desde que documentalmente comprovadas, na forma da lei.
>
> **§ 1º** Não será devida a comissão ao leiloeiro público na hipótese da desistência de que trata o art. 775 do Código de Processo Civil, de anulação da arrematação ou de resultado negativo da hasta pública.
>
> **§ 2º** Anulada ou verificada a ineficácia da arrematação ou ocorrendo a desistência prevista no art. 775 do Código de Processo Civil, o leiloeiro público e o corretor devolverão ao arrematante o valor recebido a título de comissão, corrigido pelos índices aplicáveis aos créditos respectivos.
>
> **§ 3º** Na hipótese de acordo ou remição após a realização da alienação, o leiloeiro e o corretor público farão jus à comissão prevista no caput.
>
> **§ 4º** Se o valor de arrematação for superior ao crédito do exequente, a comissão do leiloeiro público, bem como as despesas com remoção e guarda dos bens, poderá ser deduzida do produto da arrematação.
>
> **§ 5º** Os leiloeiros públicos credenciados poderão ser nomeados pelo juízo da execução para remover bens e atuar como depositário judicial.
>
> **§ 6º** A recusa injustificada à ordem do juízo da execução para remoção do bem deverá ser imediatamente comunicada ao Tribunal para análise de eventual descredenciamento.
>
> **§ 7º** O executado ressarcirá as despesas previstas no caput, inclusive se, depois da remoção, sobrevier substituição da penhora, conciliação, pagamento, remição ou adjudicação.

🔴 **O que este artigo decide, literalmente:**

| Ponto | O texto diz | O erro que o guard bloqueia |
|---|---|---|
| Percentual | "**no mínimo** de 5% (cinco por cento)" | Dizer que **o CPC** fixa 5% — o CPC **não fixa** (art. 884, §único). A fonte é esta Resolução + Decreto 21.981/32 |
| Quem arbitra | "a ser **fixada pelo magistrado** (art. 884, §único)" | Tratar os 5% como teto |
| Quem paga | "**a cargo do arrematante**" | Supor que sai do lance — **soma-se** a ele |

⭐⭐ **5% é PISO, não teto — e não existe teto** (ADENDO E1 do BUILD-CONTRACT). O texto do caput é
literal: "**no mínimo**". **7% em leilão JUDICIAL é lícito** (arbitramento do juiz, CPC 884, §único +
este art. 7º). O eixo de ataque do arrematante é **temporal**: impugnar o percentual **ANTES do
lance** — não impugnado e pago, consolida-se. Resíduos obrigatórios na skill: (a) não há ato do DREI
dizendo isso expressamente — risco disciplinar formal não zerado; (b) **no EXTRAJUDICIAL da 9.514 o
raciocínio NÃO se transporta** (não há juiz arbitrando); (c) os precedentes são de **turma**, não
repetitivos. Ver `context/jurisprudencia-leiloes.md`.

**A tabela de quando a comissão é ou não devida — direto dos §§:**

| Situação | Comissão | § |
|---|---|---|
| Desistência do art. 775 do CPC · anulação · **leilão negativo** | ❌ **Não devida** | §1º |
| Anulada / ineficaz / desistida **depois de paga** | ❌ **Devolvida corrigida** ao arrematante | §2º |
| ⭐ **Acordo ou remição APÓS a alienação** | ✅ **Devida** | §3º |
| Arrematação > crédito do exequente | ✅ Pode ser **deduzida do produto** | §4º |
| Remoção e guarda (depois de substituição de penhora, conciliação, pagamento, remição, adjudicação) | ✅ **Executado ressarce** | §7º |

⭐ **O §3º é a armadilha do executado que "acordou depois do leilão":** acordo ou remição **posteriores
à alienação NÃO afastam a comissão**. Confirmado em julgado de turma — ver
`context/jurisprudencia-leiloes.md`.

- **Usa:** `leiloeiro-comissao-e-prestacao-de-contas` ⭐ · `custo-total-real-e-precificacao` ⭐ ·
  `analise-de-edital` · `adjudicacao-e-as-tres-remicoes` · `agravo-de-instrumento-leiloes`.

## Art. 8º ✅

> **Art. 8º** O juízo da execução deverá priorizar os bens removidos na ordem de designação do leilão, assim como o ressarcimento das despesas com a remoção e guarda, observados os privilégios legais.
>
> Seção III
>
> Da Nomeação dos Leiloeiros Públicos

---

# CAPÍTULO I — Seção III: Da Nomeação dos Leiloeiros Públicos

## Arts. 9º e 10 — indicação, sorteio e a competência dos tribunais ✅

> **Art. 9º** Os leiloeiros públicos credenciados poderão ser indicados pelo exequente, cuja designação deverá ser realizada pelo juiz, na forma do art. 883, ou por sorteio na ausência de indicação, inclusive na modalidade eletrônica, conforme regras objetivas a serem estabelecidas pelos tribunais.
>
> **§ 1º** O desenvolvimento de ferramenta eletrônica para realização de sorteio dos leiloeiros públicos ficará a cargo de cada Tribunal.
>
> **§ 2º** As designações diretas ou por sorteio devem ser feitas de modo equitativo, observadas a impessoalidade, a capacidade técnica do leiloeiro público e a participação em certames anteriores.
>
> **§ 3º** Nas ações trabalhistas, o leiloeiro será nomeado nos termos do art. 888, § 3º, da Consolidação das Leis do Trabalho.

> **Art. 10.** Os tribunais brasileiros ficam autorizados a editar disposições complementares sobre o procedimento de alienação judicial e dispor sobre o credenciamento dos leiloeiros públicos de que trata o art. 880, § 3º, do Código de Processo Civil, observadas as regras desta Resolução e ressalvada a competência das unidades judiciárias para decidir questões jurisdicionais.
>
> **Parágrafo único.** Os leilões eletrônicos deverão ser realizados por leiloeiro credenciado e nomeado na forma desta Resolução ou, onde não houver leiloeiro público, pelo próprio Tribunal (art. 881, § 1º).

- **Três vias de nomeação:** indicação pelo **exequente** · designação pelo **juiz** (art. 883) ·
  **sorteio** na ausência de indicação.
- 🔴 **A escala de antiguidade NÃO se aplica ao leilão judicial** (Dec. 21.981/32, art. 43 + IN DREI 52,
  art. 71, §3º — ela vale só nas vendas de bens da União/Estados/Municípios). **Impugnar nomeação em
  execução cível por "quebra de antiguidade" é tese perdida.**
- 🟡 **O art. 10 delega aos tribunais.** Cada TJ/TRT tem regulamento próprio (prazos, sorteio,
  percentual arbitrado) — **não levantados**. Skill que afirmar regra local marca *"conferir a norma do
  tribunal antes de protocolar"*.
- **Usa:** `leiloeiro-responsabilidade-e-regularidade` · `estrategia-de-lance-e-habilitacao` ·
  `risco-de-anulacao-do-certame`.

## Art. 11 — abertura do sistema e o leilão SIMULTÂNEO ✅

> **Art. 11.** A modalidade eletrônica de leilão judicial será aberta para recepção de lances com, no mínimo, 5 (cinco) dias (art. 887, § 1º) de antecedência da data designada para o início do período em que se realizará o leilão (art. 886, IV), observado o disposto no art. 889, parágrafo único, do Código de Processo Civil.
>
> **Parágrafo único.** O leilão poderá ser simultâneo (eletrônico e presencial), cujo endereço será indicado no edital e a modalidade presencial se dará no último dia do período designado para o leilão eletrônico.

- 🔴 **Os "5 dias" daqui são a ABERTURA DO SISTEMA PARA LANCES** — não confundir com os 5 dias de
  **publicação do edital** (CPC 887, §1º) nem com os 5 dias de **cientificação** do CPC 889.
- ⭐ **No simultâneo, o presencial ocorre no ÚLTIMO DIA** do período eletrônico — e é isso que muda a
  janela de prorrogação de 3 min para **15 segundos** (art. 21).
- **Usa:** `estrategia-de-lance-e-habilitacao` ⭐ · `mecanica-do-leilao-judicial` · `analise-de-edital`.

---

# CAPÍTULO II — DO LEILÃO ELETRÔNICO

## Arts. 12 a 15 — cadastramento prévio, gratuito e INDISPENSÁVEL ✅

> **Art. 12.** O usuário interessado em participar da alienação judicial eletrônica, por meio da rede mundial de computadores, deverá se cadastrar previamente no site respectivo, ressalvada a competência do juízo da execução para decidir sobre eventuais impedimentos.

> **Art. 13.** O cadastramento será gratuito e constituirá requisito indispensável para a participação na alienação judicial eletrônica, responsabilizando-se o usuário, civil e criminalmente, pelas informações lançadas por ocasião do cadastramento.
>
> **Parágrafo único.** O cadastramento implicará na aceitação da integralidade das disposições desta Resolução, assim como das demais condições estipuladas no edital respectivo.

> **Art. 14.** Caberá ao leiloeiro do sistema de alienação judicial eletrônica (as próprias unidades judiciais ou as entidades credenciadas) a definição dos critérios de participação na alienação judicial eletrônica com o objetivo de preservar a segurança e a confiabilidade dos lances.
>
> **§ 1º** O cadastro de licitantes deverá ser eletrônico e sujeito à conferência de identidade em banco de dados oficial.
>
> **§ 2º** Até o dia anterior ao leilão, o leiloeiro estará disponível para prestar aos interessados os esclarecimentos de quaisquer dúvidas sobre o funcionamento do leilão.
>
> **§ 3º** O leiloeiro deverá manter telefones disponíveis em seção facilmente visível em seu site na rede mundial de computadores para dirimir eventuais dúvidas referentes às transações efetuadas durante e depois do leilão judicial eletrônico.

> **Art. 15.** O leiloeiro confirmará ao interessado seu cadastramento via e-mail ou por emissão de logine senha provisória, que deverá ser, necessariamente, alterada pelo usuário.
>
> **Parágrafo único.** O uso indevido da senha, de natureza pessoal e intransferível, é de exclusiva responsabilidade do usuário.

- ⭐ **"Requisito indispensável" (art. 13):** sem cadastro prévio não se dá lance. O cadastro é
  **gratuito** por norma — plataforma que cobra pelo cadastro contraria o art. 13.
- **Operacional:** a validação do cadastro leva dias úteis nas plataformas reais (≠ habilitação no
  lote, que é rápida). Quem descobre isso na véspera do leilão **perde o lote**. Ver
  `context/mercado-leiloes-2026.md`.
- **Usa:** `estrategia-de-lance-e-habilitacao` ⭐ · `parecer-go-nogo-lote`.

## Arts. 16 e 17 — exposição e visitação ✅

> **Art. 16.** Os bens penhorados serão oferecidos em site designado pelo juízo da execução (art. 887, § 2º), com descrição detalhada e preferencialmente por meio de recursos multimídia, para melhor aferição de suas características e de seu estado de conservação.
>
> **Parágrafo único.** Fica o leiloeiro autorizado a fotografar o bem e a visitá-lo, acompanhado ou não de interessados na arrematação.

> **Art. 17.** Os bens a serem alienados estarão em exposição nos locais indicados no site, com a descrição de cada lote, para visitação dos interessados, nos dias e horários determinados.

- ⭐ **O art. 17 é o contrapeso do art. 18:** a norma **assegura visitação**. Se o edital impõe o ônus
  de verificar (art. 18) **mas a visitação foi negada ou inviabilizada**, o desequilíbrio é
  argumentável — é uma das poucas brechas contra a cláusula "sem garantia".
- **Usa:** `situacao-possessoria` · `analise-de-edital` · `risco-de-anulacao-do-certame`.

## Art. 18 — "SEM GARANTIA" e o ônus do interessado ✅ ⭐⭐ (a base normativa do gate)

> **Art. 18.** Os bens serão vendidos no estado de conservação em que se encontram, sem garantia, constituindo ônus do interessado verificar suas condições, antes das datas designadas para a alienação judicial eletrônica.

🔴 **Este é o artigo que o mercado replica em TODO edital — e ele NÃO é invenção do leiloeiro: é norma
do CNJ.** Consequências que o plugin repete sem exceção:

1. ⭐ **A cláusula "sem garantia" do edital NÃO é abusiva em si.** Ela tem base normativa expressa.
   Skill que afirmar que a cláusula é abusiva *por si só* está errada — e é erro que o guard bloqueia.
2. ⭐⭐ **É a base normativa do GATE DUE-DILIGENCE-FIRST.** O ônus de verificar é **do interessado**,
   por norma. Daí a proibição de afirmar situação do imóvel (ocupação, ônus, área, débito,
   regularidade) **sem documento lido**, e a regra do documento faltante: **NO-GO por insuficiência de
   prova**, nunca "provavelmente está ok".
3. ⭐ **O ataque útil NÃO é contra o art. 18 — é contra a OMISSÃO do art. 886, VI do CPC** (ônus,
   recurso ou processo pendente não mencionado no edital), que aciona a desistência do **art. 903 CPC,
   §5º, I**, com devolução imediata do depósito. Um ônus **omitido** não é coberto pelo "sem garantia":
   o edital tinha o dever legal de mencioná-lo.

- **Usa:** `anti-alucinacao-leiloes` ⭐ (impõe o gate) · `parecer-go-nogo-lote` ⭐ ·
  `analise-de-edital` ⭐ · `debitos-propter-rem` · `situacao-possessoria` · `leitura-de-matricula`.

## Arts. 19 e 20 — custos da divulgação e duração do pregão ✅

> **Art. 19.** O leiloeiro suportará os custos e se encarregará da divulgação da alienação, observando as disposições legais e as determinações judiciais a respeito.

> **Art. 20.** O período para a realização da alienação judicial eletrônica (art. 886, IV) terá sua duração definida pelo juiz da execução ou pelo leiloeiro, cuja publicação do edital deverá ser realizada com antecedência mínima de 5 (cinco) dias (art. 887, § 1º) da data inicial do leilão.

## Art. 21 — PRORROGAÇÃO AUTOMÁTICA ✅ ⭐ (3 min × 15 s)

> **Art. 21.** Sobrevindo lance nos 3 (três) minutos antecedentes ao termo final da alienação judicial exclusivamente eletrônica, o horário de fechamento do pregão será prorrogado em 3 (três) minutos para que todos os usuários interessados tenham oportunidade de ofertar novos lances.
>
> **Parágrafo único.** No caso de alienação presencial ou simultânea (presencial e eletrônica), o tempo previsto no caput deste artigo será de 15 (quinze) segundos.

🔴 **No leilão exclusivamente eletrônico NÃO EXISTE lance-surpresa no estalar do prazo.** Cada lance
nos 3 minutos finais empurra o fechamento em mais 3, **recursivamente**. Estratégia de *sniping*
**perde dinheiro à toa**: só revela o teto ao concorrente e reabre a janela.

| Modalidade | Janela de prorrogação |
|---|---|
| **Exclusivamente eletrônica** | **3 minutos** (recursivo) |
| **Presencial ou simultânea** | **15 segundos** |

⚠️ **Consequência prática:** identificar a modalidade **no edital** muda a tática de lance. E o
**incremento mínimo** não é publicado por nenhuma das plataformas (🟡) — é parâmetro por lote no
sistema, então **é impossível calcular de antemão o custo de cobrir um lance**. Dizer o contrário é
alucinação.

- **Usa:** `estrategia-de-lance-e-habilitacao` ⭐ · `analise-de-edital` · `custo-total-real-e-precificacao`.

## Art. 22 — PROIBIDO lance por e-mail e qualquer intervenção humana ✅ ⭐

> **Art. 22.** Durante a alienação, os lances deverão ser oferecidos diretamente no sistema do gestor e imediatamente divulgados on-line, de modo a viabilizar a preservação do tempo real das ofertas.
>
> **Parágrafo único.** Não será admitido sistema no qual os lances sejam realizados por e-mail e posteriormente registrados no site do leiloeiro, assim como qualquer outra forma de intervenção humana na coleta e no registro dos lances.

- ⭐ **Base direta de impugnação:** leilão em que houve **intermediação manual** de lances (registro
  posterior, lance por e-mail/telefone lançado pelo preposto) viola o §único. É vício **do
  procedimento**, apurável por log e pelo art. 34 (gravação integral).
- **Usa:** `risco-de-anulacao-do-certame` ⭐ · `anulatoria-de-arrematacao-judicial` ·
  `leiloeiro-responsabilidade-e-regularidade`.

## Arts. 23 a 26 — guia, pagamento, perfeição e lances anteriores ✅

> **Art. 23.** Com a aceitação do lance, o sistema emitirá guia de depósito judicial identificado vinculado ao juízo da execução.

> **Art. 24.** O pagamento deverá ser realizado de imediato pelo arrematante, por depósito judicial ou por meio eletrônico (art. 892), salvo disposição judicial diversa ou arrematação a prazo (art. 895, § 9º).

> **Art. 25.** A arrematação será considerada perfeita, acabada e irretratável tão logo assinado o auto pelo juiz, pelo arrematante e pelo leiloeiro, observadas as disposições do art. 903 do CPC (Código de Processo Civil).

> **Art. 26 (Res. CNJ 236).** Não sendo efetuados os depósitos, serão comunicados também os lances imediatamente anteriores, para que sejam submetidos à apreciação do juiz, na forma do art. 895, §§ 4º e 5º; art. 896, § 2º; arts. 897 e 898, sem prejuízo da invalidação de que trata o art. 903 do CPC (Código de Processo Civil).

- **Art. 25 remete ao art. 903 do CPC** — a arrematação é perfeita com a assinatura do auto, e daí
  correm os **10 dias**. Ver `context/cpc-leilao-879-903.md`, §17.
- **Art. 26 Res. CNJ 236 é a porta do "segundo colocado":** não efetuados os depósitos, os **lances imediatamente
  anteriores** vão ao juiz. Quem perdeu o lote por diferença pequena **não deve sumir**.
- **Usa:** `arrematacao-auto-e-carta` · `estrategia-de-lance-e-habilitacao` ·
  `invalidacao-embargos-e-desistencia-903`.

## Arts. 27 e 28 Res. CNJ 236 — rastreamento de IP e acesso do juízo ✅

> **Art. 27 (Res. CNJ 236).** Para garantir o bom uso do site e a integridade da transmissão de dados, o juiz da execução poderá determinar o rastreamento do número do IP da máquina utilizada pelo usuário para oferecer seus lances.

> **Art. 28.** O leiloeiro público deverá disponibilizar ao juízo da execução acesso imediato à alienação.

- ⭐ **O art. 27 é a ferramenta probatória contra o conluio de lances** (mesmo IP em contas distintas,
  "laranja" cobrindo o próprio lance). Pedido concreto e pouco usado — combina com o art. 34.
- **Usa:** `risco-de-anulacao-do-certame` ⭐ · `anulatoria-de-arrematacao-judicial` ·
  `reparacao-por-leilao-irregular`.

## Art. 29 Res. CNJ 236 — remoção e transferência POR CONTA DO ARREMATANTE ✅ ⭐

> **Art. 29 (Res. CNJ 236).** Correrão por conta do arrematante as despesas e os custos relativos à desmontagem, remoção, transporte e transferência patrimonial dos bens arrematados.

- ⭐ **Linha obrigatória da conta do arrematante:** desmontagem, remoção, transporte e **transferência
  patrimonial** correm por conta dele — **por norma**, não por cláusula do edital. É o "carrego" que o
  investidor esquece de somar. Ver `context/custo-total-do-arrematante.md`.
- **Usa:** `custo-total-real-e-precificacao` ⭐ · `parecer-go-nogo-lote` · `analise-de-edital`.

## Arts. 30 a 33 — responsabilidade do leiloeiro pelo sistema e risco do usuário ✅

> **Art. 30.** Serão de exclusiva responsabilidade do leiloeiro e do corretor público ônus decorrentes da manutenção e operação do site disponibilizado para a realização das alienações judiciais eletrônicas, assim como as despesas com o arquivamento das transmissões e ao perfeito desenvolvimento e implantação do sistema de leilões eletrônicos.

> **Art. 31.** A estrutura física de conexão externa de acesso e segurança ao provedor é de responsabilidade do leiloeiro e do corretor público.
>
> **Parágrafo único.** Caso a alienação judicial eletrônica não possa se realizar em razão de força maior, o início do novo período de pregão deverá ser publicado na forma do art. 897, § 1º, do CPC (Código de Processo Civil).

> **Art. 32.** Os lances e dizeres inseridos na sessão on-line correrão exclusivamente por conta e risco do usuário.

> **Art. 33.** Eventuais ocorrências ou problemas que possam afetar ou interferir nas regras desta Resolução serão dirimidos pelo juiz da execução.

- ⚠️ **O art. 32 joga no usuário o risco dos lances e dizeres inseridos.** Lance digitado errado (dígito
  a mais) é risco do arrematante — e o art. 897 do CPC pune a inadimplência com **perda da caução +
  banimento daquele leilão**. Não prometer reversão fácil de lance equivocado.
- **Art. 31, §único:** força maior → novo pregão publicado na forma do art. 897, §1º, do CPC.
- **Usa:** `estrategia-de-lance-e-habilitacao` · `invalidacao-embargos-e-desistencia-903` ·
  `leiloeiro-responsabilidade-e-regularidade`.

## Art. 34 — GRAVAÇÃO INTEGRAL do procedimento ✅ ⭐

> **Art. 34.** Todo o procedimento deverá ser gravado em arquivos eletrônicos e de multimídia, com capacidade para armazenamento de som, dados e imagens.

- ⭐ **Prova que existe e quase ninguém pede.** Todo o procedimento é gravado (som, dados e imagens).
  Combinado com o **art. 27** (IP) e o **art. 22** (vedação de intervenção humana), é o tripé
  probatório de quem alega vício **de pregão** — não de edital.
- **Usa:** `risco-de-anulacao-do-certame` ⭐ · `anulatoria-de-arrematacao-judicial` ·
  `reparacao-por-leilao-irregular`.

---

# CAPÍTULO III — DOS REGISTROS ELETRÔNICOS DE PENHORA

## Arts. 35 e 36 — convênios e vigência ✅

> **Art. 35.** O CNJ celebrará convênios com entidades públicas e privadas, a fim de viabilizar a efetivação da penhora de dinheiro e as averbações de penhoras incidentes sobre bens imóveis e móveis por meio eletrônico, nos termos do art. 837 do Código de Processo Civil.
>
> **§ 1º** Os convênios a que se refere o caput já celebrados por ocasião da vigência desta Resolução ficam por ela convalidados.
>
> **§ 2º** Até que sejam definidas as normas de segurança sob critérios uniformes do CNJ, ficam reconhecidas as diretrizes adotadas junto a cada instituição conveniada.

> **Art. 36.** Esta Resolução entra em vigor 90 (noventa) dias após a data de sua publicação.
>
> Ministro RICARDO LEWANDOWSKI

- **Vigência:** 90 dias após a publicação (DJe/CNJ de 15/07/2016) → **em vigor desde 13/10/2016**, sem
  alteração posterior registrada na ficha.

---

## GUARD — o que este anexo proíbe

1. Dizer que **"a comissão é de 5% por força do CPC"** — a fonte é o **art. 7º desta Resolução** +
   Decreto 21.981/32. O CPC **não fixa percentual**.
2. Tratar os **5% como teto** — o texto diz "**no mínimo**". 7% em leilão judicial é lícito
   (arbitramento do juiz), com os resíduos do E1.
3. Afirmar que a cláusula **"sem garantia"** do edital é **abusiva em si** — o **art. 18** lhe dá base
   normativa. O ataque é contra a **omissão do art. 886, VI do CPC**.
4. Prometer **lance-surpresa** no fim do pregão eletrônico — o **art. 21** prorroga 3 min
   recursivamente (15 s no presencial/simultâneo).
5. Afirmar **incremento mínimo** de lance — nenhuma plataforma publica (🟡).
6. Dizer que se credencia **"a plataforma"** — credencia-se o **leiloeiro pessoa física** (art. 1º).
7. Impugnar nomeação de leiloeiro por **"quebra da escala de antiguidade"** em execução cível — a
   escala **não se aplica** ao judicial.
8. Afirmar regra **local de tribunal** sem conferir — o **art. 10** delega, e os regulamentos não foram
   levantados (🟡).

Toda peça fecha por **`suprema-corte-leiloes`** (R1-R4) **+ `validador-leiloes`**.

---

## Fonte e verificação

- **Texto integral (transcrição verbatim):** página oficial do ato —
  `https://atos.cnj.jus.br/atos/detalhar/2313` — capturada em **2026-08-02**.
- **Fac-símile oficial (escaneado, SEM camada de texto):**
  `https://atos.cnj.jus.br/files/resolucao_236_13072016_15072016155240.pdf` — 12 páginas, zero fontes
  embutidas; serve para conferência visual, **não** para transcrição.
- **Publicação:** DJe/CNJ, nº 121, de 15/07/2016, p. 2-5. **Situação: Vigente. Alteração: vazio.**
- **Conferência:** 36 artigos presentes, cada um **uma única vez** na página.
- **Anexos irmãos:** `context/cpc-leilao-879-903.md` (o art. 882, §1º que dá fundamento a esta
  Resolução) · `context/leiloeiro-decreto-21981-in-drei-52.md` · `context/custo-total-do-arrematante.md`
  · `context/clausulas-armadilha-de-edital.md` · `context/jurisprudencia-leiloes.md`.
