---
tipo: correcao
fonte: autoral
disciplina: ["APF, SAFe e Testes"]
assunto: "APF/IFPUG · funções de dados (ALI × AIE × RLR, o que não se conta) + transações ligadas a elas"
semana: 3
data: 2026-11-11
acertos: 5
total: 8
---

# Correção · APF · Funções de dados (8 questões)

**Data:** 11/11/2026 (bloco de 06/11) · **Semana 3** · **Placar: 5/8 (62%)** · 3 erros · 0 "não sabia"

**Respostas lidas das anotações do PDF:** 1-A · 2-A · 3-C · 4-B · 5-B · 6-A · 7-E · 8-C

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

> **Como li as marcas:** usei os círculos nas letras (a tabela "Minhas respostas" ficou vazia). **Nenhum "?"**. Na Q4, há **pontinho na (B) e na (D)** (duas candidatas) e o círculo na (B): conta como **acerto com dúvida**. Na Q3, você **riscou a palavra "Protocolos" da (E)**, que era a certa.

| Questão | Assunto | Sua | Gabarito | Resultado |
|---|---|---|---|---|
| 1 | ALI × AIE: aplicação que altera um campo | A | C | ❌ |
| 2 | ALI com RLR × ALI independente | A | A | ✅ |
| 3 | Tabelas de código (UF, situação) | C | E | ❌ |
| 4 | Carga de arquivo (EE) + base própria (ALI) | B (pontinho em B e D) | B | ✅ com dúvida |
| 5 | Propriedades do AIE (I/II/III) | B | D | ❌ |
| 6 | Tabelas físicas normalizadas = 1 ALI | A | A | ✅ |
| 7 | API de outro sistema (AIE) + log técnico | E | E | ✅ |
| 8 | EE, EE, SE + ALI | C | C | ✅ |

**Por tipo:**

| Tipo | Questões | Placar |
|---|---|---|
| Agrupamento lógico: RLR × ALI, tabelas físicas | 2, 6 | **2/2** |
| Transações ligadas aos dados (EE, SE) | 4, 8 | **2/2** (1 com dúvida) |
| Quem mantém: ALI × AIE | 1, 7 | 1/2 |
| O que não conta (log, tabela de código) | 3, 7 | 1/2 |
| Teoria do AIE (I/II/III) | 5 | 0/1 |

**Acertos firmes:** 4 de 5 (a Q4 teve duas candidatas). **Erros convictos:** 3 de 3, sem "?".

**Comparação:** funções de dados estavam em **0/3** no bloco de 03/11 e agora estão em **5/8**. O **agrupamento lógico ficou firme**: deliberação dentro da ata (Q2) e as três tabelas do servidor como um único cadastro (Q6). Você também separou bem o que é dado do que é ação (Q8: escreveu EE, EE, SE no enunciado). Falta fechar **três regras pontuais**:

1. Quem **altera** o dado também mantém, mesmo que não tenha criado (Q1).
2. **Tabela de código** não conta (Q3).
3. Todo AIE é ALI de **outro** sistema (Q5).

**APF funções de dados sai da fila** (teoria de 03/11 + bloco corrigido). As três regras ficam como ponto fraco.

---

## Questão 1 · ❌ Errou

A analista Renata está contando os pontos de função do sistema e-CONCILIA, que agenda as sessões de conciliação de um Tribunal de Justiça. O cadastro de conciliadores (nome, matrícula, telefone e disponibilidade de agenda) é mantido pelo sistema de Gestão de Pessoas, o SIGEP-PB. O e-CONCILIA lê esse cadastro para montar as pautas e, por meio de uma funcionalidade própria, permite que o próprio conciliador atualize o campo "disponibilidade de agenda".

Na contagem do e-CONCILIA, o cadastro de conciliadores deve ser classificado como:

❌ (A) Arquivo de Interface Externa, porque o cadastro foi criado e pertence ao SIGEP-PB; ← sua resposta

(B) Arquivo de Interface Externa, porque a alteração de um único campo não caracteriza manutenção;

✅ **\(C) Arquivo Lógico Interno, porque o e-CONCILIA mantém esse grupo de dados por meio de um processo elementar próprio;**

(D) Entrada Externa, porque o conciliador informa dados que atravessam a fronteira do e-CONCILIA;

(E) função não contada no e-CONCILIA, porque um grupo de dados só pode ser contado na aplicação de origem.

**Onde você se confundiu:** você leu "é mantido pelo SIGEP-PB" e "lê esse cadastro" e fechou em AIE, justificado por **quem criou** o cadastro. Faltou a última frase: "**por meio de uma funcionalidade própria, permite que o próprio conciliador atualize** o campo". Atualizar é manter. A partir daí, o e-CONCILIA também mantém o grupo de dados.

**A regra:** o que decide ALI × AIE é se a aplicação contada **inclui, altera ou exclui** o dado por um processo próprio. **Basta uma** das três, e basta **um campo**. Quem criou ou de quem o dado "é" não entra na conta. O mesmo grupo pode ser **ALI nas duas aplicações** que o mantêm.

**Por que as outras erram:** (A) usa a origem como critério · (B) diz que um campo só não caracteriza manutenção, mas caracteriza · (D) a atualização é uma EE, mas a pergunta é sobre o **cadastro** (o dado), não sobre a ação · (E) um grupo de dados pode ser contado em mais de uma aplicação.

📌 **ALI × AIE = a aplicação contada altera o dado? Se altera (mesmo um campo, por funcionalidade própria), é ALI.** "Foi criado por outro" e "pertence a outro" não decidem. Leia o enunciado **até o fim** procurando "atualiza", "altera", "inclui".

---

## Questão 2 · ✅ Acertou

O sistema e-AUDIÊNCIA registra as atas de audiência de um Tribunal de Justiça. Cada ata possui data, sala e magistrado e contém uma lista de deliberações (texto e prazo). Uma deliberação só existe dentro de uma ata e é gravada junto com ela. As partes (nome, CPF e endereço) são cadastradas no próprio e-AUDIÊNCIA de forma independente: uma mesma parte é reutilizada em várias atas e pode ser incluída ou alterada sem que haja audiência.

Na contagem de pontos de função do e-AUDIÊNCIA, as funções de dados devem ser identificadas como:

✅ **(A) dois Arquivos Lógicos Internos: Atas, com dois Registros Lógicos Referenciados, e Partes, com um;** ← sua resposta

(B) três Arquivos Lógicos Internos: Atas, Deliberações e Partes, cada um com um Registro Lógico Referenciado;

\(C) um Arquivo Lógico Interno, Atas, com três Registros Lógicos Referenciados;

(D) dois Arquivos Lógicos Internos: Atas, com um Registro Lógico Referenciado, e Partes, com dois;

(E) dois Arquivos Lógicos Internos e um Arquivo de Interface Externa, sendo Deliberações o arquivo externo.

**Por quê:** você circulou ata, deliberações e partes e sublinhou "independente". A deliberação só existe dentro da ata, então é **RLR** de Atas (Atas fica com 2 RLR: a ata e a deliberação). A parte vive sozinha, então é **ALI próprio**. (B) faz da deliberação um arquivo · \(C) junta as partes, que são independentes · (D) inverte os RLR · (E) a deliberação é gravada pelo próprio sistema, não pode ser externa.

📌 "Só existe dentro de" = **RLR** do pai. "Independente, reutilizado, incluído sem o outro" = **ALI próprio**.

---

## Questão 3 · ❌ Errou

O sistema e-PROTOCOLO registra os documentos protocolados nas comarcas de um Tribunal de Justiça. Além da tabela de Protocolos, mantida pelas funcionalidades de inclusão, alteração e arquivamento, o banco de dados do e-PROTOCOLO possui duas tabelas carregadas na implantação e nunca alteradas pelo usuário: UF (sigla e nome) e Situação do Protocolo (código e descrição: "recebido", "em análise", "arquivado"). Essas duas tabelas servem apenas para preencher listas de seleção nas telas.

Na contagem de pontos de função do e-PROTOCOLO, devem ser contados como funções de dados:

(A) três Arquivos Lógicos Internos: Protocolos, UF e Situação do Protocolo;

(B) um Arquivo Lógico Interno e dois Arquivos de Interface Externa;

❌ \(C) um Arquivo Lógico Interno, Protocolos, com três Registros Lógicos Referenciados; ← sua resposta

(D) um Arquivo Lógico Interno, Protocolos, e um Arquivo de Interface Externa, UF, pois a lista de estados segue o padrão do IBGE;

✅ **(E) apenas Protocolos, como Arquivo Lógico Interno, pois UF e Situação do Protocolo são dados de código.**

**Onde você se confundiu:** você percebeu que UF e Situação não são ALI (riscou a (A)) e nem AIE (riscou a (B)). Bom. Mas, para não "perder" as duas tabelas, você as colocou como **RLR** dentro de Protocolos. E **riscou "Protocolos" na (E)**, a certa, sem apontar a palavra errada nela (ponto fraco 0a).

**A regra:** tabela **carregada na implantação, nunca alterada pelo usuário, que só preenche lista de seleção** é **dado de código** (também chamado de dado de referência ou domínio). Ela **não conta como nada**: nem ALI, nem AIE, nem RLR. O "nunca alteradas pelo usuário" e o "servem apenas para preencher listas" do enunciado são as pistas.

**Por que as outras erram:** (A) e (B) contam as tabelas de código como arquivos · \(C) as transforma em subgrupos, mas RLR é subgrupo de dados de negócio que só existe dentro do pai (como a deliberação da Q2) · (D) "padrão do IBGE" não torna nada AIE (AIE é ALI de **outra aplicação**, não de um padrão).

📌 **Tabela de código (UF, situação, tipo, sexo, estado civil) carregada na implantação e nunca mantida pelo usuário: não conta.** Não é ALI, AIE nem RLR. Na margem, anote "✗ código".

---

## Questão 4 · ✅ Acertou (com dúvida)

O sistema e-DEPÓSITO controla os depósitos judiciais de um Tribunal de Justiça. Todos os dias, o banco conveniado envia um arquivo com os depósitos realizados. O e-DEPÓSITO lê o arquivo, valida cada registro e grava os depósitos na sua própria base de dados, que só ele mantém.

Na contagem de pontos de função do e-DEPÓSITO, a funcionalidade de carga do arquivo e a base de depósitos devem ser contadas, respectivamente, como:

(A) Arquivo de Interface Externa e Arquivo Lógico Interno;

✅ **(B) Entrada Externa e Arquivo Lógico Interno;** ← sua resposta (pontinho)

\(C) Arquivo de Interface Externa e Arquivo de Interface Externa;

(D) Entrada Externa e Arquivo de Interface Externa, pois os dados se originam no banco conveniado; ← pontinho

(E) Arquivo de Interface Externa, apenas, pois a carga em lote não é contada como transação.

**Por quê:** você escreveu "ALI" em cima do e-DEPÓSITO e destacou "grava os depósitos" e "sua própria base". Carga de arquivo = **ação** que traz dado de fora e grava = **EE**. A base que só ele mantém = **ALI**. 

**A pista entre B e D:** a (D) justifica o AIE pela **origem** do dado ("se originam no banco"). Origem não decide nada (é o mesmo erro da Q1). O enunciado diz "**que só ele mantém**", então é ALI. (A), \(C) e (E) chamam a carga, que é uma ação, de arquivo.

📌 Arquivo que **chega** de fora e é **gravado** na sua base = **EE** (a carga) + **ALI** (a base). De onde o dado veio não importa.

---

## Questão 5 · ❌ Errou

Durante um treinamento de APF, o instrutor apresentou as afirmativas a seguir sobre funções de dados.

I\. Todo Arquivo de Interface Externa de uma aplicação deve ser mantido como Arquivo Lógico Interno em alguma outra aplicação.

II. Um mesmo grupo lógico de dados pode ser Arquivo Lógico Interno em uma aplicação e Arquivo de Interface Externa em outra.

III. Um Arquivo de Interface Externa pode ser alterado pela aplicação que está sendo contada, desde que a alteração seja eventual.

Está correto o que se afirma em

(A) I, apenas.

❌ (B) II, apenas. ← sua resposta

\(C) III, apenas.

✅ **(D) I e II, apenas.**

(E) I, II e III.

**Onde você se confundiu:** III com X está certo (AIE nunca é alterado pela aplicação contada). O erro foi o **X no I**. O item I é a **definição** do AIE no IFPUG: o AIE é o ALI de **outra** aplicação, visto de fora. Se ninguém mantém aquele dado como ALI, ele não é AIE de ninguém. Você aceitou o II, que é a mesma ideia vista pelo outro lado: o cadastro de férias é ALI do SIGEP-PB e AIE do SisPLANTÃO (Q7).

**Provável raciocínio:** "e se o dado vier de fora, de um arquivo do IBGE ou de um banco?". Nesse caso, ou ele é gravado e vira ALI (Q4), ou é código (Q3). Não existe AIE "solto", sem uma aplicação dona.

📌 **Todo AIE é ALI de alguma outra aplicação** (I) · o mesmo grupo pode ser ALI numa e AIE noutra (II) · AIE **nunca** é alterado pela aplicação contada: se alterar, vira ALI (III falso, e é a Q1).

---

## Questão 6 · ✅ Acertou

No banco de dados do sistema SIGEP-PB, os dados de um servidor estão normalizados em três tabelas físicas: SERVIDOR (matrícula, nome e cargo), SERVIDOR_ENDERECO (um endereço por servidor) e SERVIDOR_CONTATO (vários telefones e e-mails por servidor). Endereço e contatos só existem vinculados a um servidor e são mantidos na mesma tela de cadastro. Para o usuário da área de Gestão de Pessoas, tudo isso é "o cadastro do servidor".

Na contagem de pontos de função do SIGEP-PB, essas três tabelas devem ser consideradas como:

✅ **(A) um Arquivo Lógico Interno, pois a APF considera o agrupamento lógico na visão do usuário, e não as tabelas físicas;** ← sua resposta

(B) três Arquivos Lógicos Internos, um para cada tabela física;

\(C) dois Arquivos Lógicos Internos: Servidor e Contatos, pois a relação um-para-muitos gera um arquivo separado;

(D) um Arquivo Lógico Interno e dois Arquivos de Interface Externa;

(E) nenhuma função de dados, pois tabelas normalizadas são detalhes de implementação.

**Por quê:** você destacou "o cadastro do servidor": é a visão do usuário que manda. (B) conta tabela física · \(C) 1:N não gera arquivo, gera no máximo RLR · (D) tudo é mantido pelo próprio SIGEP-PB · (E) exagera: a tabela física é detalhe, mas o grupo lógico conta.

📌 APF conta **grupos lógicos na visão do usuário**, nunca tabelas físicas. Normalização não multiplica ALI.

---

## Questão 7 · ✅ Acertou

O sistema SisPLANTÃO monta as escalas de plantão judicial de um Tribunal de Justiça, com funcionalidades de inclusão, alteração e exclusão de escalas. Para impedir que um servidor de férias seja escalado, o SisPLANTÃO consulta, por uma API REST, os períodos de férias mantidos exclusivamente pelo SIGEP-PB. O SisPLANTÃO também grava um log técnico de erros, usado apenas pela equipe de infraestrutura para depuração.

Considerando apenas as funções de dados, a contagem do SisPLANTÃO deve identificar:

(A) dois Arquivos Lógicos Internos: Escalas e Férias, pois o SisPLANTÃO utiliza os dois;

(B) dois Arquivos Lógicos Internos, Escalas e Log, e um Arquivo de Interface Externa, Férias;

\(C) um Arquivo Lógico Interno, Escalas, e dois Arquivos de Interface Externa, Férias e Log;

(D) um Arquivo Lógico Interno, Escalas, apenas, pois dados obtidos por API não são funções de dados;

✅ **(E) um Arquivo Lógico Interno, Escalas, e um Arquivo de Interface Externa, Férias.** ← sua resposta

**Por quê:** você riscou "dois" nas alternativas que contavam o log e a palavra "Arquivos" onde não cabia. Escalas = ALI (inclui, altera, exclui). Férias = só consulta, "mantidos **exclusivamente** pelo SIGEP-PB" = AIE (aqui o "exclusivamente" fecha a porta que estava aberta na Q1). Log técnico = não conta. (A) "utiliza" ≠ mantém · (B) e \(C) contam o log · (D) o meio (API, arquivo, banco) não importa.

📌 Consulta por API de dado **mantido só pelo outro** = AIE. Log técnico = não conta.

---

## Questão 8 · ✅ Acertou

O sistema e-LICENÇA, de um Tribunal de Justiça, possui três funcionalidades: (1) o servidor preenche o pedido de licença médica, que é validado e gravado na base do sistema; (2) a chefia aprova o pedido, o que altera a situação gravada; (3) a Diretoria de Pessoas emite um relatório mensal com o total de dias de licença por setor, calculado pelo sistema. Os pedidos ficam armazenados numa base mantida apenas pelo e-LICENÇA.

As três funcionalidades e a base de pedidos devem ser contadas como:

(A) uma Entrada Externa, uma Consulta Externa, uma Saída Externa e um Arquivo Lógico Interno;

(B) duas Entradas Externas, uma Consulta Externa e um Arquivo Lógico Interno;

✅ **\(C) duas Entradas Externas, uma Saída Externa e um Arquivo Lógico Interno;** ← sua resposta

(D) três Entradas Externas e um Arquivo Lógico Interno;

(E) duas Entradas Externas, uma Saída Externa e um Arquivo de Interface Externa.

**Por quê:** você escreveu EE, EE e SE em cima de cada funcionalidade. Gravar = EE; aprovar altera o dado gravado = EE; relatório com total **calculado** = SE. Base mantida só por ele = ALI. (A) e (B) tratam a aprovação ou o relatório como consulta · (D) relatório não grava nada · (E) a base é dele: ALI.

📌 Grava ou altera = **EE** · sai com cálculo/total = **SE** · sai só recuperando = **CE**.

---

## Para o caderno de erros

| Assunto | Por que errei | Regra certa |
|---|---|---|
| ALI × AIE (Q1) | Decidi por quem criou o cadastro e não li até o "permite que o conciliador atualize" | Se a aplicação contada altera o dado (mesmo um campo, por funcionalidade própria), é ALI. Origem não decide |
| Tabela de código (Q3) | Pus UF e Situação como RLR para "não perder" as tabelas e risquei "Protocolos" na certa | Tabela carregada na implantação e nunca mantida pelo usuário não conta: nem ALI, nem AIE, nem RLR |
| Definição de AIE (Q5, item I) | Achei que podia existir AIE sem dono | Todo AIE é ALI de alguma outra aplicação. AIE nunca é alterado pela aplicação contada |

---

## O que estudar agora

| Quando | O que fazer |
|---|---|
| Agora, 5 min | Reler as 3 regras 📌 dos erros e refazer **Q1, Q3 e Q5** sem olhar, escrevendo na margem a lista "coisa → ALI/AIE/RLR/✗" |
| 22:40 · revisão | Regras 📌 de hoje (árvores e APF) + revisão espaçada de 04/11 + 15 min de Anki |
| Qui 12/11 · almoço | 🔴 **G. Semântica e reescrita** (1º da fila de Português) |
| Qui 12/11 · 19h Bloco 1 | 🔴 **Hash:** diagnóstico pronto (8 questões), último item de Específicas da fila |
| Qui 12/11 · 20h Bloco 2 | Com a fila de Específicas vazia, segue o plano da Semana 3: 🟡 **busca e ordenação** (complexidade e estabilidade; pedir a teoria ao Claude). Depois: POO, SOLID e GoF (🔴) |
| Dom 15/11 · 13h | Simulado de domingo (rotina do plano) |

**Hábito para a prova:** nas questões de funções de dados, faça a lista na margem (como fez na Q8 com EE, EE, SE) **antes** das alternativas. E não risque uma alternativa sem apontar a palavra errada: na Q3, a palavra riscada ("Protocolos") estava certa.
