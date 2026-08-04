---
name: excussao-multipla-e-concurso-de-credores
description: "Dois imoveis ou dois credores na mesma garantia — as duas engrenagens que a Lei 14.711/2023 criou e que quase ninguem opera. Entrega o art. 27-A da Lei 9.514/97 (excussao SIMULTANEA ou SUCESSIVA de varios imoveis, a ordem escolhida pelo credor SALVO clausula contratual em contrario, o demonstrativo averbado nas matriculas nao leiloadas e o prazo de 30 dias, nao 60) e o art. 10 da Lei 14.711/2023 (concurso de credores CARTORIAL, sem juiz: intimacao simultanea pelo oficial do registro, habilitacao em 15 dias, quadro de credores por antiguidade do credito real — e a distribuicao do dinheiro a cargo do CREDOR EXEQUENTE, que e o ponto sensivel). Use quando houver mais de um imovel em garantia, mais de um credor na matricula, ou quando disserem o banco leiloou meu outro imovel, sou credor de segundo grau, nao recebi minha parte."
---

# EXCUSSAO-MULTIPLA-E-CONCURSO-DE-CREDORES

> Camada 4. **Onde a garantia deixa de ser um imovel e vira uma fila.** Duas regras novas de 2023, sem jurisprudencia formada, e com alavancas contratuais que se perdem por desatencao na redacao.

## Anexos obrigatorios (context/)
- `context/lei-9514-consolidada.md` — §6 do anexo (art. 27-A verbatim, **4 paragrafos**) e §5 (art. 27 da Lei 9.514, o rito para o qual o §3º remete) — **grep + ler a faixa**.
- `context/lei-14711-2023.md` — §2 do anexo (art. 10 verbatim, com os **3 incisos** de requerimento e os **2 paragrafos**) e §1 (art. 9º, o rito hipotecario que tambem alimenta o concurso) — **grep + ler a faixa**.
- `context/jurisprudencia-leiloes.md` — §10, o **vacuo declarado**: nao ha jurisprudencia do STJ sobre o art. 27-A da Lei 9.514 nem sobre o concurso cartorial — **grep + ler a faixa**.
- `context/metodologia-leiloes.md` — §10, os prazos e marcos — **grep + ler a faixa**.

## Objetivo
Devolver **a ordem em que os bens vao cair**, **quem recebe primeiro e quanto**, e **onde ha alavanca** — de contrato para quem redige, de habilitacao para quem ja e credor, de due diligence para quem vai arrematar um imovel que faz parte de um pacote.

## Metodologia
1. **Contar as garantias:** quantos imoveis respondem pela mesma divida, e se ha **vinculacao de cada imovel a uma parcela** — havendo, o art. 27-A da Lei 9.514 nao se aplica.
2. **Ler o contrato** procurando **disposicao expressa sobre a ordem de excussao** (§1º) — e a alavanca principal.
3. **Ler as matriculas de TODAS as garantias**, nao so a do lote de interesse: o §2º manda averbar o **demonstrativo do resultado** de cada leilao nas matriculas dos imoveis **nao leiloados**. Essa averbacao e prova.
4. **Mapear os credores concorrentes** e a **antiguidade** de cada credito real — e ela que ordena o quadro.
5. **Cravar os prazos:** habilitacao em 15 dias; leilao do imovel seguinte em 30 dias.
6. Fechar por `suprema-corte-leiloes` + `validador-leiloes`.

## 1. Varios imoveis — art. 27-A da Lei 9.514

**Pressuposto do caput:** credito garantido por **alienacao fiduciaria de dois ou mais imoveis**, **sem** vinculacao de cada imovel a uma parcela da divida.

| Modo | Como funciona |
|---|---|
| **Simultaneo** | Consolidacao e leilao de **todos os imoveis em conjunto**, num ato so |
| **Sucessivo** | Consolidacao e leilao de **cada imovel em sequencia**, **a medida do necessario** para satisfazer o credito |

| § | O que decide | Onde morde |
|---|---|---|
| §1º ⭐ | Na via sucessiva, **o credor indica os imoveis a excutir em sequencia — EXCETO se houver disposicao em sentido contrario expressa no contrato**, hipotese em que a **consolidacao dos demais fica SUSPENSA** | **Alavanca real de quem redige do lado do devedor**: clausula barata de negociar, cara de esquecer |
| §2º | A cada leilao, o credor **averba o demonstrativo do resultado nas matriculas dos imoveis nao leiloados** e o encaminha ao devedor e aos terceiros fiduciantes, nos enderecos **fisico e eletronico** do contrato | Demonstrativo ausente ou nao averbado e **achado documental** |
| §3º ⚠️ | Nao alcancada a quantia suficiente, o credor recolhe **ITBI** e, se for o caso, **laudemio** do imovel seguinte, requer a averbacao da consolidacao e, **em 30 dias**, realiza o leilao nos termos do art. 27 da Lei 9.514 | 🔴 **30 dias, nao 60** — divergencia interna da lei, respeitada como esta |
| §4º | Satisfeito o credito, o credor entrega **termo de quitacao** e **autorizacao de cancelamento** do registro da propriedade fiduciaria dos imoveis que restarem | Garantia que sobra tem de ser **liberada** |

⭐ **Para o arrematante:** o lote pode ser **peca de um pacote**. Pergunte se ha outros imoveis na mesma garantia e leia o **demonstrativo averbado** — ele diz quanto ja foi apurado e se o credito ainda esta descoberto. Pacote em curso muda o apetite do credor no proximo leilao.

## 2. Concurso de credores CARTORIAL — art. 10 da Lei 14.711/2023

**Pressuposto:** **mais de um credito garantido pelo mesmo imovel**, havendo averbacao de inicio da excussao hipotecaria ou de consolidacao da propriedade fiduciaria.

| Etapa | O que a lei manda |
|---|---|
| Intimacao | O **oficial do registro de imoveis** intima **simultaneamente todos os credores concorrentes** para habilitarem seus creditos |
| Prazo | **15 dias**, contados da data da intimacao |
| Requerimento (**3 incisos**) | **I** calculo do valor **atualizado** do credito para excussao, com os acessorios · **II** documentos de **desembolso e saldo devedor**, quando o credito for futuro, condicionado ou rotativo · **III** **sentenca judicial ou arbitral** que torne liquido e certo o montante, quando iliquida a obrigacao |
| §1º | Findo o prazo, o oficial lavra **certidao** e intima o garantidor e todos os credores do **quadro atualizado**, com os creditos e os **graus de prioridade**, observada a **antiguidade do credito real** |
| §2º 🔴 | **A DISTRIBUICAO dos recursos fica a cargo do CREDOR EXEQUENTE**, que deve observar o quadro e os prazos legais de entrega do remanescente ao devedor |

🔴 **O ponto sensivel e o §2º.** Criou-se um concurso **sem juiz**, e o pagamento dos concorrentes fica **nas maos de uma parte interessada**. Consequencias praticas:

- **Credor de grau inferior:** habilitar **dentro dos 15 dias** e a unica forma de entrar no quadro; e o credito precisa chegar **liquido** (inciso III). Perdido o prazo, a discussao migra para reparacao.
- **Quem foi preterido:** o **quadro lavrado pelo oficial** e a prova documental do que era devido; o descumprimento pelo credor exequente e argumento concreto → `reparacao-por-leilao-irregular`.
- **Arrematante:** o concurso **nao e problema seu** — o preco vai para a fila —, mas conferir as **averbacoes de excussao** de outros credores na matricula evita surpresa de disputa sobre o produto → `leitura-de-matricula`.

## Regras de ouro
- **Contar antes de opinar:** quantos imoveis, quantos credores, quantas averbacoes. Numero que nao foi contado no documento nao entra no parecer.
- **A antiguidade que ordena e a do CREDITO REAL**, nao a da divida nem a do vencimento.
- ⚠️ **Nao transportar prazo:** os **30 dias** do §3º do art. 27-A da Lei 9.514 valem para o **imovel seguinte na excussao sucessiva**; os **60 dias** do art. 27 da Lei 9.514 valem para o 1º leilao a partir da consolidacao.
- 🔴 **Vacuo declarado:** **nao foi localizada** jurisprudencia do STJ sobre o art. 27-A da Lei 9.514 nem sobre o concurso cartorial. Sustentar pelo **texto**, e dizer que a aplicacao ainda nao tem precedente. Tratar como **"nao localizado"**, nunca "inexistente".
- 🟡 **Regulamentacao registral nao verificada** — a operacionalizacao do quadro de credores, da certidao e das intimacoes simultaneas depende de norma de corregedoria **estadual** nao conferida. Marcar *"conferir a norma do Estado antes de protocolar"* e rotear ao `validador-leiloes`.
- Cross-link soft: o rito de cada leilao esta em `os-dois-leiloes-da-alienacao-fiduciaria` e em `hipoteca-extrajudicial-14711`; a leitura das matriculas, em `leitura-de-matricula`; a responsabilizacao, em `reparacao-por-leilao-irregular`.

## Entrega obrigatoria final
(a) **Mapa das garantias** — imoveis, matriculas, averbacoes, demonstrativos; (b) **modo de excussao** e a **ordem**, dizendo se ha clausula contratual que a inverte e suspende a consolidacao dos demais; (c) **quadro de credores** com antiguidade e prazo de habilitacao com data; (d) **cronograma** com os 30 dias de cada imovel seguinte; (e) itens 🟡 nomeados. Validado por `suprema-corte-leiloes` + `validador-leiloes`.

## Guard
Nunca afirmar a ordem de excussao **sem ler o contrato** — o §1º do art. 27-A da Lei 9.514 e ressalvado por clausula. Nunca aplicar o art. 27-A da Lei 9.514 quando **cada imovel esta vinculado a uma parcela**. Nunca escrever **60 dias** onde o §3º diz **30**. Nunca dizer que o oficial distribui o dinheiro — **e o credor exequente** (art. 10, §2º, da Lei 14.711/2023). Nunca alegar jurisprudencia sobre estes dispositivos — **nao foi localizada**. Sempre nomear o diploma junto do numero do artigo. Fecha por `suprema-corte-leiloes` + `validador-leiloes`.
