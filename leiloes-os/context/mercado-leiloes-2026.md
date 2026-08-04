# Mercado de leilões 2026 — volume, deságio, concorrência e vocabulário

> Anexo de mercado do plugin **leiloes-os**. Insumo dos pareceres (o que é "preço de mercado" e "deságio real"), da skill `assessoria-de-arrematacao-proposta-e-contrato` (precificação do serviço) e da copy.
> **Regra deste arquivo: número com fonte, ou não entra.** Onde as fontes divergem no que o número mede, a divergência está **declarada** e a formulação conservadora está indicada.
> **Captura:** 2026-08-02. **Legenda:** ✅ multi-fonte ou fonte primária · 🟡 secundária / divergente · 🔴 não provado.
> **Como usar:** `grep` pelo tema (`deságio`, `concorrência`, `honorários`, `vocabulário`) e **leia a faixa**.

---

## 0. ⛔ AS QUATRO TRAVAS DESTE ANEXO

1. **NUNCA prometer "70% de desconto".** A média provada é **37,3%**. A formulação permitida é *"deságio médio de 37,3%, com lotes chegando a 70%"*.
2. **NUNCA dizer "leilão é seguro".** O próprio material do nicho vende a tríade de riscos (§4). E nunca o oposto — "cai como qualquer negócio" — que é igualmente falso.
3. **NUNCA dar resposta única sobre débito condominial.** É onde toda plataforma concorrente erra, e é diferencial de produto dizer a verdade (§6).
4. **Não existe canal de leilão com "milhões de inscritos".** 🔴 **Não confirmado.** A viralidade do nicho vem do **volume de plataformas (8 SaaS) e de cursos (R$ 617–5.900)**, não de um canal gigante isolado. Não usar como pilar de copy.

---

## 1. VOLUME E TENDÊNCIA

| Indicador | Número | Fonte | Âncora |
|---|---|---|---|
| Imóveis levados a leilão — **1º semestre/2025** | **116,6 mil** | Abraim (Assoc. Brasileira dos Arrematantes de Imóveis) | ✅ multi-fonte |
| Crescimento vs. 1S/2024 | **+25,1%** | Abraim | ✅ |
| **Deságio médio** sobre a avaliação oficial | **37,3%** | Abraim | 🟡 |
| Prazo médio edital → arrematação | **45 dias** | Abraim | 🟡 |
| Leilões registrados em 2025 | 299.732 | via imprensa setorial | 🟡 secundária |
| Volume financeiro movimentado em 2025 | R$ 420 bilhões | via imprensa setorial | 🟡 secundária |
| Inadimplentes no país | 81,7 milhões (42% reincidentes) | via imprensa setorial | 🟡 |
| Crescimento do volume de arrematações em 2025 | ~18% | imprensa setorial | 🟡 |

> ⚠️ **Ressalva honesta sobre o 116,6 mil:** as fontes **divergem no que o número mede** — uma registra "imóveis **levados a leilão**", outra registra "**arremates**". Para copy e parecer, usar a formulação conservadora, **verdadeira nas duas leituras**: *"116,6 mil imóveis a leilão no primeiro semestre de 2025, +25,1%"*. 🟡

**Motores declarados do crescimento** (convergentes em todas as fontes): inadimplência condominial e bancária em alta · juros elevados empurrando credores à liquidez · consolidação do leilão **eletrônico** como canal padrão · retomada de imóveis por **alienação fiduciária** alimentando o pipeline.

### ⭐ A leitura que define o produto DUAL

O mercado cresce por **inadimplência**, não por euforia. Isso significa que os dois lados do produto crescem **juntos e em proporção fixa**: cada imóvel que entra em leilão gera simultaneamente **um arrematante** (que precisa de due diligence) e **um executado/fiduciante** (que precisa de defesa).

> **O plugin dual não é um hedge — é a captura das duas pontas do mesmo evento.**

---

## 2. AS TRÊS DORES Nº 1 DO ARREMATANTE

Os criativos do nicho convergem para a **mesma tríade**, formulada quase com as mesmas palavras em canais independentes:

> **"IMÓVEL OCUPADO · DÍVIDAS OCULTAS · LEILÃO ANULADO POR VÍCIO"**

| Dor | O que o arrematante teme | Camada que responde |
|---|---|---|
| **1. Imóvel ocupado** | Arrematar e não conseguir entrar; ocupante resiste; custo e prazo de desocupação não precificados | `situacao-possessoria` + `imissao-na-posse-do-arrematante` |
| **2. Dívidas ocultas** | IPTU, condomínio, taxas — descobrir depois que a dívida "veio junto" | `debitos-propter-rem` |
| **3. Anulação posterior** | Pagar, registrar, reformar — e o leilão cair por vício de intimação, preço vil ou edital | `risco-de-anulacao-do-certame` ⭐ |

> ⭐ **A dor nº 3 é a mais valiosa comercialmente e a menos atendida.** **Nenhum** dos 8 SaaS concorrentes analisa risco de anulação por vício do procedimento — todos param em matrícula, edital e ROI. É justamente o item que exige **corpus jurídico**, não base de dados. **É o fosso.**

---

## 3. CONCORRÊNCIA DIRETA — 8 plataformas de due diligence com IA

**Existe concorrência, e é densa.** Ao menos **8 plataformas brasileiras** vendem análise de leilão com IA. **Todas atacam o lado investidor. Nenhuma redige peça.**

| Plataforma | Preço | O que a IA faz | Escala declarada |
|---|---|---|---|
| **Arremata.ai** | Grátis (5 análises) · **dossiê R$ 9,90** · GOLD R$ 39,17/mês (**R$ 470/ano**) | Score 0–100, riscos jurídicos por gravidade, ROI à vista × financiado, lance mín./máx. sugerido, lê editais, matrículas e processos | 34 mil+ imóveis · 140+ leiloeiros · 27 estados |
| **BidHero** | **R$ 99/mês** · **R$ 712/ano** · trial 10 imóveis/30 d | Análise de matrícula e edital com alertas de risco, ROI, comparação de mercado, mapa | 900+ leiloeiros |
| **Leilão Ninja** | **R$ 97/mês** · **R$ 797/ano** · garantia 7 d | **Índice 0–10** (margem 60% + risco 30% + demanda 10%), compara 20+ portais, risco jurídico e dívidas | 900+ leiloeiros · 5.000+ investidores |
| **Monitor Leilão** | Grátis · **R$ 79,90/mês** | Agregação, badges de % OFF, dados premium (endereço/leiloeiro) | canal com 17 mil inscritos |
| **Pro Leilão** | a partir de **R$ 24/semana** · trial 3 dias | Análise de matrícula com IA: histórico de proprietários, irregularidades, financiamentos | foco em imóveis de bancos |
| **Smart Leilões** | Grátis + Premium (não exposto) 🟡 | **Ranking 0–100**; perfis Conservador × Arrojado; calculadora com ITBI, emolumentos, laudêmio, desocupação | 34.500+ imóveis · 97 leiloeiros |
| **BUSCAi Leilões** | não capturado 🟡 | Soma custo total real e compara com preço da região | — |
| **Auctio** | não capturado 🟡 | "Análise de risco jurídica automática" + lucro estimado | — |

**Adjacentes** (análise de matrícula pura, sem leilão): serviços de análise de matrícula avulsa e agregadores de lote.

### ⭐ O que a concorrência PROVA (a favor) e o que DEIXA ABERTO (o fosso)

**Prova:**
- O mercado **paga por due diligence automatizada de leilão** — R$ 39–99/mês, com players em escala. A hipótese central do produto está **validada por 8 empresas**, não por suposição.
- Todas convergem para o mesmo tripé: **matrícula + edital + custo total**. O rol da camada de due diligence está certo.
- Todas convergem para **score/ranking** (0–100, 0–10, GO/NO-GO). O parecer GO/NO-GO é o **formato que o mercado já ensinou o usuário a consumir**.

**Deixam aberto — NENHUMA plataforma faz:**

1. **Redige peça.** Zero. Nenhuma entrega anulatória, imissão, embargos ou agravo.
2. **Atende o lado do devedor/executado.** Todas são 100% arrematante. **Metade do mercado está descoberta.**
3. **Analisa risco de anulação por vício do procedimento.** Exige corpus jurídico, não base de dados.
4. **Entrega o instrumento comercial** (proposta + contrato de assessoria) que faz o advogado faturar.
5. **Assume divergência jurisprudencial.** Todas dão **resposta única** sobre condomínio — e a resposta única aqui está errada nos dois sentidos possíveis (§6).

> **Posicionamento derivado:** o plugin **não compete com as plataformas de dados** — ele é a camada que **começa onde elas param**. Parte do comprador **já assina uma delas**.

### ⚠️ Risco competitivo real — a ancoragem decide o preço

**Um dossiê avulso a R$ 9,90 é o piso psicológico do mercado.** Se a comunicação vender **"análise de lote"**, o produto é comparado a **R$ 9,90**. Se vender **"parecer + peça + os dois lados"**, é comparado a **honorário**. A ancoragem correta é **honorário, nunca assinatura**.

---

## 4. BENCHMARK DE CURSOS E MENTORIAS DO NICHO

| Produto | Preço | Formato |
|---|---|---|
| Formação de arrematantes (imersão presencial + EAD) | **De R$ 14.400 por R$ 5.900** à vista · 12× R$ 491,66 | Presencial + EAD |
| Mentoria de arrematação (10 semanas ao vivo) | **R$ 2.697** à vista · 12× R$ 275,66 | Ao vivo, 8 módulos, lista de leiloeiros |
| Curso avançado — leilão judicial e extrajudicial | **R$ 1.299,90** (de R$ 1.599,90) | EAD |
| Curso de entrada do nicho | **12× R$ 51,40 (~R$ 617)** | EAD, móveis + imóveis |
| Curso de arrematação da **Escola Superior da Advocacia (OAB-SP)** | institucional | — |
| Curso de leilões de instituto de direito imobiliário | não capturado 🟡 | Ao vivo; público declarado: **"advogados, investidores e profissionais"** |

**Faixa do nicho: R$ 617 → R$ 5.900.** Mediana em torno de **R$ 1.300–2.700**.

### Dois achados estratégicos escondidos nessa tabela

1. **O produto dual JÁ EXISTE no mercado — validado por quem vende.** Um dos cursos ensina explicitamente o ciclo completo *"para quem quer lucrar adquirindo **ou vendendo serviços de assessoria** a interessados"*. Outro vende para "advogados, investidores e profissionais" na mesma turma. **A decisão dual não é aposta — é o formato que o mercado já provou.**
2. **A ESA OAB-SP tem curso de arrematação.** O nicho atravessou de "investimento alternativo" para **formação jurídica reconhecida**. Isso **legitima o lado advogado** do produto diante do comprador cético.

---

## 5. ⭐ HONORÁRIOS DA ASSESSORIA DE ARREMATAÇÃO — o serviço recorrente

| Modelo | Faixa praticada | Observação |
|---|---|---|
| **Percentual sobre o valor arrematado** | **5% a 10%** (algumas fontes: 3% a 10%) | Modelo dominante |
| **Valor fixo por serviço** | **R$ 1.000 a R$ 5.000** | Análise de edital + participação no leilão + acompanhamento |
| **Cláusula de êxito** | % sobre o valor economizado ou sobre o valor do bem | Combinada com o fixo |

**Escopo típico vendido como pacote** (converge em todos os escritórios do nicho), em **três tempos**:

- **ANTES** — análise de edital + matrícula + ocupação + débitos + risco de anulação;
- **DURANTE** — habilitação e estratégia de lance;
- **DEPOIS** — carta de arrematação, ITBI, registro, baixa de gravames, imissão na posse.

> 🟡 **Limite honesto:** os escritórios do nicho **não publicam tabela** — a maioria remete a contato. As faixas acima vêm de **conteúdo editorial de escritórios** explicando o mercado, **não de tabela oficial da OAB**. Uma **tabela oficial de seccional** para assessoria de arrematação **não foi localizada**. Ao usar em proposta, apresentar como **prática de mercado**, não como tabela.

**A prova documental de que o serviço é necessário** está no próprio edital: *"o Leiloeiro é auxiliar da justiça e está impedido de atuar nessa esfera"* — ver `clausulas-armadilha-de-edital.md` ARM-15.

---

## 6. A TESE EM DISPUTA — e por que a honestidade aqui é diferencial de produto

O mercado de conteúdo trata o débito condominial do arrematante como **rachado**, com fontes apontando em direções opostas. **A verificação em fonte primária mostrou outra coisa:**

- Com o **edital INFORMANDO** a dívida, o arrematante **RESPONDE** — orientação **consolidada**, reafirmada pela **2ª Seção do STJ, por unanimidade, em 13/05/2026**.
- **Proibido escrever "a matéria está em aberto no STJ".**
- A brecha real é o **edital OMISSO** — e é **tese**, não regra.

Ver `jurisprudencia-leiloes.md` §4 para o verbete completo.

> ⭐ **Por que isso é ativo comercial:** as 8 plataformas dão **resposta binária** sobre condomínio — e a resposta binária está errada. Quem entrega a distinção correta (**tributário fechado a favor** × **condominial condicionado ao edital**) entrega o que nenhuma delas entrega, e evita o prejuízo que a resposta errada causa. **Postura honesta não é fraqueza de produto — é o produto.**

---

## 7. O VOCABULÁRIO QUE VIRALIZA

| Termo | Nota de uso |
|---|---|
| **"deságio"** | Termo-assinatura do nicho. O insider fala "deságio", o leigo fala "desconto". **Usar os dois na mesma peça** marca autoridade sem excluir o iniciante |
| **"arrematar"** | O verbo do nicho. **Nunca "comprar em leilão"** ao falar com insider |
| **"antes do lance"** | Marcador temporal que separa due diligence de arrependimento. É o nome que converte melhor que qualquer sigla |
| **"70% OFF"** | ⚠️ **Nunca prometer.** Aparece em badge de plataforma; a média provada é **37,3%** |
| **"imóvel abaixo do mercado"** | Genérico; converte pouco sozinho |
| **"o problema quase nunca está no preço, está no risco mal analisado"** | ⭐ Capturado em criativo de plataforma concorrente — **é a tese exata do pilar DUE-DILIGENCE-FIRST**, dita pelo próprio mercado |

---

## 8. GANCHOS DUAIS — advogado × investidor

Os do lado advogado ancoram em **honorário**; os do investidor, em **prejuízo evitado** — **nunca em lucro prometido**.

| Tema | 🎓 ADVOGADO | 💰 INVESTIDOR |
|---|---|---|
| **As teses de 2025** | "Preço vil abaixo de 50%, edital desatualizado, intimação viciada. Todo leilão de alienação fiduciária dos últimos anos virou auditável — e cada auditoria é um cliente." | "Você pode arrematar hoje um leilão que será anulado amanhã. O plugin checa **antes** do seu lance." |
| **Imóvel ocupado** | "Imissão na posse é o serviço que o arrematante contrata sem pechinchar — ele já pagou o imóvel." | "Arrematou e não consegue entrar? Saber o rito **antes** do lance é o que separa deságio de prejuízo." |
| **Dívidas ocultas** | "O Tema 1.134 blindou seu cliente contra IPTU anterior. No condomínio, a regra é outra — e quem souber disso ganha a defesa." | "IPTU antigo **não** é seu. Condomínio antigo **pode ser** — depende do que o edital diz. Quem te prometer resposta única está chutando." |
| **Due diligence** | "Assessoria de arrematação é 5% a 10% do arrematado. Falta só o parecer e o contrato — estão aqui." | "O problema quase nunca está no preço. Está no risco mal analisado. GO ou NO-GO antes do lance." |
| **Volume** | "116,6 mil imóveis a leilão só no primeiro semestre de 2025, +25,1%. Cada um gera um arrematante **e** um executado." | "116,6 mil imóveis a leilão em seis meses, deságio médio de 37,3%. O funil é enorme — o filtro é o problema." |
| **Os dois lados** | "Mesmo corpus, dois lados: você ataca o leilão pelo executado e defende a arrematação pelo comprador." | "Quem entende como se anula um leilão é quem sabe comprar um que não será anulado." |

### 🚫 As quatro regras que a comunicação NÃO pode furar

- ❌ Nunca **"70% de desconto garantido"** — a média provada é 37,3%; 70% é teto de lote isolado.
- ❌ Nunca **"leilão é seguro"** — o material do próprio nicho vende a tríade de riscos.
- ❌ Nunca **resposta única sobre condomínio**.
- ❌ Nunca **"essa arrematação nunca cai"** — e nunca o oposto, "cai como qualquer negócio".
- ✅ Sempre *"deságio médio de 37,3% (Abraim), com lotes chegando a 70%"*.

---

## 9. 🟡 O QUE ESTA FRENTE **NÃO** PROVOU

| Lacuna | Status |
|---|---|
| **Volume judicial quantificado** de anulatórias e embargos | 🔴 base de jurisprudência bloqueou a coleta; contagem retornou vazio |
| **Canal de leilão com "milhões de inscritos"** | 🔴 **NÃO confirmado** — o maior capturado no nicho tem 17 mil inscritos. **Não usar como pilar de copy** |
| Preço de dois cursos e de três plataformas | 🟡 não capturado |
| **Tabela oficial da OAB** para assessoria de arrematação | 🔴 não localizada — a faixa 5–10% é editorial de escritórios |
| Volume e participação dos **leilões de bancos públicos** (maior ofertante isolado do país) | 🔴 não pesquisado — pode alterar a priorização, pois esse rito tem particularidades |
| Estatística de **cumprimento real** da liminar de 60 dias (art. 30 da Lei 9.514) | 🔴 não pesquisada — liminar concedida não é imóvel vazio |

---

## 10. FRONTEIRAS DESTE ANEXO

| Precisa de | Vá para |
|---|---|
| A conta do arrematante (o que corrói o deságio de 37,3%) | `custo-total-do-arrematante.md` |
| As cláusulas de edital que geram as três dores | `clausulas-armadilha-de-edital.md` |
| Os julgados por trás de cada tese comercial | `jurisprudencia-leiloes.md` |
| O gate que separa parecer de palpite | `metodologia-leiloes.md` |
