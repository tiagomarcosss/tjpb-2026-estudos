---
tipo: bloco
fonte: autoral
status: pendente
disciplina: ["APF, SAFe e Testes"]
assunto: "APF/IFPUG (classificação de funções, telas, VAF e conceitos)"
semana: 2
data: 2026-11-03
---

# Bloco · APF/IFPUG · padrão FGV (8 questões)

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

> Assunto único: Análise de Pontos de Função. Formato baseado nas questões reais da FGV (TJ-RJ 2026, MPU 2025, TJ-PI 2015): classificar funções a partir de um cenário, contar funções em telas, calcular o VAF e reconhecer propriedades da técnica. Sem tabelas de DER/RLR. Marque "?" no que não souber e nunca deixe em branco.

## Questão 1

O sistema CUSTAS-JUD é utilizado pelos cartórios de um Tribunal de Justiça para controlar o recolhimento de custas processuais. O CUSTAS-JUD possui uma funcionalidade por meio da qual o servidor do cartório informa os dados de uma guia de custas paga (número da guia, valor e data de pagamento), que são validados e armazenados na base de dados do sistema. Para os advogados, o CUSTAS-JUD disponibiliza outra funcionalidade que emite o demonstrativo de custas de um processo, no qual o sistema soma os valores de todas as guias pagas e calcula o saldo devedor atualizado.

Com base na Análise de Pontos de Função (APF), as funcionalidades supracitadas do CUSTAS-JUD serão contadas, respectivamente, como:

(A) Saída Externa e Consulta Externa;

(B) Entrada Externa e Consulta Externa;

\(C) Arquivo Lógico Interno e Saída Externa;

(D) Consulta Externa e Saída Externa;

(E) Entrada Externa e Saída Externa.

---

## Questão 2

Durante a contagem de pontos de função do sistema de Cadastro de Peritos de um Tribunal de Justiça, as telas do sistema foram utilizadas como subsídio:

- **Tela 1 · Cadastro de Perito:** campos nome, CPF, telefone, e-mail e comarca de atuação (lista suspensa), com os botões Incluir, Alterar e Excluir.
- **Tela 2 · aba Especialidades:** grade com a especialidade e o número de registro no conselho profissional. Uma especialidade só existe vinculada a um perito e é gravada junto com ele, pelos botões da Tela 1.

A lista de comarcas exibida na Tela 1 é lida de uma tabela mantida exclusivamente pelo sistema de Organização Judiciária do Tribunal.

Considerando apenas as Entradas Externas e as funções de dados, o cadastro apresentado deve ser contado como:

(A) uma Entrada Externa, um Arquivo Lógico Interno e um Arquivo de Interface Externa;

(B) três Entradas Externas e dois Arquivos Lógicos Internos;

\(C) três Entradas Externas, um Arquivo Lógico Interno e um Arquivo de Interface Externa;

(D) três Entradas Externas, dois Arquivos Lógicos Internos e um Arquivo de Interface Externa;

(E) seis Entradas Externas, dois Arquivos Lógicos Internos e um Arquivo de Interface Externa.

---

## Questão 3

A Análise de Pontos de Função mede o tamanho funcional de um software sob a ótica do usuário. No processo de contagem, a transação cujo objetivo principal é apresentar informações ao usuário por meio de uma lógica de processamento que contenha ao menos uma fórmula matemática ou cálculo, ou que crie dados derivados, é classificada como

(A) entrada externa.

(B) consulta externa.

\(C) arquivo de interface externa.

(D) saída externa.

(E) arquivo lógico interno.

---

## Questão 4

O escritório de métricas de um Tribunal de Justiça contou o sistema de Precatórios e obteve 120 pontos de função não ajustados. Em seguida, levantou o nível de influência de cada uma das 14 características gerais do sistema:

- COMUNICAÇÃO DE DADOS: 3
- PROCESSAMENTO DISTRIBUÍDO: 1
- PERFORMANCE: 4
- UTILIZAÇÃO DO EQUIPAMENTO: 2
- VOLUME DE TRANSAÇÕES: 3
- ENTRADA DE DADOS ON-LINE: 2
- EFICIÊNCIA DO USUÁRIO FINAL: 1
- ATUALIZAÇÃO ON-LINE: 0
- PROCESSAMENTO COMPLEXO: 2
- REUTILIZAÇÃO DE CÓDIGO: 1
- FACILIDADE DE IMPLANTAÇÃO: 0
- FACILIDADE OPERACIONAL: 3
- MÚLTIPLOS LOCAIS: 1
- FACILIDADE DE MUDANÇAS: 2

A partir dessas informações, o valor dos pontos de função ajustados é:

(A) 108;

(B) 90;

\(C) 120;

(D) 150;

(E) 102.

---

## Questão 5

A Secretaria de TI de um Tribunal de Justiça passou a contratar o desenvolvimento de software medido em pontos de função. Sobre a técnica, analise as afirmativas a seguir.

I\. A Análise de Pontos de Função mede o tamanho do software a partir das funcionalidades solicitadas e recebidas pelo usuário.

II. Dois sistemas com as mesmas funcionalidades, um desenvolvido em Java e outro em Python, terão tamanhos diferentes em pontos de função, porque linguagens diferentes exigem quantidades diferentes de linhas de código.

III. O tamanho em pontos de função pode servir de base para estimar esforço e custo, desde que combinado com a produtividade da equipe ou do fornecedor.

Está correto o que se afirma em

(A) I, apenas.

(B) I e III, apenas.

\(C) II, apenas.

(D) II e III, apenas.

(E) I, II e III.

---

## Questão 6

O Sistema de Diárias (SisDiárias) de um Tribunal de Justiça registra, altera e aprova as solicitações de diárias dos servidores. Para preencher automaticamente o nome, o cargo e a lotação do solicitante, o SisDiárias apenas lê o cadastro de servidores, que é mantido exclusivamente pelo Sistema de Gestão de Pessoas. As duas bases ficam armazenadas no mesmo servidor de banco de dados corporativo do Tribunal.

Na contagem de pontos de função do SisDiárias, o cadastro de servidores e o cadastro de solicitações de diárias devem ser classificados, respectivamente, como:

(A) Arquivo de Interface Externa e Arquivo Lógico Interno;

(B) Arquivo Lógico Interno e Arquivo de Interface Externa;

\(C) Arquivo Lógico Interno e Arquivo Lógico Interno, pois ambos são utilizados pelo SisDiárias;

(D) Arquivo de Interface Externa e Arquivo de Interface Externa, pois ambos ficam no banco de dados corporativo;

(E) Entrada Externa e Arquivo Lógico Interno, pois o cadastro de servidores fornece dados de entrada ao SisDiárias.

---

## Questão 7

O sistema GABINETE apoia o trabalho dos magistrados de um Tribunal de Justiça. Por meio de uma primeira funcionalidade, o juiz solicita a lista dos processos conclusos ao seu gabinete, com a quantidade de dias em que cada processo está concluso, calculada pelo sistema a partir da data atual e da data da conclusão. Por meio de uma segunda funcionalidade, o assessor informa o número de um processo e o sistema exibe a classe, o assunto e as partes, exatamente como estão armazenados na base de dados.

Com base na Análise de Pontos de Função (APF), as funcionalidades supracitadas serão contadas, respectivamente, como:

(A) Consulta Externa e Consulta Externa, pois ambas apenas apresentam dados ao usuário;

(B) Entrada Externa e Consulta Externa;

\(C) Consulta Externa e Saída Externa;

(D) Saída Externa e Consulta Externa;

(E) Saída Externa e Saída Externa, pois ambas recuperam dados de Arquivos Lógicos Internos.

---

## Questão 8

Na contagem de pontos de função do sistema de Mandados de um Tribunal de Justiça, o analista identificou as seguintes estruturas no banco de dados:

I\. tabela de Mandados, mantida pelas funcionalidades de expedição e de registro de cumprimento do próprio sistema;

II. tabela temporária, criada apenas para ordenar o resultado de um relatório e descartada ao final do processamento;

III. índice criado sobre a coluna do número do processo, para acelerar as buscas;

IV. arquivo de backup diário da tabela de Mandados.

Devem ser contados como Arquivo Lógico Interno:

(A) I, II, III e IV.

(B) I e IV, apenas.

\(C) I, apenas.

(D) I e II, apenas.

(E) I, III e IV, apenas.

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
