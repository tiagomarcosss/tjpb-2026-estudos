---
tipo: correcao
fonte: autoral
disciplina: ["Engenharia de Software e Ágil"]
assunto: "Estimativa ágil: story points, Planning Poker, T-shirt sizing e velocidade (15 questões)"
semana: 1
data: 2026-10-30
acertos: 10
total: 15
---

# Correção · Engenharia de Software · Estimativa ágil · 15 questões

**Data:** 30/10/2026 · **Semana 1** · **Placar: 10/15 (67%)** · 4 erros (1 chute) · 1 em branco

**Respostas lidas das anotações do PDF:** 1-C · 2-A · 3-E · 4-B · 5-A · 6-C (chute) · 7-A · 8-D · 9-B · 10-D · 11-em branco (?) · 12-A · 13-E · 14-D · 15-D

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

> **Como li as marcas:** na Q6 você escreveu "chutei" ao lado da (C), então ela conta como "não sabia". Na Q11, o "?" está ao lado do enunciado e nenhuma letra foi marcada (em branco). **Pontinho = acerto com dúvida:** Q1 (pontinho em B, círculo em C) e Q14 (pontinho em B, círculo em D).

| Questão | Assunto | Sua | Gabarito | Resultado |
|---|---|---|---|---|
| 1 | Story points: o que medem | C | C | ✅ (com dúvida) |
| 2 | Planning Poker: procedimento | A | A | ✅ |
| 3 | Por que Fibonacci | E | E | ✅ |
| 4 | Planning Poker: divergência | B | B | ✅ |
| 5 | Velocidade média e previsão | A | D | ❌ (erro de conta) |
| 6 | Leitura de código Python: média das 3 últimas | C (chute) | E | ❌ (chute) |
| 7 | T-shirt sizing | A | A | ✅ |
| 8 | Uso da velocidade ("incorreta") | D | C | ❌ |
| 9 | Guia do Scrum 2020: quem dimensiona | B | B | ✅ |
| 10 | Cartas "?" e "∞" | D | D | ✅ |
| 11 | Cone da Incerteza | — | B | ⬜ em branco (?) |
| 12 | Story points × dias ideais | A | A | ✅ |
| 13 | Capacidade com férias | E | E | ✅ |
| 14 | Estimativa relativa (triangulação) | D | D | ✅ (com dúvida) |
| 15 | Wideband Delphi, velocidade, afinidade (I/II/III) | D | C | ❌ |

**Por tipo:**

| Tipo | Questões | Placar |
|---|---|---|
| Conceito de story points e escalas | 1, 3, 12, 14 | 4/4 (2 com dúvida) |
| Planning Poker e cartas | 2, 4, 10 | 3/3 |
| T-shirt sizing, Scrum, Cone da Incerteza | 7, 9, 11 | 2/3 (Cone em branco) |
| Velocidade: contas e código | 5, 6, 13 | 1/3 |
| Velocidade: uso correto | 8, 15 | 0/2 |

**Comparação:** o bloco anterior de Engenharia de Software (28/10, user stories, INVEST e BDD) teve 13/15 (87%). Hoje foram 10/15 (67%), em assunto estudado só por vídeo, no mesmo dia. O **conceito** de estimativa está firme (Planning Poker e story points: 7 de 7). A queda está toda em **velocidade**: duas contas (uma divisão errada e o `[-3:]` ignorado) e duas regras de uso (comparar equipes e itens parcialmente prontos).

---

## Questão 1 · ✅ Acertou (com dúvida: pontinho em B)

Na equipe que mantém o PJe no Tribunal, o Scrum Master informou que as histórias passariam a ser estimadas em **story points**.

Sobre essa unidade de estimativa, é correto afirmar que

(A) corresponde a uma quantidade fixa de horas, definida pela organização para todas as equipes.

(B) mede a produtividade individual de cada desenvolvedor.

✅ **\(C) é uma medida relativa do tamanho do item, que considera esforço, complexidade e incerteza em comparação com outros itens.** ← sua resposta

(D) é calculada após a conclusão da história, com base no tempo efetivamente gasto.

(E) é obrigatória pelo Guia do Scrum para estimar os itens do Product Backlog.

**Pista para tirar a dúvida da (B):** story points são do **item** (da história), e não da **pessoa**. A equipe estima junta, e o ponto mede o tamanho do trabalho, não quem trabalha mais. (A) e (D) falam em horas; (E) é falsa, porque o Guia do Scrum não prescreve técnica.

📌 **Story point = tamanho RELATIVO do item (esforço + complexidade + incerteza).** Não é hora, não é produtividade individual, não é obrigatório no Scrum.

---

## Questão 2 · ✅ Acertou

Assinale a descrição correta do **Planning Poker**.

✅ **(A) Cada participante escolhe uma carta em segredo e todos a revelam ao mesmo tempo; havendo divergência, os que deram as estimativas extremas explicam seus motivos e faz-se nova rodada, até a convergência.** ← sua resposta

(B) O Product Owner estima cada item e os Developers votam para aprovar ou rejeitar a estimativa.

\(C) Cada participante anuncia sua estimativa em voz alta, na ordem de senioridade, começando pelo mais experiente.

(D) As cartas são reveladas uma por vez, e a estimativa final é a média aritmética dos valores.

(E) O Scrum Master define a estimativa final quando há divergência entre os participantes.

(C) e (D) quebram o segredo da revelação simultânea, que existe para evitar a **ancoragem** (todo mundo copiar o sênior). (B) e (E) tiram a estimativa de quem faz o trabalho.

📌 **Planning Poker: segredo → revelação simultânea (contra ancoragem) → extremos explicam → nova rodada até convergir.** Sem média, sem chefe decidindo.

---

## Questão 3 · ✅ Acertou

As cartas usadas pela equipe seguem uma sequência semelhante à de Fibonacci: 1, 2, 3, 5, 8, 13, 20, 40, 100.

A principal razão para usar essa escala, em vez de números consecutivos (1, 2, 3, 4, 5, 6...), é que

(A) facilita a conversão direta de pontos em horas.

(B) permite somar as estimativas com mais precisão matemática.

\(C) obriga a equipe a estimar sempre o maior valor possível.

(D) elimina a necessidade de discussão entre os participantes.

✅ **(E) os intervalos crescentes refletem que, quanto maior o item, maior a incerteza, o que evita discussões sobre diferenças pequenas e sem significado, como entre 14 e 15.** ← sua resposta

As outras prometem precisão ou conversão em horas, que é justamente o que a escala evita.

📌 **Fibonacci = saltos maiores para itens maiores, porque a incerteza cresce com o tamanho.**

---

## Questão 4 · ✅ Acertou

Na primeira rodada de Planning Poker da história "consultar andamento processual pelo aplicativo", as cartas reveladas foram:

- Ana: 3
- Bruno: 3
- Carla: 2
- Davi: 13
- Elisa: 3

Conforme a técnica, o próximo passo adequado é

(A) registrar 3 pontos, pois é a estimativa da maioria.

✅ **(B) pedir que Carla e Davi expliquem suas estimativas e, após a discussão, fazer nova rodada.** ← sua resposta

\(C) registrar a média, 4,8 pontos, arredondada para 5.

(D) descartar o voto de Davi, por ser muito diferente dos demais.

(E) registrar 13 pontos, pois deve prevalecer a estimativa mais conservadora.

O 13 do Davi pode indicar um risco que ninguém viu (ou um mal-entendido). Por isso quem dá o extremo explica, e não é descartado. Maioria (A), média (C) e "o maior vence" (E) são iscas.

📌 **Divergência no Planning Poker = os extremos (maior e menor) explicam e vota-se de novo.** Nunca maioria, média ou descarte.

---

## Questão 5 · ❌ Errou (erro de conta, não de conceito)

Nas três últimas sprints, a equipe do sistema de custas judiciais concluiu 21, 18 e 24 pontos. Restam 105 pontos no Product Backlog para a próxima versão.

Usando a velocidade média dessas sprints, a previsão para concluir a versão é de

❌ (A) 3 sprints. ← sua resposta

(B) 4 sprints.

\(C) 6 sprints.

✅ **(D) 5 sprints.**

(E) 7 sprints.

**Onde se confundiu (sua conta na margem):** o método estava certo, e a soma também (63). O erro foi na divisão: você escreveu **63 ÷ 3 = 32** (e testou 31 × 3 = 93). O certo é **63 ÷ 3 = 21**. Com 31 ou 32, 105 dá cerca de 3, e você marcou a (A).

Conta certa: (21 + 18 + 24) ÷ 3 = 63 ÷ 3 = **21** → 105 ÷ 21 = **5 sprints**.

**Prova real rápida:** 21 + 18 + 24 têm todos os valores **entre 18 e 24**, então a média **tem de estar entre 18 e 24**. 32 é impossível.

📌 **Previsão = backlog ÷ velocidade média (arredondar para CIMA).** Conferir sempre: a média fica entre o menor e o maior valor.

---

## Questão 6 · ❌ Errou (chute: "chutei")

Um analista do Tribunal escreveu a função abaixo, em Python, para prever quantas sprints faltam para concluir o backlog, usando a média das três últimas sprints.

```python
import math

def sprints_restantes(entregues, backlog):
    ultimas = entregues[-3:]
    media = sum(ultimas) / len(ultimas)
    return math.ceil(backlog / media)

historico = [40, 30, 20, 25, 15]
print(sprints_restantes(historico, 95))
```

O valor exibido pelo programa é

(A) 3

(B) 4

❌ \(C) 4.75 ← sua resposta (chute)

(D) 6

✅ **(E) 5**

**Onde se confundiu (sua conta na margem):** você fez **130 ÷ 5**, ou seja, a média das **cinco** sprints, e não das três últimas. Ignorou o `[-3:]`. (A média das cinco dá 26; você anotou 27, e 95 ÷ 27 ficou perto de 3, que não estava entre as suas opções.) Depois riscou a (B) e chutou a (C). A (C) também cai por outro motivo: `math.ceil` arredonda para cima e devolve inteiro, então "4.75" nunca seria impresso.

**Rastreio linha a linha:**

| Linha | Valor |
|---|---|
| `entregues[-3:]` | os 3 últimos → [20, 25, 15] |
| `sum(ultimas)` | 60 |
| `len(ultimas)` | 3 |
| `media` | 60 / 3 = 20.0 |
| `backlog / media` | 95 / 20 = 4.75 |
| `math.ceil(4.75)` | **5** |

A (B) = 4 é a isca de quem usa as cinco sprints (95 ÷ 26 = 3,65 → ceil = 4).

📌 **Python: `lista[-3:]` = os 3 ÚLTIMOS itens · `lista[:3]` = os 3 primeiros · `math.ceil` = arredonda para CIMA e devolve inteiro.**

---

## Questão 7 · ✅ Acertou

Na elaboração do roadmap anual do novo sistema de precatórios, o Product Owner precisa de uma estimativa rápida e grosseira de dezenas de épicos ainda pouco detalhados. A equipe classificou cada épico como PP, P, M, G ou GG.

Sobre essa técnica, é correto afirmar que

✅ **(A) trata-se do T-shirt sizing, adequado a estimativas iniciais e de alto nível, pois evita falsa precisão numérica em itens com muita incerteza.** ← sua resposta

(B) trata-se do Planning Poker, que exige o uso de tamanhos de camiseta no lugar de números.

\(C) trata-se da Análise de Pontos de Função, que mede o tamanho funcional pela visão do usuário.

(D) trata-se do T-shirt sizing, que, por não usar números, impede qualquer conversão posterior para story points.

(E) só pode ser aplicada a histórias prontas para a sprint, que atendam à Definição de Pronto.

Você riscou as quatro iscas na parte certa. Atenção à (D): o nome está certo, mas a afirmação é falsa, porque os tamanhos podem depois ser mapeados para pontos (ex.: M ≈ 5).

📌 **T-shirt sizing (PP/P/M/G/GG) = estimativa grosseira de épicos e roadmap.** Pode ser convertida depois em pontos.

---

## Questão 8 · ❌ Errou (inverteu o "INCORRETA")

O diretor de TI comparou duas equipes: a Equipe A entrega, em média, 40 pontos por sprint; a Equipe B, 20.

Sobre o uso da velocidade, assinale a afirmativa **INCORRETA**.

(A) A velocidade é usada principalmente pela própria equipe, para planejar quanto trabalho cabe nas próximas sprints.

(B) Como cada equipe calibra seus pontos de forma própria, a comparação direta de velocidades entre equipes não é adequada.

✅ **\(C) A Equipe A é duas vezes mais produtiva que a Equipe B, pois entrega o dobro de pontos por sprint.**

❌ (D) Transformar a velocidade em meta de desempenho tende a gerar inflação das estimativas. ← sua resposta

(E) A velocidade tende a se estabilizar após algumas sprints, quando a composição da equipe se mantém.

**Onde se confundiu:** você **riscou a (C)**, ou seja, percebeu que ela é falsa, e foi por isso mesmo que errou. Numa questão de "INCORRETA", a afirmação falsa **é a resposta**. Riscar a falsa e circular uma verdadeira (D) é o padrão de erro de 23/10 (Q6 e Q8 do DATAPREV), que voltou hoje.

A (C) é falsa porque o ponto de uma equipe não vale o ponto da outra: a Equipe B pode chamar de 3 o que a A chama de 8.

📌 **Velocidade não compara equipes: cada uma tem a sua escala de pontos.** Virar meta gera inflação de pontos.
📌 **"INCORRETA": marque V/F ao lado de cada alternativa e circule a F. Não risque a falsa.**

---

## Questão 9 · ✅ Acertou

Numa Sprint Planning, o coordenador da área de negócio pediu que o Product Owner definisse sozinho o tamanho dos itens, para agilizar a reunião.

De acordo com o Guia do Scrum (2020),

(A) o Product Owner é o responsável por dimensionar os itens, pois responde pelo valor do produto.

✅ **(B) os Developers que farão o trabalho são os responsáveis pelo dimensionamento; o Product Owner pode influenciá-los, ajudando-os a entender e a escolher trade-offs.** ← sua resposta

\(C) o Scrum Master dimensiona os itens, para garantir a neutralidade da estimativa.

(D) o uso de story points e de Planning Poker é obrigatório.

(E) o dimensionamento é feito pelos stakeholders durante a Sprint Review.

É quase a frase literal do Guia (seção do Product Backlog, refinamento). A isca é a (A): o PO **ordena** o backlog, mas não dimensiona.

📌 **Guia do Scrum 2020: quem faz o trabalho dimensiona (Developers). O PO ordena e pode influenciar, explicando trade-offs.** O Guia não obriga story points nem Planning Poker.

---

## Questão 10 · ✅ Acertou

Durante o Planning Poker da história "emitir certidão de objeto e pé com assinatura digital", um desenvolvedor mostrou a carta **"?"** e outro, a carta **"∞"**.

Em geral, essas cartas significam, respectivamente, que

(A) o participante quer uma pausa; o item já foi concluído.

(B) o item é pequeno demais para estimar; o item tem prioridade máxima.

\(C) o participante concorda com a média; o item deve ir para a próxima sprint.

✅ **(D) o participante não tem informação suficiente para estimar; o item é grande demais para ser estimado como está e deve ser dividido.** ← sua resposta

(E) o item deve ser estimado pelo Product Owner; o item tem esforço zero.

A pausa (A) é a carta do **café ☕**. Pequeno demais seria a carta **0** ou **½**.

📌 **Cartas especiais: "?" = falta informação · "∞" = grande demais, dividir · "☕" = pausa · "0" = trivial.**

---

## Questão 11 · ⬜ Em branco (não sabia: "?")

No início do projeto do novo sistema de mandados judiciais, o gerente pediu um prazo exato de entrega. O analista respondeu com base no **Cone da Incerteza**, explicando que

(A) as estimativas iniciais são as mais precisas, pois são feitas antes de surgirem problemas.

✅ **(B) a variação das estimativas é maior no início do projeto e diminui à medida que os requisitos e a solução são detalhados.**

\(C) a incerteza é constante durante todo o projeto; por isso, as estimativas não devem ser revistas.

(D) a incerteza aumenta ao longo do projeto, porque o escopo sempre cresce.

(E) o cone só se aplica a projetos em cascata, e não ao desenvolvimento ágil.

**O que falta estudar (onde está o "?"):** o termo "Cone da Incerteza" (Barry Boehm, popularizado por Steve McConnell). A imagem é um cone deitado: **largo no começo** (a estimativa pode errar para mais ou para menos, até cerca de 4 vezes) e **estreito no fim** (quanto mais se conhece, menor o erro).

```
 início ◀━━━━━━━━━━━━━━━━━━━▶ fim
  ╲ muita incerteza
    ╲─────────────
      ╲──────────  pouca incerteza
```

Mesmo sem conhecer o nome, dava para eliminar pela lógica: quanto mais se sabe sobre o sistema, melhor se estima. Isso elimina (A), (C) e (D). E a (E) é "só se aplica", palavra restritiva que a FGV costuma usar em alternativa errada.

📌 **Cone da Incerteza: a estimativa é muito imprecisa no início e fica mais precisa à medida que o projeto avança.** Por isso o ágil reestima sempre e não promete prazo exato no começo.

---

## Questão 12 · ✅ Acertou

Sobre a diferença entre estimar em **story points** e em **dias ideais**, é correto afirmar que

✅ **(A) o dia ideal representa o tempo de trabalho sem interrupções; já os story points medem o tamanho relativo e não precisam ser alterados quando a equipe fica mais rápida, pois esse ganho aparece no aumento da velocidade.** ← sua resposta

(B) story points e dias ideais são sinônimos, pois 1 ponto equivale sempre a 1 dia ideal.

\(C) o dia ideal inclui as reuniões, interrupções e e-mails de um dia real de trabalho.

(D) quando a equipe ganha experiência, as histórias já estimadas devem ter seus pontos reduzidos.

(E) story points só podem ser usados por equipes com mais de dez desenvolvedores.

Você riscou as quatro iscas. A (D) é a pegadinha mais comum: os pontos ficam como estão, e a equipe mais rápida entrega mais pontos por sprint.

📌 **Dia ideal = sem interrupções. Equipe mais rápida: o ponto não muda, a velocidade sobe.**

---

## Questão 13 · ✅ Acertou

A equipe do sistema de distribuição processual tem 5 desenvolvedores e velocidade média de 30 pontos por sprint. Na próxima sprint, 2 desenvolvedores estarão de férias.

Na Sprint Planning, a conduta mais adequada é

(A) selecionar 30 pontos, pois a velocidade média não deve ser alterada.

(B) selecionar 45 pontos, compensando as férias com horas extras.

\(C) reestimar todas as histórias com valores menores, para que caibam 30 pontos.

(D) cancelar a sprint até o retorno dos desenvolvedores.

✅ **(E) considerar a capacidade reduzida e selecionar menos pontos, por exemplo cerca de 18, proporcional aos 3 desenvolvedores disponíveis.** ← sua resposta

30 × 3/5 = 18. A (C) é a isca perigosa: mexer nos pontos para "caber" destrói a escala.

📌 **Capacidade = velocidade ajustada à disponibilidade (férias, feriados).** Ajusta-se a quantidade de itens, nunca os pontos.

---

## Questão 14 · ✅ Acertou (com dúvida: pontinho em B)

Para estimar novas histórias, a equipe escolheu "consultar processo pelo número CNJ" como história de referência de 2 pontos e uma história mais trabalhosa como referência de 8 pontos. Cada nova história é comparada a essas duas para decidir se é maior, menor ou parecida.

Essa prática

(A) é inadequada, porque estimativas ágeis devem ser absolutas, em horas.

(B) corresponde à Análise de Pontos de Função, que compara funcionalidades com uma tabela de complexidade.

\(C) obriga a equipe a usar exclusivamente dias ideais.

✅ **(D) aplica a estimativa relativa por comparação (triangulação), que é a base dos story points.** ← sua resposta

(E) só é válida se as histórias de referência mudarem de valor a cada sprint.

**Pista para tirar a dúvida da (B):** na APF, cada função (EE, SE, CE, ALI, AIE) é contada e classificada por **tabelas de complexidade padronizadas** (IFPUG), e não comparada com uma história escolhida pela equipe. Comparar com histórias de referência da própria equipe é estimativa **relativa**, ou seja, story points.

📌 **Triangulação = comparar a nova história com 2 referências (uma menor e uma maior).** É estimativa relativa (story points), não APF.

---

## Questão 15 · ❌ Errou

Analise as afirmativas sobre estimativa ágil.

I\. O Planning Poker é uma variação da técnica Wideband Delphi, que busca o consenso de especialistas a partir de estimativas independentes seguidas de discussão.

II. Para calcular a velocidade, somam-se os pontos de todas as histórias iniciadas na sprint, inclusive as que ficaram parcialmente prontas.

III. Na estimativa por afinidade (affinity estimation), a equipe organiza rapidamente muitos itens em grupos de tamanho parecido, comparando-os entre si, o que é útil para estimar um backlog grande.

Está correto o que se afirma em

(A) I, apenas.

(B) II, apenas.

✅ **\(C) I e III, apenas.**

❌ (D) II e III, apenas. ← sua resposta

(E) I, II e III.

**Onde se confundiu (dois pontos):**

1. **Item I:** você riscou a palavra "independentes" e marcou F. Mas a independência é justamente o centro do Delphi e do Planning Poker: cada um estima **sozinho, sem ver o outro** (as cartas em segredo da Q2), e só depois se discute. Você acertou essa ideia na Q2 e não a reconheceu aqui com outro nome.
2. **Item II:** aceitou que histórias parcialmente prontas contam. Não contam: história **não concluída** (fora da Definição de Pronto) **vale zero** na velocidade e volta para o backlog.

📌 **Wideband Delphi → Planning Poker: estimativas INDEPENDENTES (secretas) + discussão + nova rodada.**
📌 **Velocidade só conta pontos de itens CONCLUÍDOS (que atendem à DoD). Parcialmente pronto = 0.**

---

## Para o caderno de erros

| Assunto | Por que errei | Regra certa |
|---|---|---|
| Previsão com velocidade (Q5) | Errei a divisão: 63 ÷ 3 = 32 | 63 ÷ 3 = 21 → 105 ÷ 21 = 5. Média sempre fica entre o menor e o maior valor |
| Leitura de código: fatiamento (Q6, chute) | Ignorei o `[-3:]` e fiz a média das 5 | `[-3:]` = 3 últimos. `math.ceil` = para cima, inteiro |
| Velocidade entre equipes + "INCORRETA" (Q8) | Risquei a falsa (C) e circulei uma verdadeira | Em "INCORRETA", a falsa é a resposta: marcar V/F e circular a F. Velocidade não compara equipes |
| Cone da Incerteza (Q11, em branco) | Não conhecia o termo | Incerteza alta no início, que diminui com o tempo. "Só se aplica" = restritivo, desconfiar |
| Delphi e velocidade (Q15) | Achei que "independentes" estava errado e que item parcial conta | Delphi/Poker = estimativas independentes. Velocidade = só itens prontos (DoD) |

---

## O que estudar agora

| Quando | O que fazer |
|---|---|
| Hoje · 22:40 (revisão) | Reler as regras 📌 da Q5, Q6, Q8, Q11 e Q15. Refazer a Q5 e a Q6 sem olhar, **escrevendo a conta inteira e conferindo se a média está entre o menor e o maior valor** |
| Sáb 31/10 · noite | Criar no Anki os cartões de estimativa ágil (pendente desde 29/10) junto com os de Português A2 |
| Sáb 31/10 · Bloco 2 | RLM conjuntos e Venn (como planejado) |
| Dom 01/11 · 13h | 1º simulado oficial. **Em toda "INCORRETA"/"EXCETO", escrever V/F ao lado de cada letra antes de circular** |
