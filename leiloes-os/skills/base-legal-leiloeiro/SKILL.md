---
name: base-legal-leiloeiro
description: "Fundacao legal do leiloeiro oficial: Decreto 21.981/1932 (a lei especial) + IN DREI 52/2022 (a norma administrativo-disciplinar vigente, nunca a IN DNRC 113/2010), lidos com o mapa de norma viva x norma morta — porque muito artigo de 1932 esta materialmente superado e cita-lo em peca entrega o flanco. Cobre matricula e caucao moderna, exercicio pessoal e prepostos, deveres e proibicoes, prestacao de contas e repasse, credenciamento judicial, a escala de antiguidade que NAO vale no leilao judicial, e a comissao: os 5% do comprador sao PISO, nao existe teto, e o ataque do arrematante e temporal. Use para conferir a regularidade do leiloeiro antes do lance, em consultivo do lado do leiloeiro, em impugnacao de comissao ou de nomeacao, e quando disserem o leiloeiro pode isso, comissao de 7 por cento, matricula na Junta, a plataforma e credenciada, prestacao de contas do leiloeiro."
---

# BASE-LEGAL-LEILOEIRO

> Camada 1. Fundacao. **Duas normas, uma materia:** o Decreto e a lei especial; a IN DREI 52/2022 rege a relacao leiloeiro x Junta Comercial. **A IN nao e norma processual e nao governa o arbitramento judicial da comissao.**

## Anexos obrigatorios (context/)
- `context/leiloeiro-decreto-21981-in-drei-52.md` — o mapa **norma viva x norma morta** (§1), a comissao (§2) e o bloco 🟡 que nao entra em peca (§11) — **grep o artigo e leia a faixa**.
- `context/resolucao-cnj-236-2016.md` — arts. 1º, 2º, 7º e 9º: o credenciamento e a comissao no **judicial** — **grep + ler a faixa**.
- `context/jurisprudencia-leiloes.md` — §5 (RMS 65.084/SP, REsp 680.140/RS, REsp 2.198.525) — **grep + ler a faixa**.

## Objetivo
Entregar o dispositivo vigente sobre o leiloeiro — e, principalmente, **impedir a citacao de norma morta**. Alimenta `estrategia-de-lance-e-habilitacao` (due diligence do leiloeiro), as duas skills consultivas do leiloeiro e qualquer impugnacao de comissao ou de nomeacao.

## Metodologia
1. Separar o eixo: **habilitacao** (matricula, caucao) · **exercicio** (preposto, plataforma) · **deveres** · **comissao** · **contas e repasse** · **credenciamento judicial**.
2. Conferir no mapa do §1 se o dispositivo do Decreto ainda e **norma viva**; se a IN venceu, citar a IN.
3. Grep e **leitura da faixa** nos dois textos antes de afirmar.
4. Devolver dispositivo + o que vale hoje + o risco de citar o superado.
5. Fechar por `validador-leiloes` e `suprema-corte-leiloes`.

## ⭐ Norma viva x norma morta (o que mais derruba peca)

| Tema | Decreto 21.981/1932 | IN DREI 52/2022 | O que vale hoje |
|---|---|---|---|
| **Requisitos para ser leiloeiro** | art. 2º — 25 anos, 5 anos de domicilio | **art. 47 — SEM idade minima e SEM tempo de domicilio** | 🔴 **A IN venceu.** Nunca exigir 25 anos ou 5 anos de domicilio |
| **Caucao** | art. 6º — fianca de 40:000$000 (reis; **so no DF** — nos Estados, arbitrada pelas Juntas Comerciais, red. Dec. 22.427/1933) | **art. 50 — dinheiro, fianca bancaria ou seguro garantia** | 🔴 **A IN venceu.** Peca que invoque "40:000$0" cita **norma morta** — e o valor nunca foi nacional |
| **Comissao do comprador** | **art. 24, §unico — 5% obrigatorios** | art. 80, §2º — repete | Ambos vivos e concordantes. E **PISO** (bloco abaixo) |
| **Comissao do comitente** | art. 24, caput — 5% moveis / 3% imoveis | art. 80, §1º — idem | Vivos, mas **supletivos**: so na falta de convencao escrita |
| **Vedacao de sociedade** | art. 36 — destituicao | art. 75, I IN 52/2022 — **abrandada pela IN 88/2022** | Vive; hoje se admite *holding pura* |
| **Prazo de repasse** | arts. 27-28 Dec. 21.981 — **5 dias uteis + 5 dias** | art. 74, XIV e XV IN 52/2022 — **10 dias** | ⚠️ **Divergencia REAL, nao resolvida** — dizer que ha divergencia, nao escolher por conta |
| **Escala de antiguidade** | arts. 41-43 — so bens **publicos** | art. 71, §3º — judicial e particular = livre confianca | Concordantes: **NAO vale no judicial** |
| **IN DNRC 113/2010** | — | substituida na pratica pela IN 52/2022 | 🟡 **O ato revogatorio nao foi aberto** — o achado e **desatualizacao de fundamentacao**, nao nulidade provada |

## ⭐⭐ A comissao — 5% e PISO, nao teto, e nao existe teto
Quem le o **art. 75, II, "a", da IN 52/2022 isoladamente conclui o contrario e erra**. A leitura correta: e **vedacao a cobrar ABAIXO do minimo** — comissao **abaixo** de 5% e que e ilegal, e o leiloeiro tem direito a **complementacao**.
- **RMS 65.084/SP** (4ª Turma, unanime, j. 27/06/2023, transito 14/09/2023) reafirmando o precedente-matriz **REsp 680.140/RS** (5ª Turma, unanime), cuja ementa e expressa: *"nao ha limitacao quanto ao percentual maximo"* — **10% validado**.
- ⚠️ **Cite REsp 680.140/RS.** A ementa do RMS traz **"640.140" por erro de digitacao do proprio STJ** — **nao reproduzir**.
- **7% em leilao JUDICIAL e licito** (arbitramento do juiz — CPC 884, §unico + Res. CNJ 236, art. 7º).
- ⚠️ **Os tres residuos, obrigatorios em qualquer skill que toque comissao:** (a) **nao existe ato do DREI** declarando isso — o risco disciplinar formal do leiloeiro **nao esta zerado**; (b) **no EXTRAJUDICIAL o raciocinio NAO se transporta** — la nao ha juiz arbitrando, **nenhum julgado localizado**, e e a hipotese mais exposta ao art. 75; (c) sao **acordaos de turma, nao repetitivos**.
- ⭐ **O eixo de ataque do arrematante e TEMPORAL, nao substantivo:** impugnar o percentual **ANTES do lance**. Publicado o edital, houve ciencia dos termos; nao impugnado e pago, **consolida-se**.
- **REsp 2.198.525** (3ª Turma, julho/2026 — **turma, nao repetitivo**): remicao posterior ao lance e anterior ao auto **nao** afasta a comissao; o leiloeiro tem legitimidade recursal como terceiro prejudicado (CPC 996).

## Credenciamento, exercicio e responsabilidade
- **Credencia-se o LEILOEIRO pessoa fisica, nao a plataforma** (IN art. 60 · Res. CNJ 236, arts. 1º e 2º). A plataforma e **atividade-meio**, e o art. 60 **nao afasta a responsabilidade pessoal** do leiloeiro. Due diligence se faz por **nome + matricula**, cruzando a lista do tribunal com a da Junta — o **art. 89, VII** obriga a Junta a publicar a **situacao** (regular / licenciado / suspenso). Procurar "a empresa" na Junta **nao devolve nada**.
- **Funcao pessoal e indelegavel**; prepostos nos arts. 11-13 do Decreto — **leilao com desrespeito a regra de substituicao do preposto e NULO**.
- **Proibicoes** (Dec. art. 36 x IN 52/2022 art. 75): **autocompra e punida com multa, nao com destituicao**; nulidade do pregao em domingo ou feriado e da delegacao.
- **Responsabilidade:** fiel depositario; responde pela perda de fundos **ainda em caso fortuito** (art. 40). Dever de **informar antes do pregao** (IN art. 74, IX: anuncio 3 vezes **enunciando gravames e onus**; XXIII: nome e matricula no edital) — e o contrapeso do "sem garantia" do art. 18 da Res. CNJ 236.
- **Leilao pela internet** entrou no Decreto pelo art. 19 (Lei 13.138/2015) — competencia privativa do leiloeiro.

## Regras de ouro
- **Impugnar nomeacao por "quebra de antiguidade" em execucao civel e tese perdida** — a escala so vale nas vendas de bens da Uniao, Estados e Municipios.
- **Divergencia de repasse (5+5 x 10 dias) e real:** expor as duas fontes, nunca apresentar um dos prazos como pacifico.
- 🟡 **O bloco §11 do anexo nao entra em peca** — dispositivos de 1932 cuja compatibilidade com o direito vigente **nao foi verificada**, entre eles a **prisao do leiloeiro como depositario remisso** (Dec. 21.981 art. 27, §4º) x **SV 25/STF**.
- Cross-link soft: a comissao **no processo** (901 §1º, 884 §unico) esta em `base-legal-leilao-judicial`; a conta do arrematante, em `custo-total-real-e-precificacao`.

## Entrega obrigatoria final
Dispositivo + qual das duas normas prevalece + faixa lida + o risco de citar o superado + skill de destino.

## Guard
Norma morta **nao entra em peca** (idade minima, domicilio, fianca em reis, IN DNRC 113/2010 como vigente). Comissao acima de 5% **no extrajudicial** nunca sai como licita sem o residuo (b). Nunca escrever "640.140". Fecha por `validador-leiloes` e `suprema-corte-leiloes`.
