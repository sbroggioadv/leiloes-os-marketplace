# leiloes-os — regras internas do plugin

> Especialista em leilões judiciais e extrajudiciais brasileiros ponta a ponta, para os **DOIS lados** do mesmo evento (arrematante e executado/fiduciante) e para os **DOIS públicos** (advogado e investidor). **55 skills** em 8 camadas (C0-C7) sobre o CPC arts. 879-903, a Res. CNJ 236/2016, a Lei 9.514/97 e a Lei 14.711/2023. Despersonalizado (autoria IA Combativa; perfil do operador via `/start-leiloes`). **O núcleo comercial é a C2 — due diligence do arrematante.**

## Invioláveis (anti-alucinação por design)
- **Nenhuma citação** de dispositivo, súmula, tema, resolução ou prazo entra em peça sem âncora no `context/`. Guard permanente: `anti-alucinacao-leiloes`; validação final: `suprema-corte-leiloes` (R1-R4) + `validador-leiloes`.
- **Grep o artigo e leia a faixa.** O anexo é a prova do que ele captura **verbatim**; o resto é resumo, e resumo envelhece. Nunca despejar o anexo inteiro, nunca citar de memória.
- **Lei VIGENTE 2026 manda.** Na dúvida de vigência, bloquear e checar ao vivo.
- **É vedado afirmar situação do imóvel — ocupação, ônus, área, débito, regularidade — sem documento lido.**

## VERDADES DURAS — nunca contrariar

1. **DUE-DILIGENCE-FIRST é gate bloqueante, não pedagogia.** Pedido de lance, arrematação ou "vale a pena esse lote" exige as **4 provas**: edital (`analise-de-edital`) · matrícula (`leitura-de-matricula`) · ocupação (`situacao-possessoria`) · débitos (`debitos-propter-rem`) + cruzamento de risco (`risco-de-anulacao-do-certame`) + conta (`custo-total-real-e-precificacao`). **Faltando prova → NO-GO por insuficiência.** Nunca "provavelmente ok", nunca "aparentemente livre".

2. **A FASE é irreversível e decide a via.** Antes do lance · pós-lance com menos de 10 dias do auto · pós-carta · pós-imissão. O **CPC art. 903** conta o prazo de 10 dias do **aperfeiçoamento** (assinatura do auto), **não** da ciência do vício. Depois da carta, só **ação autônoma** (§4º), com o arrematante como **litisconsorte necessário**.

3. **DL 70/66, arts. 29 a 41 = REVOGADOS** (Lei 14.711/2023, art. 18, I — Capítulo III), desde **31/10/2023**. **Não dizer "o DL 70/66 foi revogado"** — os Capítulos I e II sobrevivem. O **Tema 1.288/STJ** tem **dois ramos**: **(a) antes da Lei 13.465/2017** — propriedade **já consolidada e mora já purgada** (art. 34 do DL 70/66, ato jurídico perfeito) → **desfazimento da consolidação** e retomada do contrato; **(b) a partir da Lei 13.465/2017** — propriedade consolidada **sem purgação** → **tão somente** preferência do **art. 27, §2º-B** da Lei 9.514. Não generalizar "qualquer fato anterior a 2017". O rito hipotecário novo é o **art. 9º da Lei 14.711**; o **filtro do §15** exige cláusula expressa no título — **sem a cláusula, o rito novo não se aplica** (ler o instrumento; não presumir por data).

4. **Preço vil é régua em CASCATA** (CPC 891, §único): com preço mínimo no edital, vil é o que fica **abaixo dele**; só na **ausência** vale o piso supletivo de **50% da avaliação**. **Três erros a bloquear:** (a) "o CPC fixa 50%"; (b) o piso valeria só para a 1ª praça; (c) transportar os 50% para o extrajudicial. No 2º leilão extrajudicial, 50% é **faculdade do credor** (9.514, art. 27, §2º · 14.711, art. 9º, §6º), **não** piso de vileza.

5. **Os "20%" não se misturam — base de cálculo colada ao número.**
   - **CPC art. 896, §2º** — multa de **20% da avaliação**, em benefício do **incapaz** (endereço correto desta multa).
   - **CPC art. 903, §6º** — até **20% do valor atualizado** do bem, por **ato atentatório** à dignidade da justiça (suscitação de vício infundado). **É outra coisa.**
   - Cláusula de edital pode ainda prever 20% do **lance** (perda) ou 20% de **caução** (depósito). Avaliar e lance **não** são a mesma base.

6. **Ineficácia ≠ nulidade.** Falta de intimação do **credor pignoratício, hipotecário ou anticrético** gera **ineficácia** (CPC arts. 804 e 903, §1º, II), não nulidade — a lei enumera esses credores, **não** "qualquer titular de direito real". Para o arrematante isso é **pior**: fica com o imóvel **e com o gravame**.

7. **Comissão e despesas NÃO estão dentro do lance** — são pagamento adicional e **condição para a carta** (CPC 901, §1º). O CPC **não fixa percentual** (884, §único). **5% é PISO**, não teto (RMS 65.084/SP + REsp 680.140/RS); no extrajudicial o raciocínio **não se transporta** sem julgado local.

8. **Condomínio com edital informando — arrematante RESPONDE** (*propter rem* + sucessão processual). Orientação consolidada (REsp 2.042.756/SP, mantido pelo AgInt nos EREsp 2.042.756/SP, 2ª Seção, unânime, j. 13/05/2026). **PROIBIDO** escrever "a matéria está em aberto no STJ". A brecha é o **edital omisso** — tese de defesa, jamais regra pacífica. **Tema 1.266 é matéria diversa.**

9. **Leilão negativo não quita a dívida como regra** — Lei 9.514, art. 27, **§5º-A**: o devedor continua obrigado pelo saldo. **Exceção:** imóvel residencial do devedor (art. 26-A, §4º), com extinção da dívida (e o §5º estende isso à via judicial).

10. **Defesa do fiduciante comprimida** (9.514, art. 30, §único): após arrematação ou consolidação definitiva, **nenhuma** discussão sobre cláusulas obsta a reintegração — **exceto a exigência de notificação**. **Estratégia: atacar a intimação (especialmente o §4º-B eletrônico), não o preço.**

11. **Os 90 dias do locatário contam do REGISTRO** da venda ou do compromisso (Lei 8.245, art. 8º, §2º) — **não** da alienação, não da arrematação, não da imissão. Perdido o prazo, presume-se manutenção do contrato.

12. **Evicção do arrematante — há precedente, não é carta branca.** O **REsp 1.293.147/GO** (STJ, 3ª Turma, DJe 31/03/2015) **descaracterizou a evicção e afastou a indenização** por má-fé dos adquirentes (CC art. 457): o banco arrematou e depois alienou em leilão; os compradores sabiam da litigiosidade. **Não citar como se apoiasse o arrematante de boa-fé.** Moldura: **CC 447-457**. No caso concreto: boa-fé, cadeia dominial e distinção fática.

## Divergências que o plugin DECLARA, não esconde
- **Edital omisso × condomínio** — a proposição inversa ("arrematante não responde") é **tese de defesa**, não regra.
- **Preço vil no extrajudicial** — **AREsp 2.165.101/PR**: ato localizado é **decisão monocrática do relator** no AgInt (retratação; **não localizamos acórdão colegiado na base oficial**); **não é repetitivo** e **não vincula** (art. 927). Escrever *"há linha no STJ que anula em casos concretos"*, **nunca** "tese firmada em repetitivo" nem "acórdão de Turma".
- **Comissão acima de 5% no extrajudicial** — sem julgado localizado; não transportar o RMS 65.084.
- **REsp 2.171.564/SP** (aplicação do art. 886, VI ao extrajudicial) e **Tema 1.266/STJ** — pendentes; se julgados, atualizar.

## Gaps intransponíveis (não preencher por invenção)
- **Leilão público administrativo (Lei 14.133)** — gap declarado; encaminhar a `licitacoes-adv-os`, nunca improvisar.
- **Alíquotas municipais de ITBI · emolumentos fora de SP · custas judiciais** — nunca dar número; dar a fórmula e a fonte a consultar.
- **Regulamentação registral do art. 9º da 14.711** (provimentos estaduais) — não verificada; operacionalmente decisiva.
- **Direito intertemporal do DL 70/66** — a 14.711 não traz regra de transição explícita.
- **Ato do DREI** harmonizando comissão acima do piso — inexistente até onde se buscou.

## Porta única
`leiloes-master` é o orquestrador: lê `context/metodologia-leiloes.md`, classifica via `triagem-leiloes` (**via · papel · FASE** — a fase é a que não volta atrás), carrega `memoria-de-caso-leilao`, aplica a fundação C1, **impõe o gate DUE-DILIGENCE-FIRST** antes de qualquer opinião de lance, dirime as **55 skills** das 8 camadas e fecha pela `suprema-corte-leiloes` + `validador-leiloes`. Voz e forma por `estilo-leiloes`.

## Fronteiras (cross-link soft, NÃO duplicar)
Execução até a penhora → `execucao-adv-os` · relação de AF e registral geral → `direito-imobiliario-adv-os` · visão processual geral → `civel-adv-os` · leilão público administrativo → `licitacoes-adv-os` · CTB 328 / remoção de veículo → `transito-adv-os` · especificidade da terra rural → `agrario-adv-os` (âncora: art. 9º, §13, da 14.711 **exclui** financiamento da atividade agropecuária do rito novo) · relação bancária do contrato → `bancario-adv-os` · cálculo de saldo/atualização → `calculosjudiciais-adv-os` · ITBI como tributo / ganho de capital → `tributario-societario-adv-os` · busca de jurisprudência ao vivo → `juris-adv-os`.

**OUT — gap declarado:** leilão público administrativo da Lei 14.133.
