# Custo total real do arrematante — a conta inteira, não o lance

> Anexo de prática do plugin **leiloes-os**. É a base da skill `custo-total-real-e-precificacao` e da conta que fecha o `parecer-go-nogo-lote`.
> **Regra deste arquivo: só entra o que tem fonte.** Onde o número varia por ente federativo (alíquota de ITBI, emolumentos fora de SP, custas judiciais), este anexo dá **a fórmula e a fonte a consultar** — **nunca o número**.
> **Captura:** Planalto, STJ, tabela de emolumentos SP 2026, termos de uso e editais reais de plataformas, em **02/08/2026**.
> **Como usar:** `grep` pela linha de custo (`comissão`, `ITBI`, `emolumento`, `carrego`, `taxa de ocupação`) e **leia a faixa**.

---

## 0. ⛔ AS QUATRO TRAVAS DESTE ANEXO

1. **O lance é a MENOR parte da conta.** Um lance de **R$ 1.000.000** custa **R$ 1.050.000** só de lance + comissão a 5%, **antes** de ITBI, emolumentos, carrego, desocupação e reforma.
2. **NUNCA dar número de alíquota de ITBI, de emolumento fora de São Paulo ou de custas judiciais.** Esses valores **variam por município e por estado** e não foram pesquisados. Dar **a fórmula + a fonte a consultar**. Inventar número aqui é alucinação que vira prejuízo.
3. **O que se entrega é o TETO DE LANCE, não o "desconto".** O deságio anunciado encolhe — às vezes desaparece — nesta conta.
4. **Documento faltando ⇒ a conta não fecha ⇒ NO-GO por insuficiência de prova.** Não estimar débito, ocupação ou área "por alto" para completar a planilha.

---

## 1. ⭐ A FÓRMULA DO TETO DE LANCE

```
        VALOR DE MERCADO LÍQUIDO ESPERADO
      − comissão do leiloeiro (% do EDITAL, por fora)
      − ITBI (alíquota municipal × base da arrematação)
      − emolumentos de registro (pela MAIOR base — §5)
      − laudêmio, se imóvel foreiro
      − encargos de administração da plataforma
      − débitos condominiais que o edital informa (§6)
      − carrego: meses até a posse × (cota + IPTU)   (§7)
      − custo de desocupação: honorários + tempo      (§8)
      − reforma / regularização (cenário pessimista)  (§10)
      − honorários do pós-arrematação                 (§11)
      + taxa de ocupação recuperável, se extrajudicial (§9 — CRÉDITO)
      ─────────────────────────────────────────────────
      = TETO DE LANCE
```

> **Regra operacional que evita o erro mais caro:** a comissão é **somada por fora**, então **lance o teto MENOS a comissão**, nunca o teto cheio. Quem lança o teto cheio já estourou o orçamento no martelo.

---

## 2. COMISSÃO DO LEILOEIRO — por fora, e o piso é 5% (não o teto)

**Base legal:** CPC art. 884, §único — *"O leiloeiro tem o direito de receber do arrematante a comissão estabelecida em lei ou arbitrada pelo juiz."* **O CPC não fixa percentual.** O piso vem do art. 24, §único, do Decreto 21.981/1932 e do art. 7º da Res. CNJ 236/2016 ("no mínimo 5%").

**É acréscimo ao preço, não parcela dele** — o edital diz com todas as letras:

> **[E1]:** "A comissão do leiloeiro **não está inclusa no valor do lance** e não será devolvida ao arrematante em nenhuma hipótese, salvo se a arrematação for desfeita por determinação judicial, por razões alheias à vontade do arrematante."

### 🚨 5% é PISO, não teto — e NÃO EXISTE TETO

| Comando | Leitura confirmada |
|---|---|
| Decreto 21.981/32, art. 24, §único ("obrigatoriamente 5%") | **Piso** — RMS 65.084/SP (4ª T, unânime, j. 27/06/2023) reafirmando **REsp 680.140/RS** |
| Percentual máximo | **NÃO EXISTE** — *"não há limitação quanto ao percentual máximo"*; **10% validado** |
| **7% em leilão judicial** (edital real [E2]) | **LÍCITO** — acima do piso, arbitrado na moldura do CPC 884, §único |
| Comissão **abaixo** de 5% | **Ilegal** — o leiloeiro tem direito à complementação |

> ⚠️ **Ao citar o precedente-matriz use REsp 680.140/RS** (a ementa do RMS 65.084 traz "640.140" por erro de digitação do próprio STJ). Detalhes, resíduos e o eixo temporal de impugnação: `jurisprudencia-leiloes.md` §5.

**Para a conta, o que importa:** **ler o percentual em CADA edital**. Não assumir 5%. A diferença entre 5% e 7% em um imóvel de R$ 500 mil é **R$ 10.000**.

### Quando a comissão é devida e quando não é (Res. CNJ 236, art. 7º)

| Situação | Comissão | Base |
|---|---|---|
| Resultado **negativo** da hasta | **Não** devida | art. 7º, §1º |
| **Anulação** da arrematação | **Não** devida — e o já pago é **devolvido corrigido** | art. 7º, §§1º e 2º |
| **Desistência do exequente** (CPC 775) | **Não** devida — devolução corrigida | art. 7º, §§1º e 2º |
| **Acordo ou remição APÓS a alienação** | **Devida** | art. 7º, §3º |
| Arrematação **maior** que o crédito do exequente | Pode ser **deduzida do produto** | art. 7º, §4º |
| Remoção/guarda após substituição de penhora, conciliação, pagamento, remição ou adjudicação | O **executado** ressarce as despesas | art. 7º, §7º |

**🔴 Reforço de 2026:** o STJ decidiu (3ª Turma, **REsp 2.198.525**, Rel. Min. Ricardo Villas Bôas Cueva, julho/2026) que a **remição posterior ao lance e anterior à assinatura do auto NÃO afasta a comissão** — a arrematação já existe com a aceitação do lance e o depósito do preço. **Turma, não repetitivo.** Não alcança leilão negativo nem acordo **anterior** ao pregão.

### No extrajudicial da Lei 9.514, a comissão aparece duas vezes — e não pode ser cobrada duas vezes

O art. 27, §3º, II, inclui a comissão do leiloeiro no conceito de **"despesas"**, que se abatem do produto antes de apurar o saldo do fiduciante. Na prática, o edital cobra 5% **do arrematante, por fora**. As duas coisas convivem: o arrematante paga por fora, e o que **o credor** gastou entra na conta de acerto com o devedor.

> ⚠️ **Munição para quem ataca a prestação de contas do credor fiduciário:** a comissão **paga pelo arrematante** não pode ser lançada **outra vez** como despesa do credor contra o fiduciante. 🟡 **Nenhum julgado localizado** sobre essa dupla contagem — é argumento de prestação de contas, não de precedente.

---

## 3. ENCARGOS DE PLATAFORMA — a linha que ninguém soma

- **Uma das cinco plataformas verificadas cobra encargos de administração em tabela fixa por faixa de lance — de R$ 35,00 a R$ 65.000,00** — expressamente *"não inclusos no valor do lance"* e **somados** à comissão de 5%. A mesma plataforma **veda PIX**.
- Em leilão de **veículos**, outra plataforma publica tabela de despesas de depósito (ordem de grandeza: moto ~R$ 550 · leve ~R$ 2.350 · pesado ~R$ 4.900 · estadia ~R$ 50/dia após 5 dias úteis) — **custo invisível no lance**.
- **🔴 Nenhuma das cinco plataformas publica o incremento mínimo do lance.** É parâmetro definido **lote a lote no sistema**. **É impossível calcular de antemão o custo de cobrir um lance** — a skill de estratégia deve dizer isso, não estimar.

**Gargalo operacional que muda a conta de tempo:** **cadastro não é habilitação**. Todas exigem habilitação **por leilão**. E o gargalo real é a **validação do cadastro** — uma plataforma avisa que a validação *"tem prazo de até 3 (três) dias úteis para ser **iniciada**"*. **Quem descobre o lote na véspera não consegue dar lance.**

---

## 4. ITBI — base é o valor da hasta, e a sequência é invertida

- **Base de cálculo:** o STJ entende que na arrematação a base do ITBI é o **valor alcançado em hasta pública**, não o venal — **REsp 1.188.655/RS**, Rel. Min. Luiz Fux, 1ª Turma, j. 20/05/2010: *"a arrematação representa a aquisição do bem alienado judicialmente, considerando-se como base de cálculo do ITBI aquele alcançado na hasta pública."*
- **⚠️ É jurisprudência de TURMA, não tese vinculante.** **Não existe tese repetitiva sobre ITBI em arrematação.** E o **Tema 1.113 NÃO é sobre arrematação** — é ITBI em geral, sem trânsito em julgado (RE 1.412.419 concluso no STF). Ver `jurisprudencia-leiloes.md` §2 e §9.
- **🟡 Alíquota:** **varia por município e NÃO foi pesquisada.** **Nunca dar o número.** Dar a fórmula (**alíquota municipal × base da arrematação**) e mandar consultar a **legislação do município do imóvel**.

### 🚨 A ARMADILHA DE SEQUÊNCIA — o ITBI é pago ANTES de você ter o título

O **CPC art. 901, §2º** exige que a carta de arrematação contenha *"a prova de pagamento do imposto de transmissão"*. E o **§1º** condiciona a carta e o mandado de imissão ao depósito do preço **+ comissão + despesas**.

```
pagar preço  →  pagar comissão  →  pagar despesas  →  pagar ITBI
                                                          ↓
                                                    CARTA de arrematação
                                                          ↓
                                                 MANDADO de imissão na posse
```

> **Consequência de fluxo de caixa:** o arrematante desembolsa **tudo** antes de ter título e antes de ter posse. Quem planejou pagar o ITBI "depois, com o aluguel do imóvel" trava a própria carta.

**No extrajudicial**, a Lei 14.711/2023, art. 9º, §14, coloca ITBI e laudêmio **antes do registro** — mesma lógica.

---

## 5. EMOLUMENTOS DE REGISTRO — pela MAIOR base, não pelo lance

**A regra que quebra a intuição:** em São Paulo, o **art. 7º da Lei Estadual 11.331/2002** manda usar o **MAIOR** entre:

1. **preço declarado** (o lance),
2. **valor tributário do IPTU**,
3. **base de cálculo do ITBI**.

E o parágrafo único manda usar o **valor da avaliação judicial** quando a lei assim exigir.

> 🚨 **Arrematar com 50% de desconto NÃO corta o emolumento pela metade.** Se o IPTU ou a base do ITBI forem maiores que o lance, é por eles que a faixa é enquadrada. Esta é uma das linhas que mais destrói margem em lote de deságio alto.

**Ordem de grandeza (Tabela II dos Ofícios de Registro de Imóveis — SP, 2026), item "Registro com valor declarado":**

| Faixa de valor | Emolumento (ordem de grandeza) |
|---|---|
| R$ 38.420,01 – 115.260,00 | ~R$ 1.483,46 |
| R$ 384.200,01 – 768.400,00 | ~R$ 3.284,18 |
| R$ 1.152.600,01 – 1.536.800,00 | ~R$ 4.427,79 |

**🟡 Três limites honestos, obrigatórios ao citar esta tabela:**

1. **Só São Paulo foi verificado.** Emolumentos são **estaduais** — para qualquer outro estado, **dar a fórmula e mandar consultar a tabela da corregedoria/associação de registradores local**. Nunca extrapolar os valores de SP.
2. **Não existe item de tabela nominado "carta de arrematação"** — foi usado o item genérico de registro com valor declarado.
3. As faixas entre **R$ 192.100,01 e R$ 345.780,00** vieram com **OCR corrompido** na captura e **não são reproduzidas**. Conferir no PDF original.

**Somar ainda:** laudêmio, quando o imóvel for **foreiro** (enfiteuse / terreno de marinha) — incide na transferência e pode somar dezenas de milhares. Checar **na matrícula**.

---

## 6. DÉBITOS ANTERIORES — dois regimes que NÃO se misturam

### ✅ Tributário — fechado A FAVOR do arrematante

**Tema 1.134/STJ** (transitado em julgado em 12/12/2024): é **inválida** a cláusula de edital que atribui ao arrematante os débitos **tributários** anteriores. Sub-rogação **sobre o preço** (CTN art. 130, §único):

> "Art. 130. […] Parágrafo único. No caso de arrematação em hasta pública, a sub-rogação ocorre sôbre o respectivo preço."

**Na conta: R$ 0** de tributo anterior — **desde que** o edital tenha sido **publicizado após a publicação da ata de julgamento** do repetitivo (modulação), **ou** haja ação judicial / pedido administrativo já pendente (aplicação imediata).

> ⚠️ **A data da ata NÃO é declarada na fonte.** A praxe usa 24/10/2024 (publicação do acórdão) — **é convenção, não texto**. Ver `jurisprudencia-leiloes.md` §3.

**Achado de campo:** **nenhum dos três editais** analisados joga tributo anterior no arrematante — **o mercado já se ajustou**. Encontrar um que jogue é **anomalia** e cláusula inválida.

### 🚨 Condominial — regime OPOSTO, e a conta pode inverter o negócio

**Com o edital INFORMANDO a dívida, o arrematante RESPONDE** (*propter rem*) **e sofre sucessão processual** — orientação **consolidada** (REsp 2.042.756/SP, mantido pelo **AgInt nos EREsp 2.042.756/SP, 2ª Seção, UNÂNIME, 13/05/2026**). **Proibido escrever "a matéria está em aberto no STJ".**

**O número real de um edital analisado:** débito condominial de **R$ 53.374,15 + R$ 5.337,41 de honorários**, sobre avaliação de **R$ 136.142,37** — **39% da avaliação**.

> 🚨 **É a linha que mais inverte o sinal do negócio.** Um lote com 37% de deságio e 39% de dívida condominial informada no edital **não é oportunidade — é prejuízo**. Ler a cláusula de débitos condominiais **antes do lance** decide a responsabilidade.

**A cláusula de sub-rogação no edital não é garantia:** a proteção do **CPC 908, §1º** depende de o crédito estar **documentalmente comprovado e habilitado**. Se o condomínio **não se habilitar**, a natureza *propter rem* puxa o débito para o imóvel.

**Edital omisso** ⇒ leitura *a contrario* (CPC 908, §1º) é **tese de defesa bem fundamentada**, com lastro de 2º grau — **jamais regra pacífica**. Detalhes e o precedente contrário: `jurisprudencia-leiloes.md` §4.

**Na conta:** lançar o **valor integral informado no edital** como custo certo; se o edital for omisso, lançar como **risco quantificado** (obter declaração de débito da administradora) — **nunca como R$ 0**.

---

## 7. CARREGO — o custo que corre enquanto você não pode usar o imóvel

Os editais são explícitos em fazer o relógio virar **na arrematação**, não na posse:

> **[E3]:** "Todos os tributos e demais encargos, incidentes sobre o imóvel em questão, **inclusive encargos condominiais, após a data da efetivação da arrematação são de responsabilidade exclusiva do arrematante**."

```
CARREGO = (meses estimados até a POSSE) × (cota condominial + IPTU mensal)
```

> **É a linha mais esquecida da conta.** Em imóvel ocupado com resistência, "meses até a posse" não é 2 — pode ser 12 ou mais, e a estimativa tem de vir da apuração de **quem** ocupa, não de um chute.

---

## 8. DESOCUPAÇÃO — a assimetria que muda o prazo e o custo

| | **Judicial (CPC 901, §1º)** | **Extrajudicial (Lei 9.514, art. 30)** |
|---|---|---|
| Instrumento | Mandado de imissão **nos próprios autos** | **Ação própria** de reintegração |
| Liminar | **Não há qualificação liminar no texto** | **Liminar EXPRESSA** |
| Prazo legal | **Não há** | **60 dias** para desocupação |
| Pré-requisito | Só após pagos **preço + comissão + despesas + ITBI** | Comprovada a **consolidação** da propriedade |

**Texto do art. 30 (redação da Lei 14.711/2023):**

> "É assegurada ao fiduciário, ao seu cessionário ou aos seus sucessores, **inclusive ao adquirente do imóvel por força do leilão público** […] a reintegração na posse do imóvel, que será concedida **liminarmente**, para desocupação no prazo de **60 (sessenta) dias** […]"

> 🔴 **A assimetria favorece o extrajudicial** — e quase ninguém precifica isso. Mas **estatística de cumprimento real não foi pesquisada**: liminar concedida não é imóvel vazio. Orçar honorários de imissão/reintegração **sempre**.

**⚠️ A armadilha dos 90 dias do locatário** (Lei 8.245, art. 8º): havendo locação, o arrematante tem **90 dias contados do REGISTRO da venda ou do compromisso** para denunciá-la. **Perdido o prazo, presume-se concordância com a manutenção do contrato** — e o imóvel vem com inquilino até o fim do contrato. 🔴 **CORRIGIDO 02/08 — este parágrafo dizia "contados da alienação" e o marco estava ERRADO.** O **§2º** é literal: *"A denúncia deverá ser exercitada no prazo de noventa dias contados do **registro da venda ou do compromisso**"* (verbatim em `context/lei-8245-locacao.md`). **O registro é POSTERIOR à alienação** — contar da alienação **declara morto um prazo que ainda corre** e faz o arrematante desistir da denúncia sem precisar.

---

## 9. TAXA DE OCUPAÇÃO — é CRÉDITO do arrematante, não custo

**Lei 9.514/97, art. 37-A** (redação da Lei 14.711/2023):

> "Art. 37-A (Lei 9.514). O fiduciante pagará ao credor fiduciário **ou ao seu sucessor**, a título de taxa de ocupação do imóvel, por mês ou fração, valor correspondente a **1% (um por cento)** do valor de que trata o inciso VI do *caput* ou o parágrafo único do art. 24 desta Lei, computado e exigível **desde a data da consolidação da propriedade fiduciária** no patrimônio do credor fiduciário **até a data em que este ou seu sucessor vier a ser imitido na posse** do imóvel."

- **É obrigação do FIDUCIANTE**, em favor do credor **ou seu sucessor** — logo, **potencial crédito do arrematante**, não despesa.
- **O marco inicial é a CONSOLIDAÇÃO**, não a data do leilão.
- **🟡 A legitimidade do arrematante terceiro para cobrá-la NÃO foi pesquisada.** Lançar na conta como **crédito eventual**, com a ressalva — nunca como receita certa que financia o lance.

---

## 10. REFORMA E REGULARIZAÇÃO

Com **ARM-01** (sem garantia) e **ARM-02** (renúncia a vício oculto) no edital, o custo de reforma é **integralmente** do arrematante, sem recurso contra vendedor ou leiloeiro.

- Orçar no **cenário pessimista** — o imóvel muitas vezes não pôde ser vistoriado por dentro.
- **Regularização** (construção não averbada, habite-se ausente, divergência de área) tem custo próprio: **projeto + INSS + averbação**. É também o que **destrava financiamento e revenda** — sem isso, o comprador seguinte não consegue crédito, e a saída do investimento fica presa a compradores à vista.

---

## 11. HONORÁRIOS DO PÓS-ARREMATAÇÃO — custo de aquisição, não extra

O edital diz, em letras próprias, que o arrematante fica sozinho:

> **[E1]:** "o Leiloeiro é auxiliar da justiça e **está impedido de atuar nessa esfera** […] O acompanhamento e o procedimento pós leilão será de Responsabilidade do Arrematante […] deverá acompanhar e solicitar ao juízo responsável a expedição da Carta de arrematação e Imissão na posse […]"

**O que entra no escopo do pós:** carta de arrematação · ITBI · registro · baixa de gravames · imissão na posse · eventual defesa em cobrança de débitos.

**Faixas praticadas no mercado de assessoria de arrematação** (🟡 vindas de conteúdo editorial de escritórios, **não de tabela oficial da OAB**): **5% a 10%** sobre o valor arrematado, ou **R$ 1.000 a R$ 5.000** fixos, às vezes com cláusula de êxito.

> **Orçar isso ANTES do lance.** É custo de aquisição tanto quanto o ITBI.

---

## 12. 🟡 CUSTAS JUDICIAIS — não pesquisadas

Custas da execução e da **expedição da carta de arrematação** **não foram pesquisadas** e variam por tribunal. **Não dar número.** Mandar consultar o regimento de custas do tribunal de origem.

---

## 13. ⭐ CHECKLIST DA CONTA COMPLETA — as 12 linhas

| # | Item | Ordem de grandeza | Status da fonte |
|---|---|---|---|
| 1 | **Lance** | — | edital |
| 2 | **Comissão do leiloeiro** | **5%** (7% em edital real; **sem teto legal**) do lance, **por fora** | ✅ §2 |
| 3 | **Encargos de administração da plataforma** | R$ 35 a R$ 65.000 por faixa, em uma das plataformas | ✅ §3 |
| 4 | **ITBI** | alíquota **municipal** × valor da arrematação | 🟡 alíquota — **nunca dar número** · §4 |
| 5 | **Emolumentos de registro** | pela **MAIOR base**; ~R$ 1,5 mil a R$ 4,4 mil nas faixas SP 2026 | 🟡 **só SP** · §5 |
| 6 | **Laudêmio** (se foreiro) | % sobre a transferência | ✅ checar na matrícula · §5 |
| 7 | **Débitos tributários anteriores** | **R$ 0** se o edital é posterior à virada da modulação | ✅ §6 |
| 8 | **Débitos condominiais anteriores** | **RISCO REAL** — chegou a **39% da avaliação** em edital real | 🚨 §6 |
| 9 | **Carrego** (condomínio + IPTU até a posse) | meses × (cota + IPTU) | ✅ §7 |
| 10 | **Desocupação** | honorários + tempo; 60 dias com liminar no extrajudicial | ✅ §8 |
| 11 | **Reforma / regularização** | orçamento pessimista, sem garantia de vício | ✅ §10 |
| 12 | **Honorários do pós-arrematação** | 5–10% **sobre o valor arrematado** ou R$ 1k–5k 🟡 | ✅ o leiloeiro não atua · §11 |
| — | *(a somar quando extrajudicial)* **Taxa de ocupação** | **1%/mês desde a CONSOLIDAÇÃO** — **crédito**, não custo | 🟡 legitimidade do terceiro · §9 |
| — | **Custas judiciais** | não pesquisadas | 🟡 §12 |

---

## 14. O QUE ESTA CONTA PROVA — e como se usa no parecer

1. **O deságio anunciado não é o deságio real.** Média provada de mercado: **37,3%** sobre a avaliação. Depois de comissão, ITBI, emolumentos pela maior base, carrego e desocupação, a margem efetiva é **substancialmente menor** — e em lote com dívida condominial informada pode ser **negativa**.
2. **A conta é a diferença entre um parecer e um palpite.** É o que o `parecer-go-nogo-lote` entrega e o que nenhuma resposta de "vale a pena?" sem documento consegue produzir.
3. **Três linhas dependem de documento que só a due diligence traz** — dívida condominial (edital + declaração da administradora), carrego (apuração da ocupação), regularização (matrícula + planta). **Sem elas, a conta não fecha, e o parecer sai NO-GO por insuficiência de prova.**

---

## 15. FRONTEIRAS DESTE ANEXO

| Precisa de | Vá para |
|---|---|
| As cláusulas de edital que geram cada linha de custo | `clausulas-armadilha-de-edital.md` |
| O julgado de cada trava (comissão sem teto, Tema 1.134, condomínio, ITBI) | `jurisprudencia-leiloes.md` |
| Texto integral do CPC 884, 886, 891, 895, 901, 903, 908 §1º | `cpc-leilao-879-903.md` |
| Texto integral da Lei 9.514 (arts. 24, 27, 30, 37-A) | `lei-9514-consolidada.md` |
| Texto do art. 9º da Lei 14.711 (ITBI e laudêmio antes do registro — §14) | `lei-14711-2023.md` |
| Deveres do leiloeiro e regime da comissão na norma | `leiloeiro-decreto-21981-in-drei-52.md` |
| Preço de mercado, deságio e concorrência | `mercado-leiloes-2026.md` |
| O gate que impede montar a conta sem documento lido | `metodologia-leiloes.md` |
