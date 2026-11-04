---
tipo: correcao
fonte: autoral
disciplina: ["APF, SAFe e Testes"]
assunto: "APF/IFPUG: classificação de funções, telas, VAF e conceitos (8 questões)"
semana: 2
data: 2026-11-03
acertos: 3
total: 8
---

# Correção · APF/IFPUG · padrão FGV · 8 questões

**Data:** 03/11/2026 · **Semana 2** · **Placar: 3/8 (38%)** · 4 erros · 1 em branco ("?")

**Respostas lidas das anotações do PDF:** 1-C · 2-E · 3-D · 4-em branco (?) · 5-B · 6-C · 7-D · 8-E

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

> **Como li as marcas:** na Q4 há só um "?" grande ao lado da lista e nenhuma letra marcada (não sabia a fórmula do VAF). Na Q2 há pontinhos em (D) e (E), com círculo em (E). Na Q6 há pontinho ao lado da (C), a circulada. Na Q8 você marcou V em I, F em II, V em III e V em IV.

| Questão | Assunto | Sua | Gabarito | Resultado |
|---|---|---|---|---|
| 1 | Cenário: grava guia + demonstrativo com soma | C | E | ❌ |
| 2 | Telas de cadastro: EE, ALI e AIE | E | C | ❌ |
| 3 | Definição de SE | D | D | ✅ |
| 4 | Cálculo do PF ajustado (VAF) | — | A | ⬜ em branco (?) |
| 5 | Propriedades da APF (I/II/III) | B | B | ✅ |
| 6 | ALI × AIE (quem mantém) | C | A | ❌ (com dúvida) |
| 7 | SE × CE (dado derivado) | D | D | ✅ |
| 8 | O que não é ALI | E | C | ❌ |

**Por tipo:**

| Tipo | Questões | Placar |
|---|---|---|
| Transações: EE × SE × CE | 1, 3, 7 | 2/3 |
| Funções de dados: ALI × AIE × RLR | 2, 6, 8 | 0/3 |
| Conceito e VAF | 4, 5 | 1/2 |

**Comparação:** primeiro bloco de APF, estudado hoje só pelo texto e pelas tabelas no chat. A parte de **transações já está boa** (SE × CE 2/2). O problema está todo nas **funções de dados**: em quatro questões você tratou como ALI algo que não é um ALI separado (o "armazenar" da Q1, a especialidade da Q2, o cadastro lido da Q6 e o backup/índice da Q8). É um erro só, repetido: **confundir "o sistema usa ou grava" com "é um ALI separado"**.

---

## Questão 1 · ❌ Errou

O sistema CUSTAS-JUD é utilizado pelos cartórios de um Tribunal de Justiça para controlar o recolhimento de custas processuais. O CUSTAS-JUD possui uma funcionalidade por meio da qual o servidor do cartório informa os dados de uma guia de custas paga (número da guia, valor e data de pagamento), que são validados e armazenados na base de dados do sistema. Para os advogados, o CUSTAS-JUD disponibiliza outra funcionalidade que emite o demonstrativo de custas de um processo, no qual o sistema soma os valores de todas as guias pagas e calcula o saldo devedor atualizado.

Com base na Análise de Pontos de Função (APF), as funcionalidades supracitadas do CUSTAS-JUD serão contadas, respectivamente, como:

(A) Saída Externa e Consulta Externa;

(B) Entrada Externa e Consulta Externa;

❌ **\(C) Arquivo Lógico Interno e Saída Externa;** ← sua resposta

(D) Consulta Externa e Saída Externa;

✅ **(E) Entrada Externa e Saída Externa.**

**Onde você se confundiu:** você sublinhou "armazenados na base de dados do sistema" e marcou ALI. Só que a pergunta é sobre **funcionalidades**, e funcionalidade é sempre **transação** (EE, SE, CE). O ALI é a **tabela** onde a guia fica guardada, não a **ação** de guardar. A ação de informar dados que são gravados é a **EE**. A segunda parte você acertou: "soma" e "calcula" → SE.

📌 **"Funcionalidade" é sempre transação (EE, SE ou CE). ALI e AIE são os dados guardados, nunca a ação.** Quem grava dado vindo de fora é EE; o lugar onde ele fica é o ALI.

---

## Questão 2 · ❌ Errou (pontinhos em D e E)

Durante a contagem de pontos de função do sistema de Cadastro de Peritos de um Tribunal de Justiça, as telas do sistema foram utilizadas como subsídio:

- **Tela 1 · Cadastro de Perito:** campos nome, CPF, telefone, e-mail e comarca de atuação (lista suspensa), com os botões Incluir, Alterar e Excluir.
- **Tela 2 · aba Especialidades:** grade com a especialidade e o número de registro no conselho profissional. Uma especialidade só existe vinculada a um perito e é gravada junto com ele, pelos botões da Tela 1.

A lista de comarcas exibida na Tela 1 é lida de uma tabela mantida exclusivamente pelo sistema de Organização Judiciária do Tribunal.

Considerando apenas as Entradas Externas e as funções de dados, o cadastro apresentado deve ser contado como:

(A) uma Entrada Externa, um Arquivo Lógico Interno e um Arquivo de Interface Externa;

(B) três Entradas Externas e dois Arquivos Lógicos Internos;

✅ **\(C) três Entradas Externas, um Arquivo Lógico Interno e um Arquivo de Interface Externa;**

(D) três Entradas Externas, dois Arquivos Lógicos Internos e um Arquivo de Interface Externa;

❌ **(E) seis Entradas Externas, dois Arquivos Lógicos Internos e um Arquivo de Interface Externa.** ← sua resposta

**Onde você se confundiu:** você acertou o AIE (sublinhou "mantida exclusivamente pelo sistema de Organização Judiciária") e eliminou a (B). Errou em dois pontos:

1. **Especialidade não é ALI separado.** Ela "só existe vinculada a um perito": é um **RLR dentro do ALI Perito** (a classe filha dentro do agregado, como você mesmo lembrou na analogia). Resultado: 1 ALI, não 2.
2. **Seis EE:** você contou Incluir/Alterar/Excluir duas vezes (perito e especialidade). Mas a especialidade "é gravada junto com ele, pelos botões da Tela 1": são os **mesmos 3 processos elementares**. Resultado: 3 EE.

**Pista entre (D) e (E):** as duas erravam no ALI. A frase "só existe vinculada a" é o sinal clássico de RLR.

📌 **Dado que "só existe vinculado a" outro (dependente) é RLR do mesmo ALI, não um ALI novo.** Cada botão Incluir, Alterar ou Excluir = 1 EE. Se a aba é gravada pelos mesmos botões, não gera EE nova.

---

## Questão 3 · ✅ Acertou

A Análise de Pontos de Função mede o tamanho funcional de um software sob a ótica do usuário. No processo de contagem, a transação cujo objetivo principal é apresentar informações ao usuário por meio de uma lógica de processamento que contenha ao menos uma fórmula matemática ou cálculo, ou que crie dados derivados, é classificada como

(A) entrada externa.

(B) consulta externa.

\(C) arquivo de interface externa.

✅ **(D) saída externa.** ← sua resposta

(E) arquivo lógico interno.

Você sublinhou a pista certa: "fórmula matemática ou cálculo". (A) traz dado para dentro; (B) apresenta sem cálculo; (C) e (E) são funções de dados, não transações.

📌 **Apresenta + cálculo/dado derivado = SE. Apresenta sem cálculo = CE.**

---

## Questão 4 · ⬜ Em branco (não sabia: "?")

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

✅ **(A) 108;**

(B) 90;

\(C) 120;

(D) 150;

(E) 102.

**O que faltou:** a fórmula. São só 3 passos:

| Passo | Conta | Resultado |
|---|---|---|
| 1. Somar os 14 níveis (TDI) | 3+1+4+2+3+2+1+0+2+1+0+3+1+2 | **25** |
| 2. Calcular o VAF | 0,65 + 0,01 × 25 | **0,90** |
| 3. Multiplicar pelo PF não ajustado | 120 × 0,90 | **108** |

As outras são as armadilhas: (C) 120 = esquecer o ajuste; (D) 150 = usar 1 + 0,25; (B) 90 = usar 0,75; (E) 102 = 0,85 (soma errada).

📌 **PF ajustado = PF não ajustado × (0,65 + 0,01 × soma das 14 características).** O VAF vai de 0,65 (soma 0) a 1,35 (soma 70). Se a soma for 35, o VAF é 1,00 e nada muda.

---

## Questão 5 · ✅ Acertou

A Secretaria de TI de um Tribunal de Justiça passou a contratar o desenvolvimento de software medido em pontos de função. Sobre a técnica, analise as afirmativas a seguir.

I\. A Análise de Pontos de Função mede o tamanho do software a partir das funcionalidades solicitadas e recebidas pelo usuário.

II. Dois sistemas com as mesmas funcionalidades, um desenvolvido em Java e outro em Python, terão tamanhos diferentes em pontos de função, porque linguagens diferentes exigem quantidades diferentes de linhas de código.

III. O tamanho em pontos de função pode servir de base para estimar esforço e custo, desde que combinado com a produtividade da equipe ou do fornecedor.

Está correto o que se afirma em

(A) I, apenas.

✅ **(B) I e III, apenas.** ← sua resposta

\(C) II, apenas.

(D) II e III, apenas.

(E) I, II e III.

V/F certinho: I (visão do usuário) e III (tamanho × produtividade = esforço) verdadeiras; II falsa, porque APF não depende de linguagem nem de linhas de código.

📌 **APF é independente de tecnologia e mede tamanho, não esforço. Esforço = PF × produtividade.**

---

## Questão 6 · ❌ Errou (com dúvida: pontinho na C)

O Sistema de Diárias (SisDiárias) de um Tribunal de Justiça registra, altera e aprova as solicitações de diárias dos servidores. Para preencher automaticamente o nome, o cargo e a lotação do solicitante, o SisDiárias apenas lê o cadastro de servidores, que é mantido exclusivamente pelo Sistema de Gestão de Pessoas. As duas bases ficam armazenadas no mesmo servidor de banco de dados corporativo do Tribunal.

Na contagem de pontos de função do SisDiárias, o cadastro de servidores e o cadastro de solicitações de diárias devem ser classificados, respectivamente, como:

✅ **(A) Arquivo de Interface Externa e Arquivo Lógico Interno;**

(B) Arquivo Lógico Interno e Arquivo de Interface Externa;

❌ **\(C) Arquivo Lógico Interno e Arquivo Lógico Interno, pois ambos são utilizados pelo SisDiárias;** ← sua resposta

(D) Arquivo de Interface Externa e Arquivo de Interface Externa, pois ambos ficam no banco de dados corporativo;

(E) Entrada Externa e Arquivo Lógico Interno, pois o cadastro de servidores fornece dados de entrada ao SisDiárias.

**Onde você se confundiu:** você marcou as pistas certas ("apenas lê o cadastro", "mantido exclusivamente pelo Sistema de Gestão de Pessoas") e mesmo assim **riscou a (A)**, que era a resposta. Provavelmente pesou o "mesmo servidor de banco de dados corporativo" (que você enquadrou): pareceu que, se está no mesmo banco, é tudo do sistema. Essa frase era a **isca**. A APF olha a **fronteira lógica** (quem mantém), nunca onde o dado fica fisicamente. Na (C), a justificativa "ambos são utilizados" é o erro: usar não é manter.

📌 **ALI × AIE se decide por QUEM MANTÉM, nunca por onde o dado está guardado.** O sistema só lê = AIE, mesmo que esteja no mesmo banco. "Utilizado" ≠ "mantido".

---

## Questão 7 · ✅ Acertou

O sistema GABINETE apoia o trabalho dos magistrados de um Tribunal de Justiça. Por meio de uma primeira funcionalidade, o juiz solicita a lista dos processos conclusos ao seu gabinete, com a quantidade de dias em que cada processo está concluso, calculada pelo sistema a partir da data atual e da data da conclusão. Por meio de uma segunda funcionalidade, o assessor informa o número de um processo e o sistema exibe a classe, o assunto e as partes, exatamente como estão armazenados na base de dados.

Com base na Análise de Pontos de Função (APF), as funcionalidades supracitadas serão contadas, respectivamente, como:

(A) Consulta Externa e Consulta Externa, pois ambas apenas apresentam dados ao usuário;

(B) Entrada Externa e Consulta Externa;

\(C) Consulta Externa e Saída Externa;

✅ **(D) Saída Externa e Consulta Externa;** ← sua resposta

(E) Saída Externa e Saída Externa, pois ambas recuperam dados de Arquivos Lógicos Internos.

Você circulou "calculada" e sublinhou "exatamente como estão armazenados": as duas pistas certas. (A) ignora o cálculo; (C) inverte a ordem; (E) ignora que a segunda não calcula; (B) não há gravação.

📌 **"Quantidade de dias calculada" = dado derivado → SE. "Exatamente como armazenado" → CE. Atenção ao "respectivamente".**

---

## Questão 8 · ❌ Errou

Na contagem de pontos de função do sistema de Mandados de um Tribunal de Justiça, o analista identificou as seguintes estruturas no banco de dados:

I\. tabela de Mandados, mantida pelas funcionalidades de expedição e de registro de cumprimento do próprio sistema;

II. tabela temporária, criada apenas para ordenar o resultado de um relatório e descartada ao final do processamento;

III. índice criado sobre a coluna do número do processo, para acelerar as buscas;

IV. arquivo de backup diário da tabela de Mandados.

Devem ser contados como Arquivo Lógico Interno:

(A) I, II, III e IV.

(B) I e IV, apenas.

✅ **\(C) I, apenas.**

(D) I e II, apenas.

❌ **(E) I, III e IV, apenas.** ← sua resposta

**Onde você se confundiu:** você acertou I (V) e II (F), mas marcou III e IV como verdadeiras. Índice e backup são **estruturas técnicas**: existem por causa da implementação (desempenho e segurança), não porque o usuário pediu um grupo de dados de negócio. O usuário não enxerga um "índice por número de processo" como informação; ele enxerga o **Mandado**. O backup é cópia do mesmo dado, então contá-lo seria contar o Mandado duas vezes.

📌 **Não são ALI: tabela temporária, índice, backup, log técnico e arquivo de ordenação.** Só conta o grupo de dados que o usuário reconhece como negócio (visão do usuário).

---

## Para o caderno de erros

| Assunto | Por que errei | Regra certa |
|---|---|---|
| Funcionalidade que grava (Q1) | "Armazenados na base" me levou a ALI | Funcionalidade = transação. Grava dado vindo de fora = EE. ALI é a tabela, não a ação |
| Tela com aba dependente (Q2) | Contei a especialidade como ALI e dobrei as EE | Dado que "só existe vinculado a" = RLR do mesmo ALI. Mesmos botões = mesmas 3 EE |
| VAF (Q4, em branco) | Não sabia a fórmula | Soma das 14 → VAF = 0,65 + 0,01 × soma → PF ajustado = PF × VAF |
| ALI × AIE (Q6) | "Mesmo banco corporativo" me fez achar que tudo é do sistema | Quem mantém decide. Só lê = AIE, esteja onde estiver |
| Estruturas técnicas (Q8) | Contei índice e backup como ALI | Temporária, índice e backup não contam. Só dado de negócio reconhecido pelo usuário |

---

## O que estudar agora

| Quando | O que fazer |
|---|---|
| Hoje · 22:40 (revisão) | Reler as 5 regras 📌 dos erros. Refazer a Q4 no papel sem olhar (soma → 0,90 → 108) e a Q2 desenhando o agregado Perito com a classe Especialidade dentro |
| Hoje · antes de dormir | Para cada função de dados, perguntar: **o usuário reconhece isso como negócio? quem mantém?** Treinar com 3 sistemas que você conhece (PJe, SEI, sistema do trabalho) |
| Qua 04/11 · 22:40 | Anki: cartões de APF (se você pedir) com foco em ALI × AIE × RLR e no VAF |
| Qua 04/11 · Blocos 1 e 2 | Seguir a semana 2: SAFe ou testes (o plano não fixa o dia). APF volta no sábado ou na revisão, com 5 a 10 questões reais FGV/Cebraspe só de funções de dados. Não decorar tabela DER/RLR |
| Dom 08/11 · 13h | Simulado de domingo |
