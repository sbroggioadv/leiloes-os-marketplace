# Metodologia do plugin leiloes-os

> Anexo mestre. O "como pensar" antes do "o que escrever": os pilares, o **gate DUE-DILIGENCE-FIRST**, o mapa das 9 camadas, a árvore de triagem, as verdades duras, os selos e o contrato de anti-alucinação.
> É o arquivo que o `leiloes-master`, o `anti-alucinacao-leiloes`, o `validador-leiloes` e a `suprema-corte-leiloes` consultam para não escorregar.
> **Captura das fontes:** Planalto, STJ (inteiro teor e portal de precedentes), STF, CNJ, DREI e editais reais, em **02/08/2026**.
> **Como usar:** `grep` pela seção (`GATE`, `TRIAGEM`, `VERDADES`, `PROIBIDO`, `RELÓGIO`) e **leia a faixa**.

---

## 1. ⛔ A REGRA DE LEITURA DOS ANEXOS (vale para TODAS as skills)

1. **Nunca despejar um anexo inteiro em contexto.** `grep` pelo dispositivo, pelo número do julgado ou pelo tema, e **ler a faixa**.
2. **Nunca citar dispositivo, súmula, tema, prazo ou percentual que não esteja em anexo `context/`.** O `validador-leiloes` bloqueia número não ancorado.
3. **Nunca citar como vigente o que está em bloco de LISTA NEGRA, PENDENTES ou 🟡.** Ver `jurisprudencia-leiloes.md` §0.
4. **Zero dead-ref:** só existem **11 anexos** (§13). Não inventar nome de arquivo.

---

## 2. OS PILARES

### Herança da família Adv-OS

- **Porta única** — todo pedido entra pelo `leiloes-master`, que roteia e dirime.
- **Toda peça fecha por `suprema-corte-leiloes` (R1-R4) + `validador-leiloes`.** Nenhuma peça sai sem os dois.
- **Standalone-first** — os recursos da C7 são **modelados** no cível, sem dependência dura de outro plugin.
- **Anti-alucinação em duas camadas** — guard (`anti-alucinacao-leiloes`) + validador (`validador-leiloes`).
- **Lei VIGENTE em agosto/2026** — DL 70/66 arts. 29-41 mortos, Lei 14.711 no lugar, Tema 1.288 transitado.
- **Despersonalizado** — autoria IA Combativa; o escritório do usuário é configurado em runtime.

### ⭐ O 4º pilar, próprio deste domínio: DUE-DILIGENCE-FIRST

**Nenhuma skill de lance, arrematação ou estratégia de aquisição roda sem o gate.** Ver §3 — e a razão é **textual, não pedagógica**.

### O pilar de postura honesta

Onde a jurisprudência está **condicionada**, **ausente** ou **monocrática** — condomínio com edital omisso, evicção do arrematante, comissão no extrajudicial, preço vil extrajudicial — **dizer que está**. Resposta única aqui é **alucinação com cara de certeza**, e é exatamente onde os 8 SaaS concorrentes entregam resposta binária errada.

> **Postura honesta não é fraqueza do produto. É o produto.**

---

## 3. ⭐⭐ O GATE DUE-DILIGENCE-FIRST (bloqueante)

```
pedido de LANCE · ARREMATAÇÃO · "vale a pena esse lote?"
   │
   ├─→ triagem-leiloes        (judicial × extrajudicial · papel · fase)
   │
   ├─→ ██ GATE — 4 PROVAS DOCUMENTAIS, TODAS OBRIGATÓRIAS ██
   │      [1] EDITAL lido      → analise-de-edital
   │      [2] MATRÍCULA lida   → leitura-de-matricula
   │      [3] OCUPAÇÃO apurada → situacao-possessoria
   │      [4] DÉBITOS levantados → debitos-propter-rem
   │        + risco-de-anulacao-do-certame  ⭐ (cruza [1]-[4] contra as teses de 2025)
   │        + custo-total-real-e-precificacao  (teto com comissão embutida)
   │
   ├─→ parecer-go-nogo-lote   → GO · GO-CONDICIONADO · NO-GO
   │
   └─→ SÓ COM GO: estrategia-de-lance-e-habilitacao · arrematacao-parcelada-895
```

### ⚖️ A RAZÃO TEXTUAL do gate — por que ele é PRÉ-lance, e não pedagogia

O **CPC art. 903, §2º** conta o prazo de 10 dias do **APERFEIÇOAMENTO da arrematação** — a **assinatura do auto** —, **não** da ciência do vício:

- Assinado o auto, a arrematação é **perfeita, acabada e irretratável** (art. 903 CPC, *caput*).
- As três hipóteses do **§1º** (invalidação · **ineficácia** · resolução) só podem ser provocadas **em 10 dias contados do aperfeiçoamento**.
- Depois de expedida a **carta**, resta apenas **ação autônoma** (§4º), com o arrematante como **litisconsorte necessário**.

> **A due diligence feita DEPOIS do lance chega tarde POR CONSTRUÇÃO DA LEI.** O vício oculto costuma aparecer na imissão na posse — **meses ou anos depois**. Nesse momento o §2º já correu. **A preclusão é a armadilha central do arrematante**, e o gate existe para colocá-la do lado certo do relógio.

**O reforço do §5º, I:** provado **ônus real ou gravame não mencionado no edital** (violação do art. 886, VI), o arrematante **desiste e recebe o depósito de volta imediatamente** — mas isso também **caduca em 10 dias**. É a saída mais forte que ele tem, e ela só existe para quem **auditou o edital contra a matrícula**.

**O freio do §6º:** suscitar vício **infundado** para forçar a desistência é **ato atentatório à dignidade da justiça**, com multa de até **20%** do valor atualizado do bem. Por isso a auditoria tem de ser **documental**, nunca especulativa.

### 🚨 A REGRA DO DOCUMENTO FALTANTE

**Faltando qualquer uma das 4 provas, o parecer sai `NO-GO por insuficiência de prova`.**

**Nunca** "provavelmente está ok" · **nunca** "aparentemente livre" · **nunca** "não identifiquei ônus" quando o que houve foi **não ter lido a matrícula**.

### 🚫 A PROIBIÇÃO DO GUARD

**É vedado afirmar situação do imóvel — ocupação, ônus, área, débito, regularidade — sem documento lido.**

A dor nº 1 do arrematante é **comprar problema invisível**, e o **art. 18 da Res. CNJ 236/2016** põe esse ônus **nele**, com base normativa:

> "Os bens serão vendidos no estado de conservação em que se encontram, **sem garantia**, constituindo ônus do interessado verificar suas condições, antes das datas designadas para a alienação judicial eletrônica."

> ⚠️ **Corolário que separa o profissional do amador:** a cláusula "sem garantia" do edital **NÃO é abusiva em si** — ela reproduz a norma. Sustentar que é abusiva é **tese perdida** e queima a credibilidade da peça. O que se ataca é o **edital que descumpre o art. 886**, não o edital que avisa.

### Os três vereditos

| Veredito | Quando | O que acompanha |
|---|---|---|
| **GO** | 4 provas lidas · risco de anulação baixo · conta fecha com margem | **Teto de lance** (com comissão embutida) |
| **GO-CONDICIONADO** | 4 provas lidas, mas há condição objetiva a resolver (habilitação do condomínio, regularização, ocupante identificado) | Teto **rebaixado** + a condição nomeada e o custo dela |
| **NO-GO** | Falta prova documental · risco de anulação alto · a conta inverte de sinal | **O motivo específico** — nunca "não recomendo" genérico |

---

## 4. O MAPA DAS 9 CAMADAS (55 skills)

| Camada | Escopo | Nº |
|---|---|---|
| **C0 — Orquestração / QA** | Porta única, Suprema Corte R1-R4, onboarding dual, triagem, memória de caso, estilo, validador, guard anti-alucinação | 8 |
| **C1 — Fundação** | CPC do leilão + Res. CNJ 236 · Lei 9.514 consolidada · Lei 14.711 · leiloeiro · jurisprudência | 5 |
| **C2 — Due diligence do arrematante** ⭐ | **O fosso e a vitrine.** Edital · matrícula · ocupação · débitos · risco de anulação · custo total · estratégia de lance · parecer GO/NO-GO | 8 |
| **C3 — Leilão judicial** | Mecânica · intimações do 889 e ineficácia · auto e carta · parcelamento 895 · adjudicação e as três remições · invalidação e desistência 903 | 6 |
| **C4 — Leilão extrajudicial** | Consolidação e intimação · regime do imóvel residencial 26-A · os dois leilões · hipoteca da 14.711 🔴 · excussão múltipla e concurso · vícios do procedimento · outras garantias | 7 |
| **C5 — Pós-arrematação** | Imissão na posse · desocupação e locação · registro/ITBI · débitos e créditos · evicção e desfazimento | 5 |
| **C6 — Defesa do devedor / executado / fiduciante** | **Metade do mercado, que nenhum concorrente atende.** Anulatórias, defesa da consolidação e purga, preço vil, nulidades de intimação, defesa contra imissão, saldo remanescente, reparação | 8 |
| **C7 — Recursos standalone** | Agravo · apelação e ED · recursos excepcionais — **modelados** no cível, sem dependência dura | 3 |
| **Transversal / consultivo / comercial** | Tutela de urgência · protocolo P4 · assessoria (proposta + contrato) · leiloeiro: comissão e prestação de contas · leiloeiro: responsabilidade e regularidade | 5 |

**Ordem de prioridade se o ciclo apertar:** C0 → C1 → **C2** → C6 → C4 → C5 → C3 → transversal → C7.

---

## 5. A ÁRVORE DE TRIAGEM — três perguntas, e a terceira é irreversível

```
1. JUDICIAL ou EXTRAJUDICIAL?
   ├─ Judicial (CPC 879-903 + Res. CNJ 236)          → C3 · C2 · C6
   ├─ Extrajudicial AF (Lei 9.514)                    → C4 · C2 · C6
   ├─ Extrajudicial HIPOTECA (Lei 14.711, art. 9º) 🔴 → C4 — e checar o FILTRO DO §15
   └─ Leilão público administrativo (Lei 14.133)      → ⛔ GAP DECLARADO: reconhecer e encaminhar,
                                                          NUNCA improvisar

2. QUAL É O PAPEL?
   ├─ Arrematante (ou pretendente)  → C2 · C5
   ├─ Executado / fiduciante        → C6
   ├─ Credor / exequente            → C3 · C4
   └─ Leiloeiro                     → Transversal (2 skills consultivas)

3. ⭐ QUAL É A FASE?  — decide a via, e é IRREVERSÍVEL
   ├─ ANTES do lance          → GATE de due diligence (§3). Ainda dá para não errar
   ├─ PÓS-lance, < 10 dias    → CPC 903 §§1º-2º: invalidação · ineficácia · resolução
   │                             + as 3 portas de desistência do §5º. JANELA ABERTA
   ├─ PÓS-carta               → só AÇÃO AUTÔNOMA (§4º), arrematante como
   │                             LITISCONSORTE NECESSÁRIO
   └─ PÓS-imissão             → discussão indenizatória / evicção / débitos
```

> 🚨 **Errar a fase entrega a peça errada.** Pedir invalidação nos autos depois da carta, ou ação autônoma dentro dos 10 dias, é erro que se paga com extinção. **A fase é a primeira coisa a travar na triagem.**

---

## 6. AS VERDADES DURAS — o plugin vende a lei vigente, não o folclore de leiloeiro

### Bloco extrajudicial 🔴 (o que o treino não tem firme)

1. **🔴🔴🔴 DL 70/66, arts. 29 a 41 = REVOGADOS** (Lei 14.711/2023, art. 18, I — Capítulo III inteiro), desde **31/10/2023**. **O rito da execução extrajudicial hipotecária por agente fiduciário está MORTO.** ⚠️ **Qualifique:** não dizer "o DL 70/66 foi revogado" — os Capítulos I e II sobrevivem, e o **art. 34 segue aplicado a fatos anteriores a 2017** (Tema 1.288/STJ).
2. **🔴🔴 O rito hipotecário novo é o art. 9º da Lei 14.711/2023:** intimação pessoal **pelo oficial do RI** (15 dias) → averbação da excussão na matrícula → 1º leilão em 60 dias → 2º em 15 dias → **ata notarial de arrematação** como título hábil para registro. **Sem agente fiduciário, sem juiz.**
3. **🔴🔴 O filtro do §15 mata metade dos casos:** o rito do art. 9º só vale se o **título constitutivo da hipoteca contiver, como requisito de validade, previsão expressa do procedimento com menção ao teor dos §§1º a 10**. Hipoteca anterior a 31/10/2023 tipicamente **não tem** essa cláusula. **Defesa de primeira linha do devedor e item obrigatório da due diligence.**
4. **🔴🔴 Leilão negativo deixou de quitar a dívida como regra** — Lei 9.514, art. 27, **§5º-A**: o devedor **continua obrigado pelo saldo remanescente**. **Exceção:** imóvel residencial do devedor (art. 26-A, §4º), onde a dívida se extingue — e o §5º qualifica isso como **condição resolutiva inerente à dívida, que alcança também a via judicial**.
5. **🔴 No 2º leilão o credor PODE aceitar 50% da avaliação, a seu exclusivo critério** (9.514, art. 27, §2º · 14.711, art. 9º, §6º). É **faculdade do credor**, jamais direito do arrematante.
6. **🔴 Penhora não trava mais o leilão de AF** (art. 27, §11): constrições **sobre o direito real de aquisição do fiduciante** não obstam consolidação nem venda; os titulares se sub-rogam no **saldo** (§12). ⚠️ **Limite literal:** o §11 fala do direito **do fiduciante** — constrição sobre a propriedade ou de outra relação **não está coberta**.
7. **🔴 A defesa do fiduciante foi comprimida a um eixo único** (art. 30, §único): arrematado o imóvel ou consolidada definitivamente a propriedade, **nenhuma** discussão sobre cláusulas ou requisitos obsta a reintegração — **exceto a exigência de notificação**. **Estratégia do executado: atacar a intimação, não o preço.**
8. **🔴 Intimação eletrônica virou pré-requisito** (art. 26, §4º-B): havendo contato eletrônico no contrato, é **imprescindível** intimar por essa via com **15 dias** de antecedência antes do edital. Somada ao item 7, **é a tese de nulidade mais forte que restou**.

### Bloco judicial

9. **Preço vil é régua em CASCATA e o "50%" é supletivo** (CPC 891, §único): fixado preço mínimo no edital, vil é o que fica **abaixo dele**; só na **ausência** vale o piso de 50%. Três erros a bloquear: (a) "o CPC fixa 50%"; (b) o piso valeria só para a 1ª praça; (c) transportar os 50% para o extrajudicial.
10. **Comissão e despesas NÃO estão dentro do lance** — são pagamento adicional e **condição para a carta** (CPC 901, §1º). O CPC **não fixa percentual** (884, §único).
11. **Falta de intimação de titular de direito real gera INEFICÁCIA (CPC 804), não nulidade** — art. 903, §1º, II é expresso. **Para o arrematante isso é PIOR:** fica com o imóvel **e com o gravame**, não purgado perante quem não foi intimado.
12. **O art. 903 CPC é o relógio do arrematante** — ver §3.
13. **O art. 903, §5º, I é a saída mais forte e caduca em 10 dias** — ver §3.
14. **Prorrogação automática de 3 minutos** (Res. CNJ 236, art. 21): no leilão exclusivamente eletrônico **não existe lance-surpresa no estalar do prazo**; cada lance nos 3 minutos finais empurra o fechamento, recursivamente. No presencial/simultâneo, **15 segundos**. **Sniping perde dinheiro à toa.**
15. **A proposta parcelada do art. 895 CPC NÃO reserva o bem:** §7º — qualquer **lance à vista sempre prevalece**; §6º — a proposta **não suspende o leilão**. Mínimo 25% à vista + saldo em até 30 meses; a multa do §4º incide sobre a parcela inadimplida **somada às vincendas**.

### Bloco leiloeiro e custos

16. **Credencia-se o LEILOEIRO pessoa física, não a plataforma** (IN DREI 52, art. 60 · Res. CNJ 236, arts. 1º e 2º). Due diligence por **nome + matrícula**, cruzando a lista do tribunal com a da Junta Comercial (a IN DREI 52, art. 89, VII obriga a publicar a **situação**: regular / licenciado / suspenso). **Procurar "a empresa" na Junta não devolve nada.**
17. **A escala de antiguidade NÃO se aplica a leilão judicial** (Dec. art. 43 · IN DREI 52, art. 71, §3º) — vale só nas vendas de bens da União/Estados/Municípios. Impugnar nomeação por "quebra de antiguidade" em execução cível é **tese perdida**.
18. **O emolumento de registro pode ser enquadrado por valor MAIOR que o lance** (base é o **maior** entre preço declarado, valor do IPTU e base do ITBI). **Arrematar com 50% de desconto não corta o emolumento pela metade.**

### Bloco pós-arrematação

19. **Assimetria de desocupação, a favor do extrajudicial:** Lei 9.514, art. 30 dá **liminar expressa + 60 dias** ao arrematante; o CPC 901, §1º **não tem prazo nem qualificação liminar**, e o mandado de imissão só sai **depois** de pagos preço, comissão, despesas e ITBI.
20. **⚠️ A armadilha dos 90 dias do locatário** (Lei 8.245, art. 8º): o arrematante tem **90 dias contados do REGISTRO da venda ou do compromisso** para denunciar a locação — **perdido o prazo, presume-se concordância com a manutenção do contrato**. 🔴 **CORRIGIDO 02/08:** este item dizia "contados da alienação". O **§2º** é literal — *"noventa dias contados do **registro** da venda ou do compromisso"* (verbatim em `context/lei-8245-locacao.md`). **O registro é posterior à alienação**, então o marco antigo declarava morto um prazo que ainda corre.

### ⭐ 21 — Postura honesta obrigatória (redação ATUALIZADA pela verificação em inteiro teor)

**(a) DÉBITO CONDOMINIAL — a premissa mudou.** Com o **edital informando** a dívida, o arrematante **RESPONDE** (*propter rem*) **+ sucessão processual** — orientação **CONSOLIDADA** (REsp 2.042.756/SP, mantido pelo **AgInt nos EREsp 2.042.756/SP, 2ª Seção, UNÂNIME, j. 13/05/2026**).

> 🚫 **PROIBIDO escrever "a matéria está em aberto no STJ"** — a Corte teve a via formal de uniformização e **a recusou**, por ausência de divergência atual. A brecha é o **edital OMISSO**, e é **tese de defesa**, jamais regra pacífica. **Tema 1.266 é matéria DIVERSA** — não citar como saída.

**(b) EVICÇÃO — o vácuo é real e permanece.** **Não existe julgado do STJ sobre evicção especificamente do arrematante em hasta pública.** A moldura é o **CC 447-457**, que é **lei, não jurisprudência confirmada**. Declarar o vácuo **no corpo da peça**.

---

## 7. AS 11 CORREÇÕES TRAVADAS (a fonte primária venceu a premissa)

| Nunca escreva | Escreva |
|---|---|
| "Tema 1.134 = condomínio propter rem" | **Tema 1.134 é exclusivamente TRIBUTÁRIO**; o acórdão **não trata** de despesas condominiais |
| "Súmula 121/STF é âncora de leilão" | **Súmula 121/STF = capitalização de juros** (anatocismo). **Súmula 128/STJ** é válida mas restrita à **execução fiscal** |
| "O STJ fixou tese de preço vil ≥50% no extrajudicial" | **REsp 2.165.101 é MONOCRÁTICA** — escreva ***"o STJ vem anulando"***, **NUNCA** "tese firmada em repetitivo" |
| "A comissão é de 5% por força do CPC" | O CPC **não fixa percentual** (884, §único). Os 5% vêm do **Decreto 21.981/32, art. 24, §único** e da **Res. CNJ 236, art. 7º** — e são **PISO** (§ abaixo) |
| "O art. 889 exige intimação do cônjuge sob pena de nulidade" | O **art. 889 tem 8 incisos fechados e NÃO lista o cônjuge** |
| "Leilão negativo sempre quita a dívida" | Fora do art. 26-A, o **§5º-A mantém o devedor obrigado pelo saldo** |
| "DL 70/66 residual" | Arts. **29-41 REVOGADOS**. Vive só como direito intertemporal e nos Caps. I e II |
| "Tema 982/STF julgado em 2024" | Mérito julgado em **26/10/2023**; 2024 é publicação (14/02) e trânsito (22/02) |
| "Tema 1.288/STJ julgado em 19/02/2026" | Julgado em **10/12/2025**, publicado 17/12/2025, **trânsito em 15/06/2026** |
| "Existe canal de leilão com milhões de inscritos" | **Não confirmado.** A viralidade vem do **volume de plataformas (8 SaaS) e cursos (R$ 617–5.900)** |
| "O IPTU e as taxas condominiais do fiduciante estão no **art. 24, §2º**" · "a MP 1.162/2023 **não vingou**" | 🚫 **PROIBIDO dizer que a MP não vingou — ela FOI CONVERTIDA na Lei 14.620/2023.** Morreu o **ENDEREÇO**, não a regra. O endereço a citar é o **art. 23, §2º da Lei 9.514** (Incluído pela **Lei nº 14.620, de 2023**), **vigente**: *"Caberá ao fiduciante a obrigação de arcar com o custo do pagamento do Imposto sobre a Propriedade Predial e Territorial Urbana (IPTU) incidente sobre o bem e das taxas condominiais existentes."* **Prova:** o cabeçalho da própria MP no Planalto diz **"Convertida na Lei nº 14.620, de 2023"**. ⚠️ **A armadilha:** o texto compilado exibe **TAMBÉM** um art. 24, §2º com a mesma regra, mas com atribuição **apenas da MP** — logo **sem eficácia** —, e quem `grep`a "IPTU" na 9.514 **acha os dois**. **Cite o endereço da lei de conversão (23, §2º), nunca o da MP.** ⚠️ **Limite honesto:** o art. 23, §2º rege **fiduciante × fiduciário** e **NÃO resolve sozinho a dívida do arrematante** — para o arrematante valem a regra do **condomínio** (§6, verdade 21-a) e o **Tema 1.134**. Explicação canônica: `lei-9514-consolidada.md` **AVISO 3** |

> **São 11 correções.** Se alguma skill precisar escrever o número, escreve **11**.

### ⭐ A 12ª trava, vinda da verificação em inteiro teor: COMISSÃO

**5% é PISO, não teto — e NÃO EXISTE TETO.** RMS 65.084/SP (4ª T, unânime, j. 27/06/2023, trânsito 14/09/2023) reafirmando **REsp 680.140/RS** (*"não há limitação quanto ao percentual máximo"*; **10% validado**). **7% em leilão JUDICIAL é lícito.** A IN DREI 52, art. 75, II, "a" lê-se como vedação a cobrar **ABAIXO** do mínimo.

**Três resíduos obrigatórios:** (a) **não existe ato do DREI** dizendo isso expressamente — risco disciplinar formal não zerado; (b) **no EXTRAJUDICIAL o raciocínio NÃO se transporta** (não há juiz arbitrando) — **sem julgado localizado**; (c) são **acórdãos de turma, não repetitivos**.

> ⚠️ **Ao citar o precedente-matriz use REsp 680.140/RS.** A ementa do RMS 65.084 traz "640.140" por **erro de digitação do próprio STJ** — não reproduzir.

---

## 7.1 🚨 HOMÔNIMO DE CRITÉRIO — percentuais que NÃO se comparam

Há **duas** classes de homônimo neste plugin. A de **numeração** (dois "art. 27", dois "art. 26") o `audit/check-colisao-artigos.sh` detecta. **A de CRITÉRIO nenhuma ferramenta pega** — e aqui ela decide **quanto o cliente paga**.

> ⛔ **O número do percentual não diz nada sozinho. O que decide é a BASE DE CÁLCULO.** Dois "20%" com bases diferentes dão valores diferentes. **Sempre escreva o percentual COM a base colada.**

### Os três "20%" — bases diferentes

| Percentual | **Base de cálculo** | Onde | O que é |
|---|---|---|---|
| **20%** | **da AVALIAÇÃO** | CPC 896, §2º | multa do **pretendente que se arrepende** (imóvel de incapaz; em benefício do incapaz) |
| até **20%** | **do valor ATUALIZADO do bem** | CPC 903, §6º | sanção por **vício infundado** (ato atentatório à dignidade da justiça) |
| **20%** | **do LANCE ou proposta** | cláusula de edital *(E3)* | perda em favor do **vendedor** por não pagamento |
| **20%** | **caução no ato** | cláusula de edital *(ARM-12)* | **não é multa** — é depósito prévio |

⚠️ **Avaliação e lance não são o mesmo número** — num bem arrematado a 50% da avaliação, "20% da avaliação" é **o dobro** de "20% do lance". Trocar a base **dobra ou reduz pela metade** o que o cliente deve.

### Os dois "50%" — e um deles NÃO é piso

| "50%" | O que realmente é |
|---|---|
| **50% da avaliação** | **preço vil** — regra **supletiva** quando o juiz não fixou preço mínimo (CPC) |
| **50%** no 2º leilão | 🔴 **FACULDADE DO CREDOR**, a seu exclusivo critério (Lei 9.514, art. 27, §2º · Lei 14.711, art. 9º, §6º) — **NÃO é piso de vileza e NÃO é direito do arrematante** |

### Os "5%" — comissão × despesas, e o edital que soma os dois

| "5%" | Base |
|---|---|
| **comissão do leiloeiro** | sobre o **valor da arrematação** — é o **piso**; há edital cobrando **7%** |
| **despesas** | sobre o **valor do arremate** — cláusula de edital *(E1)*, **cumulativa com a comissão** ⇒ **10% somados** |

**Regra operacional:** ao ler qualquer percentual, **anote a base junto do número**. Antes de comparar dois percentuais, confirme que **incidem sobre a mesma base**. Se não incidirem, **não se somam nem se comparam** — e no cálculo do preço-teto do arrematante **entram todos, cada um sobre a sua própria base**.

🟡 **Não localizado neste corpus:** o "1% a 5% do valor da causa" (multa do agravo interno). **Não afirmar** que consta aqui — se for necessário, capturar antes.

---

## 8. OS SELOS E A RÉGUA DE POSTURA HONESTA

| Selo | Significa | Como se escreve |
|---|---|---|
| **✅** | Ancorado em fonte oficial | Cita direto, com número, turma, relator e data |
| **🟡** | Conferir antes de peça | **Nunca vira afirmação categórica e nunca some.** Afirma o que está provado → marca o que não está → diz o que conferir → roteia ao `validador-leiloes` |
| **🔴** | Novidade pós-cutoff · verdade dura · pendente · monocrático | Traz a qualificação junto (*"decisão monocrática"*, *"turma, não repetitivo"*, *"pendente de julgamento"*) |

**A régua de escrita para item 🟡** — quatro movimentos, nesta ordem:

```
1. AFIRMA o que está provado          ("a fórmula do STJ é condicionada ao edital que informa")
2. MARCA o que não está                ("a proposição inversa não foi localizada em acórdão do STJ")
3. DIZ o que conferir                  ("abrir o inteiro teor do REsp 1.299.081/SP")
4. ROTEIA                              ("→ validador-leiloes antes de protocolar")
```

> ⭐ **É esse comportamento que os 8 SaaS concorrentes não têm** — eles dão resposta binária errada. **É diferencial de produto, não fraqueza.**

---

## 9. 🟡 CONTRATO DE ANTI-ALUCINAÇÃO — o que é PROIBIDO afirmar sem verificação

Toda skill que tocar um item abaixo carrega, no corpo, a ressalva **"🟡 conferir o inteiro teor antes de protocolar"** + **o que exatamente falta** + o roteamento. **O guard bloqueia a afirmação seca.**

### Os itens que TOCAM PEÇA

| Item | O que não está provado |
|---|---|
| **Edital omisso ⇒ arrematante não responde por condomínio** | Inferência ***a contrario***. Nenhum acórdão do STJ afirma a proposição inversa; há **REsp 1.299.081/SP** em sentido contrário (falimentar, inteiro teor não aberto). **Tese de defesa, jamais regra** |
| **Data da "publicação da ata de julgamento"** do Tema 1.134 | O acórdão fixa o marco mas **não declara a data**. A praxe usa 24/10/2024 — **convenção, não texto** |
| **Comissão acima de 5% no EXTRAJUDICIAL** | Nenhum julgado localizado; o raciocínio do RMS 65.084 **não se transporta** |
| **Ato do DREI** harmonizando o art. 75, II, "a" | **Inexistente** até onde se buscou; risco disciplinar formal do leiloeiro não zerado |
| **Regime de evicção do arrematante** | **Nenhum julgado do STJ específico de hasta pública.** Os dois destacados tratam de **compra e venda**. A moldura é o CC 447-457 — **lei, não jurisprudência** |

### Os demais

`pas de nullité sans grief no leilão judicial` (só snippets; tensão real com a linha do extrajudicial — **não presumir o recorte**; e o CPC 804 fala em **ineficácia**, que não depende de grief) · `número do Tema do IPTU do fiduciante ("1.158")` (veio de busca, não da ficha — citar o REsp, não o Tema) · `revogação da IN DNRC 113/2010` (o achado é **desatualização da fundamentação**, não nulidade provada) · **`alíquotas municipais de ITBI · emolumentos fora de SP · custas judiciais`** (**NUNCA dar número — dar a fórmula e a fonte a consultar**) · `Tema 1.113 (ITBI)` (sem trânsito; **não é sobre arrematação**) · `direito intertemporal do DL 70/66` (a 14.711 **não traz regra de transição**) · `regulamentação registral do art. 9º da 14.711` (provimentos de corregedoria e normas estaduais **não verificados** — **operacionalmente decisivo**) · `números de REsp de fonte secundária` (nenhum inteiro teor aberto — lista em `jurisprudencia-leiloes.md` §11) · `prisão do leiloeiro como depositário remisso` (Dec. art. 27, §4º × **SV 25/STF** não verificada — **não usar em peça**) · `legitimidade do arrematante terceiro para cobrar a taxa de ocupação` (9.514, art. 37-A) · `incremento mínimo do lance` (**nenhuma das 5 plataformas publica** — **impossível calcular de antemão** o custo de cobrir um lance) · `tese literal e dispositivo das ADIs 7600/7601/7608` (citar **as balizas de conduta**, que são verificáveis, não a "tese literal").

### As proibições absolutas do guard

1. ⛔ **Afirmar situação do imóvel sem documento lido** (ocupação, ônus, área, débito, regularidade).
2. ⛔ **Escrever "a matéria está em aberto no STJ"** sobre débito condominial.
3. ⛔ **Chamar decisão monocrática de "tese firmada em repetitivo"**.
4. ⛔ **Citar pendente como decidido** (REsp 2.171.564/SP · Tema 1.266 · EDcl de 06/08/2026).
5. ⛔ **Dar número de alíquota de ITBI, emolumento fora de SP ou custas judiciais.**
6. ⛔ **Ensinar o DL 70/66, arts. 29-41, como rito vigente.**
7. ⛔ **Prometer desconto de 70%** (média provada: 37,3%) ou dizer que **"leilão é seguro"**.

---

## 10. ⏰ O RELÓGIO DO LEILÃO — prazos críticos

| Prazo | Marco inicial (*dies a quo*) | Base |
|---|---|---|
| **10 dias** — invalidação · ineficácia · resolução; e as 3 portas de desistência | **APERFEIÇOAMENTO** (assinatura do auto) — **não** a ciência do vício | CPC 903, §§1º-2º e §5º |
| **5 dias** — publicação do edital antes do leilão | Data do leilão, para trás | CPC 887 |
| **5 dias** — ciência das 8 categorias do art. 889 | Data do leilão, para trás | CPC 889 |
| **5 dias** — abertura do leilão eletrônico | Data do leilão, para trás | Res. CNJ 236, art. 11 |
| **3 minutos / 15 segundos** — prorrogação automática | Cada lance nos minutos finais | Res. CNJ 236, art. 21 |
| **1 dia** — depósito pelo leiloeiro · **2 dias** — prestação de contas | Recebimento | CPC 884 |
| **15 dias** — intimação da mora | Recebimento da intimação | 9.514, art. 26 |
| **15 dias** — intimação **eletrônica** antes do edital ⭐ | Contato eletrônico previsto no contrato | 9.514, art. 26, §4º-B |
| **Purga até a AVERBAÇÃO** da consolidação (imóvel residencial) + 30 dias do §1º | Averbação | 9.514, art. 26-A, §§1º-2º |
| **60 dias** — 1º leilão · **15 dias** — 2º leilão | Consolidação | 9.514, art. 27 · 14.711, art. 9º, §§3º e 6º |
| **Preferência até a data do 2º leilão** | — | 9.514, art. 27, §2º-B |
| **5 dias** (AF) · **15 dias** (hipoteca 14.711) — entrega do excedente | Alienação | 9.514, art. 27, §4º · 14.711, art. 9º, §8º |
| **30 dias** — excussão sucessiva | — | 9.514, art. 27-A, §3º |
| **60 dias** — desocupação após reintegração **liminar** | Concessão da liminar | 9.514, art. 30 |
| **90 dias** ⚠️ — denúncia da locação pelo arrematante | **REGISTRO da venda ou do compromisso** (§2º, verbatim) — **não** a alienação; perdido, presume-se manutenção do contrato | Lei 8.245, art. 8º, §2º |
| **30/90 dias** — denúncia da locação no extrajudicial | — | 9.514, art. 27, §7º |
| **1%/mês** — taxa de ocupação | **CONSOLIDAÇÃO** (não o leilão) até a imissão | 9.514, art. 37-A |
| **180 dias** — venda direta com mandato irrevogável *ex lege* | — | 14.711, art. 9º, §9º, II |

> 🚨 **Os dois marcos que mais derrubam peça:** o **aperfeiçoamento** (10 dias do 903 §2º — não a ciência) e o **REGISTRO da venda ou do compromisso** (90 dias do locatário — **não a alienação**, não a arrematação, não a imissão). 🔴 **CORRIGIDO 02/08:** este callout dizia "a **alienação**" e contradizia a própria tabela acima — o §2º é literal (verbatim em `context/lei-8245-locacao.md`), e como o registro é **posterior** à alienação, o marco antigo declarava morto um prazo que ainda corre.

---

## 11. 🔴 GATE DE CALENDÁRIO — antes de publicar e a cada atendimento sensível

| O que | Data / estado | Efeito |
|---|---|---|
| **EDcl no AgInt nos EREsp 2.042.756/SP** | **Pautado para 06/08/2026** (2ª Seção, sessão virtual) | Incide sobre **admissibilidade**, não sobre o mérito — mas o resultado entra na skill de condomínio |
| **REsp 2.171.564/SP** (ex-AREsp 2.471.891) | No gabinete da Min. Daniela Teixeira desde 06/03/2025; última fase 24/06/2025 | Se julgado e a resposta for "sim, o art. 886, VI se aplica ao extrajudicial", **abala editais já realizados** |
| **Tema 1.266/STJ** | Afetado, **sem suspensão nacional** | Se julgado, atualizar a **distinção** (é matéria diversa) |
| **Vigência da Res. CNJ 236/2016** | Campo "Alteração" **vazio** na ficha oficial em 02/08/2026 | Provimentos de corregedoria **estaduais** complementam e **variam por tribunal** — conferir o local |

---

## 12. FRONTEIRAS — cross-link soft, NUNCA duplicar

| Plugin | Quem é dono do quê | Como o `leiloes` se comporta |
|---|---|---|
| `execucao-adv-os` | Execução **até a penhora** | `leiloes` assume da **expropriação em diante** |
| `direito-imobiliario-adv-os` | A **relação** de AF (contrato, revisão) e o registral | `leiloes` é dono da **mecânica do leilão** e da **ótica do arrematante** |
| `civel-adv-os` | Visão geral processual | A C7 daqui é **modelada** no cível, **standalone** |
| `licitacoes-adv-os` | Tudo que é Lei 14.133 | Leilão público administrativo é **GAP DECLARADO**: reconhecer e encaminhar, **nunca improvisar** |
| `transito-adv-os` | Defesa do **proprietário** contra remoção e leilão de veículo | CTB 328 entra como **ponteiro** |
| `agrario-adv-os` | A **especificidade da terra** | ⚓ Âncora dura: **o art. 9º, §13, da 14.711 exclui expressamente o financiamento da atividade agropecuária do rito novo.** Há divergência aberta entre TJs sobre arrendamento rural e hasta pública — **ponteiro, nunca resposta** |
| `bancario-adv-os` | A relação com o banco | Cross-link quando o fiduciante quer discutir o **contrato**, não o leilão |
| `calculosjudiciais-adv-os` | O cálculo | Aqui se monta a **estrutura** da conta; o cálculo de saldo/atualização cruza para lá |
| `tributario-societario` / `cfo-combativo-os` | ITBI como tributo · ganho de capital na revenda | Ponteiro a partir do registro/ITBI |

---

## 13. MAPA DOS 11 ANEXOS `context/` — zero dead-ref

> 🔴 **Atualizado 02/08: são 11, não 10.** O 11º é **`lei-8245-locacao.md`** (Lei 8.245/91 — locações), capturado para fechar o marco dos 90 dias do locatário: o **art. 8º, §2º** conta do **REGISTRO da venda ou do compromisso**, **não da alienação**. Ele é consumido por `situacao-possessoria`, `desocupacao-locacao-e-ocupantes`, `defesa-contra-imissao-e-embargos-de-terceiro` e pelas skills de C0/C1 que travam o marco.

| Anexo | O que traz |
|---|---|
| `cpc-leilao-879-903.md` | Verbatim dos arts. 876-903 + 804 + 826 + 890 + 908 §1º |
| `resolucao-cnj-236-2016.md` | Verbatim dos 36 artigos + ficha oficial |
| `lei-9514-consolidada.md` | Arts. 24 a 39 consolidados pós-14.711, com o que mudou e o que foi revogado |
| `lei-14711-2023.md` | Arts. 9º e 10 verbatim + art. 18 (revogações) + o aviso da morte do DL 70/66 arts. 29-41 |
| `leiloeiro-decreto-21981-in-drei-52.md` | Decreto 21.981/32 + IN DREI 52/2022, com o mapa norma viva × norma morta |
| **`jurisprudencia-leiloes.md`** | Corpus **✅-only** + **LISTA NEGRA** + **PENDENTES** + bloco **🟡** + gate de calendário |
| **`clausulas-armadilha-de-edital.md`** | As **16 cláusulas** de editais reais + a auditoria do **art. 886 inciso a inciso** |
| **`custo-total-do-arrematante.md`** | A conta completa (12 linhas) + a **fórmula do teto de lance** + emolumentos pela maior base |
| **`mercado-leiloes-2026.md`** | Volume, deságio, os 8 SaaS, vocabulário, honorários de assessoria e as travas de copy |
| **`metodologia-leiloes.md`** | Este arquivo |

---

## 14. TOM — o que NUNCA sai da boca deste plugin

Direto, sem promessa.

- ❌ **"leilão é seguro"**
- ❌ **"70% de desconto garantido"** (a média provada é **37,3%**)
- ❌ **"essa arrematação nunca cai"**
- ❌ **"cai como qualquer negócio"**
- ❌ resposta única onde a jurisprudência é **condicionada, monocrática ou ausente**

> Onde a jurisprudência está rachada ou ausente — **condomínio com edital omisso, evicção, comissão no extrajudicial** —, **dizer que está**.
