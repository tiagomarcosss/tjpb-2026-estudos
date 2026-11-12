---
tipo: bloco
fonte: autoral
status: corrigido
disciplina: ["APF, SAFe e Testes"]
assunto: "APF/IFPUG · funções de dados (ALI × AIE × RLR, o que não se conta) + transações ligadas a elas"
semana: 2
data: 2026-11-06
---

# Bloco · APF · Funções de dados (8 questões)

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

> Reforço do bloco de 03/11 (funções de dados 0/3). Assunto único: APF. Cenários novos, sem conta de VAF. Marque "?" no que não souber e nunca deixe em branco.

## Questão 1

A analista Renata está contando os pontos de função do sistema e-CONCILIA, que agenda as sessões de conciliação de um Tribunal de Justiça. O cadastro de conciliadores (nome, matrícula, telefone e disponibilidade de agenda) é mantido pelo sistema de Gestão de Pessoas, o SIGEP-PB. O e-CONCILIA lê esse cadastro para montar as pautas e, por meio de uma funcionalidade própria, permite que o próprio conciliador atualize o campo "disponibilidade de agenda".

Na contagem do e-CONCILIA, o cadastro de conciliadores deve ser classificado como:

(A) Arquivo de Interface Externa, porque o cadastro foi criado e pertence ao SIGEP-PB;

(B) Arquivo de Interface Externa, porque a alteração de um único campo não caracteriza manutenção;

\(C) Arquivo Lógico Interno, porque o e-CONCILIA mantém esse grupo de dados por meio de um processo elementar próprio;

(D) Entrada Externa, porque o conciliador informa dados que atravessam a fronteira do e-CONCILIA;

(E) função não contada no e-CONCILIA, porque um grupo de dados só pode ser contado na aplicação de origem.

---

## Questão 2

O sistema e-AUDIÊNCIA registra as atas de audiência de um Tribunal de Justiça. Cada ata possui data, sala e magistrado e contém uma lista de deliberações (texto e prazo). Uma deliberação só existe dentro de uma ata e é gravada junto com ela. As partes (nome, CPF e endereço) são cadastradas no próprio e-AUDIÊNCIA de forma independente: uma mesma parte é reutilizada em várias atas e pode ser incluída ou alterada sem que haja audiência.

Na contagem de pontos de função do e-AUDIÊNCIA, as funções de dados devem ser identificadas como:

(A) dois Arquivos Lógicos Internos: Atas, com dois Registros Lógicos Referenciados, e Partes, com um;

(B) três Arquivos Lógicos Internos: Atas, Deliberações e Partes, cada um com um Registro Lógico Referenciado;

\(C) um Arquivo Lógico Interno, Atas, com três Registros Lógicos Referenciados;

(D) dois Arquivos Lógicos Internos: Atas, com um Registro Lógico Referenciado, e Partes, com dois;

(E) dois Arquivos Lógicos Internos e um Arquivo de Interface Externa, sendo Deliberações o arquivo externo.

---

## Questão 3

O sistema e-PROTOCOLO registra os documentos protocolados nas comarcas de um Tribunal de Justiça. Além da tabela de Protocolos, mantida pelas funcionalidades de inclusão, alteração e arquivamento, o banco de dados do e-PROTOCOLO possui duas tabelas carregadas na implantação e nunca alteradas pelo usuário: UF (sigla e nome) e Situação do Protocolo (código e descrição: "recebido", "em análise", "arquivado"). Essas duas tabelas servem apenas para preencher listas de seleção nas telas.

Na contagem de pontos de função do e-PROTOCOLO, devem ser contados como funções de dados:

(A) três Arquivos Lógicos Internos: Protocolos, UF e Situação do Protocolo;

(B) um Arquivo Lógico Interno e dois Arquivos de Interface Externa;

\(C) um Arquivo Lógico Interno, Protocolos, com três Registros Lógicos Referenciados;

(D) um Arquivo Lógico Interno, Protocolos, e um Arquivo de Interface Externa, UF, pois a lista de estados segue o padrão do IBGE;

(E) apenas Protocolos, como Arquivo Lógico Interno, pois UF e Situação do Protocolo são dados de código.

---

## Questão 4

O sistema e-DEPÓSITO controla os depósitos judiciais de um Tribunal de Justiça. Todos os dias, o banco conveniado envia um arquivo com os depósitos realizados. O e-DEPÓSITO lê o arquivo, valida cada registro e grava os depósitos na sua própria base de dados, que só ele mantém.

Na contagem de pontos de função do e-DEPÓSITO, a funcionalidade de carga do arquivo e a base de depósitos devem ser contadas, respectivamente, como:

(A) Arquivo de Interface Externa e Arquivo Lógico Interno;

(B) Entrada Externa e Arquivo Lógico Interno;

\(C) Arquivo de Interface Externa e Arquivo de Interface Externa;

(D) Entrada Externa e Arquivo de Interface Externa, pois os dados se originam no banco conveniado;

(E) Arquivo de Interface Externa, apenas, pois a carga em lote não é contada como transação.

---

## Questão 5

Durante um treinamento de APF, o instrutor apresentou as afirmativas a seguir sobre funções de dados.

I\. Todo Arquivo de Interface Externa de uma aplicação deve ser mantido como Arquivo Lógico Interno em alguma outra aplicação.

II. Um mesmo grupo lógico de dados pode ser Arquivo Lógico Interno em uma aplicação e Arquivo de Interface Externa em outra.

III. Um Arquivo de Interface Externa pode ser alterado pela aplicação que está sendo contada, desde que a alteração seja eventual.

Está correto o que se afirma em

(A) I, apenas.

(B) II, apenas.

\(C) III, apenas.

(D) I e II, apenas.

(E) I, II e III.

---

## Questão 6

No banco de dados do sistema SIGEP-PB, os dados de um servidor estão normalizados em três tabelas físicas: SERVIDOR (matrícula, nome e cargo), SERVIDOR_ENDERECO (um endereço por servidor) e SERVIDOR_CONTATO (vários telefones e e-mails por servidor). Endereço e contatos só existem vinculados a um servidor e são mantidos na mesma tela de cadastro. Para o usuário da área de Gestão de Pessoas, tudo isso é "o cadastro do servidor".

Na contagem de pontos de função do SIGEP-PB, essas três tabelas devem ser consideradas como:

(A) um Arquivo Lógico Interno, pois a APF considera o agrupamento lógico na visão do usuário, e não as tabelas físicas;

(B) três Arquivos Lógicos Internos, um para cada tabela física;

\(C) dois Arquivos Lógicos Internos: Servidor e Contatos, pois a relação um-para-muitos gera um arquivo separado;

(D) um Arquivo Lógico Interno e dois Arquivos de Interface Externa;

(E) nenhuma função de dados, pois tabelas normalizadas são detalhes de implementação.

---

## Questão 7

O sistema SisPLANTÃO monta as escalas de plantão judicial de um Tribunal de Justiça, com funcionalidades de inclusão, alteração e exclusão de escalas. Para impedir que um servidor de férias seja escalado, o SisPLANTÃO consulta, por uma API REST, os períodos de férias mantidos exclusivamente pelo SIGEP-PB. O SisPLANTÃO também grava um log técnico de erros, usado apenas pela equipe de infraestrutura para depuração.

Considerando apenas as funções de dados, a contagem do SisPLANTÃO deve identificar:

(A) dois Arquivos Lógicos Internos: Escalas e Férias, pois o SisPLANTÃO utiliza os dois;

(B) dois Arquivos Lógicos Internos, Escalas e Log, e um Arquivo de Interface Externa, Férias;

\(C) um Arquivo Lógico Interno, Escalas, e dois Arquivos de Interface Externa, Férias e Log;

(D) um Arquivo Lógico Interno, Escalas, apenas, pois dados obtidos por API não são funções de dados;

(E) um Arquivo Lógico Interno, Escalas, e um Arquivo de Interface Externa, Férias.

---

## Questão 8

O sistema e-LICENÇA, de um Tribunal de Justiça, possui três funcionalidades: (1) o servidor preenche o pedido de licença médica, que é validado e gravado na base do sistema; (2) a chefia aprova o pedido, o que altera a situação gravada; (3) a Diretoria de Pessoas emite um relatório mensal com o total de dias de licença por setor, calculado pelo sistema. Os pedidos ficam armazenados numa base mantida apenas pelo e-LICENÇA.

As três funcionalidades e a base de pedidos devem ser contadas como:

(A) uma Entrada Externa, uma Consulta Externa, uma Saída Externa e um Arquivo Lógico Interno;

(B) duas Entradas Externas, uma Consulta Externa e um Arquivo Lógico Interno;

\(C) duas Entradas Externas, uma Saída Externa e um Arquivo Lógico Interno;

(D) três Entradas Externas e um Arquivo Lógico Interno;

(E) duas Entradas Externas, uma Saída Externa e um Arquivo de Interface Externa.

---

## Minhas respostas

| Questão | Resposta |
|---|---|
| 1 | |
| 2 | |
| 3 | |
| 4 | |
| 5 | |
| 6 | |
| 7 | |
| 8 | |
