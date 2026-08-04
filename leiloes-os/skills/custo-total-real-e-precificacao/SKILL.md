---
name: custo-total-real-e-precificacao
description: "Monta a conta INTEIRA do arrematante e devolve o TETO DE LANCE, nao o desconto: lance mais comissao por fora, encargos de plataforma, ITBI, emolumentos pela MAIOR base, laudemio, debitos condominiais informados no edital, carrego ate a posse, desocupacao, reforma e honorarios do pos, menos a taxa de ocupacao recuperavel no extrajudicial. Um lance de R$ 1.000.000 custa R$ 1.050.000 so de lance mais comissao a 5 por cento. Nunca da numero de aliquota de ITBI, de emolumento fora de Sao Paulo nem de custas judiciais — variam por ente, e a skill entrega a formula e a fonte a consultar. Use para precificar qualquer lote antes do lance e quando disserem quanto vou gastar de verdade, qual meu lance maximo, vale a pena com esse desagio, quanto de ITBI e cartorio, o desconto e real."
---

# CUSTO-TOTAL-REAL-E-PRECIFICACAO

> Camada 2. Publico 💰 primeiro. **O lance e a MENOR parte da conta.** Esta skill nao calcula desconto — ela calcula **o teto acima do qual o negocio deixa de existir**.

## Anexos obrigatorios (context/)
- `context/custo-total-do-arrematante.md` — ⭐ **o anexo-eixo**: a formula do teto (§1), comissao (§2), plataforma (§3), ITBI (§4), **emolumentos pela maior base (§5)**, debitos (§6), carrego (§7), desocupacao (§8), taxa de ocupacao (§9), reforma (§10), honorarios (§11), custas (§12) e o **checklist das 12 linhas** (§13) — **grep a linha de custo e leia a faixa**.
- `context/cpc-leilao-879-903.md` — **901 §§1º e 2º** (a sequencia de pagamento e o ITBI antes da carta) e **884 §unico** — **grep + ler a faixa**.
- `context/clausulas-armadilha-de-edital.md` — ARM-07 a ARM-12 (as clausulas que geram cada linha) — **grep + ler a faixa**.
- `context/jurisprudencia-leiloes.md` — Tema 1.134 e a modulacao · condominio · comissao · REsp 1.188.655/RS — **grep + ler a faixa**.
- `context/mercado-leiloes-2026.md` — desagio medio e vocabulario do nicho — **grep + ler a faixa**.

## Objetivo
Fechar a conta linha a linha e devolver o **TETO DE LANCE** com a comissao ja embutida — mais o que **falta de documento** para a conta fechar.

## ⭐ A formula

```
        VALOR DE MERCADO LIQUIDO ESPERADO
      - comissao do leiloeiro (% DO EDITAL, por fora)
      - ITBI (aliquota municipal x base da arrematacao)
      - emolumentos de registro (pela MAIOR base)
      - laudemio, se o imovel for foreiro
      - encargos de administracao da plataforma
      - debitos condominiais que o edital informa
      - carrego: meses ate a posse x (cota + IPTU)
      - desocupacao: honorarios + tempo
      - reforma / regularizacao (cenario pessimista)
      - honorarios do pos-arrematacao
      + taxa de ocupacao recuperavel, se extrajudicial (CREDITO)
      ---------------------------------------------------
      = TETO DE LANCE
```

> ⚠️ **A regra operacional que evita o erro mais caro:** a comissao e somada **por fora**. **Lance o teto MENOS a comissao**, nunca o teto cheio — quem lanca o teto cheio ja estourou o orcamento no martelo.

## Metodologia
1. **Ler o percentual da comissao no edital em maos.** Nao assumir 5%.
2. **Puxar as tres linhas que so a due diligence traz** — debito condominial (edital + declaracao da administradora), carrego (apuracao da ocupacao), regularizacao (matricula + planta). **Sem elas a conta nao fecha.**
3. **Aplicar as travas** dos blocos abaixo (comissao, emolumento, ITBI, debitos).
4. **Marcar cada linha** como ✅ ancorada, 🟡 a consultar (formula + fonte) ou ❌ **sem documento**.
5. Devolver o **teto** e o **piso de seguranca**; havendo ❌, o resultado nao e um numero — e **NO-GO por insuficiencia de prova**.
6. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## 🚨 Comissao — 5% e PISO, nao teto, e nao existe teto
O **CPC 884, §unico nao fixa percentual**; o piso vem do **Dec. 21.981/32, art. 24, §unico** e da **Res. CNJ 236, art. 7º** ("no minimo 5%").
- **RMS 65.084/SP** (4a Turma, unanime, j. 27/06/2023) reafirmando **REsp 680.140/RS**: *"nao ha limitacao quanto ao percentual maximo"* — **10% validado**, e **7% em leilao JUDICIAL e licito**. Comissao **abaixo** de 5% e que e ilegal. ⚠️ **Cite 680.140/RS** — a ementa do RMS traz "640.140" por **erro de digitacao do proprio STJ**. **Turma, nao repetitivo.**
- ⭐ **O ataque e TEMPORAL:** impugnar **ANTES do lance**; nao impugnado e pago, **consolida-se**. 🟡 **No EXTRAJUDICIAL nao se transporta** (nao ha juiz arbitrando; **nenhum julgado localizado**) — marcar e rotear ao `validador-leiloes`.
- **Para a conta:** entre 5% e 7% em imovel de R$ 500 mil vao **R$ 10.000**. **Um lance de R$ 1.000.000 custa R$ 1.050.000** a 5%, antes de tudo o mais.
- **Nao devida** em leilao negativo, anulacao ou desistencia do exequente (art. 7º, §§1º-2º); **devida** em acordo ou remicao **posteriores a alienacao** (§3º) — e **REsp 2.198.525** (**turma**): remicao apos o lance e antes do auto **nao** afasta a comissao.

## 🚨 Emolumentos — pela MAIOR base, e o numero e regional
Em **Sao Paulo**, o **art. 7º da Lei estadual 11.331/2002** manda usar o **MAIOR** entre: (1) **preco declarado** (o lance), (2) **valor tributario do IPTU**, (3) **base de calculo do ITBI**.

> 🚨 **Arrematar com 50% de desconto NAO corta o emolumento pela metade.** Se o IPTU ou a base do ITBI forem maiores que o lance, e por eles que a faixa e enquadrada. E uma das linhas que mais destroi margem em lote de desagio alto.

🟡 **Tres limites honestos, obrigatorios ao usar esta linha:** (a) **a regra e ESTADUAL e so Sao Paulo foi verificado** — para qualquer outro estado, **dar a formula e mandar consultar a tabela da corregedoria ou da associacao de registradores local**, **nunca extrapolar os valores de SP**; (b) **nao existe item de tabela nominado "carta de arrematacao"** — usa-se o item generico de registro com valor declarado; (c) parte das faixas veio com **OCR corrompido** na captura e **nao se reproduz** — conferir no PDF original. Em duvida: **formula e fonte, nunca numero** → `validador-leiloes`.

## ITBI — base, aliquota e a armadilha de sequencia
- **Base:** o valor **alcancado na hasta**, nao o venal — **REsp 1.188.655/RS** (**turma, nao repetitivo**). ⚠️ **Nao existe tese repetitiva** sobre ITBI em arrematacao, e o **Tema 1.113 NAO e sobre arrematacao** (e ITBI em geral, sem transito).
- 🟡 **Aliquota: varia por municipio e NAO foi pesquisada. NUNCA dar o numero** — dar a formula (**aliquota municipal x base da arrematacao**) e mandar consultar a legislacao do municipio do imovel.
- 🚨 **A sequencia e invertida:** `preco → comissao → despesas → ITBI → CARTA → mandado de imissao`. O **CPC 901, §2º** exige a **prova de pagamento do ITBI na carta** e o **§1º** condiciona carta e mandado ao deposito de preco, comissao e despesas. **O arrematante desembolsa tudo antes de ter titulo e antes de ter posse** — quem planejou pagar o ITBI "depois, com o aluguel" **trava a propria carta**. No extrajudicial, a **14.711, art. 9º, §14** poe ITBI e laudemio **antes do registro**.

## As linhas que ninguem soma
- **Plataforma:** uma das cinco verificadas cobra administracao em **tabela por faixa, de R$ 35 a R$ 65.000**, *"nao inclusos no valor do lance"* e **somados** a comissao — e **veda PIX**. Em veiculos ha deposito e estadia.
- **Debitos:** tributario anterior = **R$ 0** (Tema 1.134 + CTN 130, §unico) 🟡 **desde que** o edital seja posterior a virada da modulacao — e **a data da ata nao e declarada na fonte** (a praxe usa 24/10/2024: **convencao, nao texto**), entao marcar e rotear. **Condominial informado no edital = custo CERTO**; **edital omisso = risco quantificado**, nunca R$ 0 → `debitos-propter-rem`.
- **Carrego:** `meses ate a posse x (cota + IPTU)` — **a linha mais esquecida**. O relogio vira **na arrematacao**, nao na posse (ARM-07); com ocupante resistente pode passar de 12 meses. O numero vem de `situacao-possessoria`, **nunca de chute**.
- **Desocupacao:** honorarios sempre. 🟡 Estatistica de cumprimento real **nao foi pesquisada** — liminar concedida nao e imovel vazio.
- **Taxa de ocupacao (extrajudicial):** **1%/mes sobre o valor do art. 24, VI desde a CONSOLIDACAO** ate a imissao (**37-A**) — e **CREDITO**, nao custo. 🟡 A **legitimidade do arrematante terceiro** para cobra-la **nao foi pesquisada**: lancar como **credito eventual**, jamais como receita que financia o lance.
- **Reforma e regularizacao:** com "sem garantia" e renuncia a vicio oculto, o custo e **integralmente** do arrematante — orcar no **cenario pessimista**. A regularizacao (projeto + INSS + averbacao) e o que **destrava financiamento e revenda**.
- **Honorarios do pos:** carta, ITBI, registro, baixa de gravames, imissao, defesa em cobranca — **o leiloeiro nao atua nessa esfera**. 🟡 As faixas de **5% a 10%** ou **R$ 1.000 a R$ 5.000** vem de conteudo editorial de escritorios, **nao de tabela oficial da OAB**. **Orcar ANTES do lance: e custo de aquisicao.**
- 🟡 **Custas judiciais e da carta: NAO pesquisadas**, variam por tribunal — **nao dar numero**; consultar o regimento de custas do tribunal de origem.

## Regras de ouro
- ⛔ **NUNCA dar numero de aliquota de ITBI, emolumento fora de SP ou custas.** Formula + fonte, sempre.
- **O desagio anunciado nao e o real.** A media provada e **37,3%** — e depois de comissao, ITBI, emolumento pela maior base, carrego e desocupacao a margem encolhe, e em lote com divida condominial informada pode ficar **negativa**.
- ⛔ **Nao estimar debito, ocupacao ou area "por alto" para completar a planilha.** Linha sem documento e ❌, e ❌ puxa o parecer para **NO-GO**.
- **Nunca prometer 70% de desconto** nem dizer que "leilao e seguro".
- Cross-link soft: calculo de atualizacao e saldo → `calculosjudiciais-adv-os`; ITBI como tributo e ganho de capital → `tributario-societario` / `cfo-combativo-os`; registro da carta → `registro-regularizacao-e-itbi`.

## Entrega obrigatoria final
Planilha das **12 linhas** com valor, fonte e selo (✅ / 🟡 formula-e-fonte / ❌ sem documento), o **TETO DE LANCE** e o **valor a lancar (teto menos comissao)**, o **desagio efetivo** contra o anunciado, e a lista do que falta. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Conta com linha ❌ **nao vira teto** — vira **NO-GO por insuficiencia de prova**. Nunca comissao dentro do lance. Nunca emolumento pelo lance quando o IPTU ou a base do ITBI forem maiores. Nunca numero de aliquota, emolumento fora de SP ou custas. Nunca condominio informado lancado como R$ 0. Nunca taxa de ocupacao como receita certa. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
