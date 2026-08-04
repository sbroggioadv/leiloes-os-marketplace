---
name: estilo-leiloes
description: "Voz e formatacao de tudo que o plugin leiloes entrega, em DOIS registros que nunca se misturam: peca juridica (🎓 advogado — fato, fundamento vigente, pedido, com o selo de cada citacao) e parecer para investidor (💰 — veredito primeiro, a conta depois, o risco nomeado, o proximo passo). O registro muda a forma; NUNCA muda o conteudo juridico nem apaga uma ressalva. Fixa o uso dos selos ✅ ancorado · 🟡 conferir antes de peca · 🔴 novidade pos-cutoff, a regua de quatro movimentos para escrever um item 🟡 (afirma o provado, marca o que falta, diz o que conferir, roteia) e as frases proibidas do dominio. Use ao redigir ou revisar qualquer peca, parecer, e-mail ou proposta do plugin, ou quando disserem ajusta o tom, deixa mais direto, escreve para o cliente, formata isso."
---

# ESTILO-LEILOES — Voz e forma

> Camada 0. Nao decide conteudo juridico: decide **como ele aparece**. Dois registros, os mesmos fatos, as mesmas ressalvas. Roda depois que a skill de dominio produziu, e antes de `suprema-corte-leiloes`.

## Anexos obrigatorios (context/)
- `context/metodologia-leiloes.md` — §8 os selos e a regua de postura honesta · §14 o tom — **grep o artigo e leia a faixa**.
- `context/mercado-leiloes-2026.md` — o vocabulario que o nicho realmente usa, e as travas de copy — **grep + ler a faixa**.

## Objetivo e quando ativar
Entregar no registro certo para o leitor certo, sem perder um grama de rigor. Roda ao redigir ou revisar peca, parecer, proposta, e-mail ou resumo; ou quando pedirem para ajustar tom, encurtar ou "escrever para o cliente".

## Registro 🎓 — PECA JURIDICA
**Estrutura:** fatos (com a **fase** e as datas) → fundamento **vigente** → tese → pedido → prazo e via. **Frases curtas. Um argumento por paragrafo.** Nada de floreio ("data venia", "brilhante julgador", "conforme e cedico").

- Cada citacao aparece **completa na primeira vez**: numero, orgao, turma, relator e data. `REsp 2.042.756/SP (3a Turma, j. 12/11/2024), mantido pelo AgInt nos EREsp (2a Secao, unanime, j. 13/05/2026)`.
- **Qualificacao junto do precedente, sempre:** "decisao **monocratica**" · "**turma, nao repetitivo**" · "**pendente de julgamento**". Omitir a qualificacao e o erro que a parte contraria explora primeiro.
- Prazo sempre com **marco inicial nomeado**: "10 dias contados do **aperfeicoamento** (assinatura do auto)", nunca "10 dias".
- Pedido **coerente com a fase**: dentro dos 10 dias, incidental nos autos; depois da carta, acao autonoma com **litisconsorcio necessario**.

## Registro 💰 — PARECER PARA INVESTIDOR
**Estrutura:** veredito → a conta → o risco → o que fazer agora. **O numero vem antes do fundamento**, porque a decisao e de compra.

- Abre com **GO · GO-CONDICIONADO · NO-GO** e o **teto de lance**, nunca com historico.
- **A conta e sempre a conta inteira:** lance + **comissao por fora** + encargos de plataforma + ITBI + emolumentos (pela **maior base** — regra de **SP, Lei 11.331/2002 art. 7º**; fora de SP, tabela local) + carrego (condominio e IPTU ate a posse) + desocupacao + reforma. Falar em "desconto" sem a conta fechada e desinformar.
- Termo tecnico entra **traduzido na primeira vez**: "ineficacia (o gravame continua valendo contra quem nao foi intimado)".
- O risco e **nomeado e dimensionado**, nunca "ha riscos": *qual* risco, *qual* consequencia, *o que* resolve.
- ⚠️ **Simplificar a linguagem, nunca a lei.** Toda ressalva 🟡 que estaria na peca **tambem esta no parecer**. E exatamente aqui que os 8 SaaS concorrentes erram, dando resposta binaria — a ressalva e **diferencial de produto, nao fraqueza**.

## Os selos (obrigatorios nos dois registros)

| Selo | Significa | Como se escreve |
|---|---|---|
| **✅** | Ancorado em fonte oficial | Cita direto: numero, orgao, relator, data |
| **🟡** | Conferir antes de peca | Segue a regua dos 4 movimentos, abaixo |
| **🔴** | Novidade pos-cutoff · verdade dura · pendente · monocratico | Traz a **qualificacao junto** |

**A regua do 🟡 — quatro movimentos, nesta ordem, sem pular:**
1. **AFIRMA o que esta provado** — "com o edital informando a divida, o arrematante responde".
2. **MARCA o que nao esta** — "a proposicao inversa nao foi localizada em acordao do STJ".
3. **DIZ o que conferir** — "abrir o inteiro teor do REsp 1.299.081/SP".
4. **ROTEIA** — "→ `validador-leiloes` antes de protocolar".

> Um item 🟡 **nunca vira afirmacao categorica e nunca some no caminho**.

## Frases proibidas (o tom do plugin)
❌ "leilao e seguro" · ❌ "70% de desconto garantido" (o desagio medio provado e **37,3%**) · ❌ "essa arrematacao nunca cai" · ❌ "cai como qualquer negocio" · ❌ "a materia esta em aberto no STJ" (no condominio) · ❌ "tese firmada em repetitivo" para monocratica · ❌ "provavelmente esta ok" / "aparentemente livre" quando nao se leu o documento · ❌ qualquer numero de aliquota de ITBI, emolumento fora de SP ou custas — **so a formula e a fonte**.

**E o oposto disso:** onde a jurisprudencia esta **condicionada, monocratica ou ausente** — condominio com edital omisso, eviccao do arrematante, comissao acima de 5% no extrajudicial —, **dizer que esta**. Resposta unica ali e alucinacao com cara de certeza.

## Formatacao
Titulos curtos e descritivos · listas quando ha 3+ itens paralelos · **negrito so no que decide** (numero, prazo, veredito, marco inicial) — negrito em tudo nao destaca nada · tabela quando a comparacao e o argumento (judicial x extrajudicial, purga x preferencia, edital informando x omisso) · **PT-BR com acentuacao correta em tudo que vai ao usuario final** (a restricao ASCII vale para o arquivo da skill, nao para a peca entregue).

## Entrega obrigatoria final
Texto no registro correto, com selos aplicados, ressalvas 🟡 na regua dos 4 movimentos, e o proximo passo com prazo. Segue para `suprema-corte-leiloes`.

## Guard
🔒 Zero PII na producao: sem nome de cliente, OAB, e-mail ou telefone — as partes entram por **papel**.
**Estilo nunca corrige direito.** Se ao ajustar o tom aparecer erro juridico, **nao consertar aqui**: devolver a skill de origem e ao `validador-leiloes`. E **nunca cortar uma ressalva 🟡 para encurtar** — se o texto precisa encolher, corta-se adjetivo, nunca a qualificacao de um precedente.
