---
tipo: bloco
fonte: autoral
status: corrigido
disciplina: ["Engenharia de Software e Ágil"]
assunto: "Estimativa ágil: story points, Planning Poker, T-shirt sizing e velocidade"
semana: 1
data: 2026-10-30
---

# Bloco · Engenharia de Software · Estimativa ágil (15 questões)

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

## Questão 1

Na equipe que mantém o PJe no Tribunal, o Scrum Master informou que as histórias passariam a ser estimadas em **story points**.

Sobre essa unidade de estimativa, é correto afirmar que

(A) corresponde a uma quantidade fixa de horas, definida pela organização para todas as equipes.

(B) mede a produtividade individual de cada desenvolvedor.

\(C) é uma medida relativa do tamanho do item, que considera esforço, complexidade e incerteza em comparação com outros itens.

(D) é calculada após a conclusão da história, com base no tempo efetivamente gasto.

(E) é obrigatória pelo Guia do Scrum para estimar os itens do Product Backlog.

---

## Questão 2

Assinale a descrição correta do **Planning Poker**.

(A) Cada participante escolhe uma carta em segredo e todos a revelam ao mesmo tempo; havendo divergência, os que deram as estimativas extremas explicam seus motivos e faz-se nova rodada, até a convergência.

(B) O Product Owner estima cada item e os Developers votam para aprovar ou rejeitar a estimativa.

\(C) Cada participante anuncia sua estimativa em voz alta, na ordem de senioridade, começando pelo mais experiente.

(D) As cartas são reveladas uma por vez, e a estimativa final é a média aritmética dos valores.

(E) O Scrum Master define a estimativa final quando há divergência entre os participantes.

---

## Questão 3

As cartas usadas pela equipe seguem uma sequência semelhante à de Fibonacci: 1, 2, 3, 5, 8, 13, 20, 40, 100.

A principal razão para usar essa escala, em vez de números consecutivos (1, 2, 3, 4, 5, 6...), é que

(A) facilita a conversão direta de pontos em horas.

(B) permite somar as estimativas com mais precisão matemática.

\(C) obriga a equipe a estimar sempre o maior valor possível.

(D) elimina a necessidade de discussão entre os participantes.

(E) os intervalos crescentes refletem que, quanto maior o item, maior a incerteza, o que evita discussões sobre diferenças pequenas e sem significado, como entre 14 e 15.

---

## Questão 4

Na primeira rodada de Planning Poker da história "consultar andamento processual pelo aplicativo", as cartas reveladas foram:

- Ana: 3
- Bruno: 3
- Carla: 2
- Davi: 13
- Elisa: 3

Conforme a técnica, o próximo passo adequado é

(A) registrar 3 pontos, pois é a estimativa da maioria.

(B) pedir que Carla e Davi expliquem suas estimativas e, após a discussão, fazer nova rodada.

\(C) registrar a média, 4,8 pontos, arredondada para 5.

(D) descartar o voto de Davi, por ser muito diferente dos demais.

(E) registrar 13 pontos, pois deve prevalecer a estimativa mais conservadora.

---

## Questão 5

Nas três últimas sprints, a equipe do sistema de custas judiciais concluiu 21, 18 e 24 pontos. Restam 105 pontos no Product Backlog para a próxima versão.

Usando a velocidade média dessas sprints, a previsão para concluir a versão é de

(A) 3 sprints.

(B) 4 sprints.

\(C) 6 sprints.

(D) 5 sprints.

(E) 7 sprints.

---

## Questão 6

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

\(C) 4.75

(D) 6

(E) 5

---

## Questão 7

Na elaboração do roadmap anual do novo sistema de precatórios, o Product Owner precisa de uma estimativa rápida e grosseira de dezenas de épicos ainda pouco detalhados. A equipe classificou cada épico como PP, P, M, G ou GG.

Sobre essa técnica, é correto afirmar que

(A) trata-se do T-shirt sizing, adequado a estimativas iniciais e de alto nível, pois evita falsa precisão numérica em itens com muita incerteza.

(B) trata-se do Planning Poker, que exige o uso de tamanhos de camiseta no lugar de números.

\(C) trata-se da Análise de Pontos de Função, que mede o tamanho funcional pela visão do usuário.

(D) trata-se do T-shirt sizing, que, por não usar números, impede qualquer conversão posterior para story points.

(E) só pode ser aplicada a histórias prontas para a sprint, que atendam à Definição de Pronto.

---

## Questão 8

O diretor de TI comparou duas equipes: a Equipe A entrega, em média, 40 pontos por sprint; a Equipe B, 20.

Sobre o uso da velocidade, assinale a afirmativa **INCORRETA**.

(A) A velocidade é usada principalmente pela própria equipe, para planejar quanto trabalho cabe nas próximas sprints.

(B) Como cada equipe calibra seus pontos de forma própria, a comparação direta de velocidades entre equipes não é adequada.

\(C) A Equipe A é duas vezes mais produtiva que a Equipe B, pois entrega o dobro de pontos por sprint.

(D) Transformar a velocidade em meta de desempenho tende a gerar inflação das estimativas.

(E) A velocidade tende a se estabilizar após algumas sprints, quando a composição da equipe se mantém.

---

## Questão 9

Numa Sprint Planning, o coordenador da área de negócio pediu que o Product Owner definisse sozinho o tamanho dos itens, para agilizar a reunião.

De acordo com o Guia do Scrum (2020),

(A) o Product Owner é o responsável por dimensionar os itens, pois responde pelo valor do produto.

(B) os Developers que farão o trabalho são os responsáveis pelo dimensionamento; o Product Owner pode influenciá-los, ajudando-os a entender e a escolher trade-offs.

\(C) o Scrum Master dimensiona os itens, para garantir a neutralidade da estimativa.

(D) o uso de story points e de Planning Poker é obrigatório.

(E) o dimensionamento é feito pelos stakeholders durante a Sprint Review.

---

## Questão 10

Durante o Planning Poker da história "emitir certidão de objeto e pé com assinatura digital", um desenvolvedor mostrou a carta **"?"** e outro, a carta **"∞"**.

Em geral, essas cartas significam, respectivamente, que

(A) o participante quer uma pausa; o item já foi concluído.

(B) o item é pequeno demais para estimar; o item tem prioridade máxima.

\(C) o participante concorda com a média; o item deve ir para a próxima sprint.

(D) o participante não tem informação suficiente para estimar; o item é grande demais para ser estimado como está e deve ser dividido.

(E) o item deve ser estimado pelo Product Owner; o item tem esforço zero.

---

## Questão 11

No início do projeto do novo sistema de mandados judiciais, o gerente pediu um prazo exato de entrega. O analista respondeu com base no **Cone da Incerteza**, explicando que

(A) as estimativas iniciais são as mais precisas, pois são feitas antes de surgirem problemas.

(B) a variação das estimativas é maior no início do projeto e diminui à medida que os requisitos e a solução são detalhados.

\(C) a incerteza é constante durante todo o projeto; por isso, as estimativas não devem ser revistas.

(D) a incerteza aumenta ao longo do projeto, porque o escopo sempre cresce.

(E) o cone só se aplica a projetos em cascata, e não ao desenvolvimento ágil.

---

## Questão 12

Sobre a diferença entre estimar em **story points** e em **dias ideais**, é correto afirmar que

(A) o dia ideal representa o tempo de trabalho sem interrupções; já os story points medem o tamanho relativo e não precisam ser alterados quando a equipe fica mais rápida, pois esse ganho aparece no aumento da velocidade.

(B) story points e dias ideais são sinônimos, pois 1 ponto equivale sempre a 1 dia ideal.

\(C) o dia ideal inclui as reuniões, interrupções e e-mails de um dia real de trabalho.

(D) quando a equipe ganha experiência, as histórias já estimadas devem ter seus pontos reduzidos.

(E) story points só podem ser usados por equipes com mais de dez desenvolvedores.

---

## Questão 13

A equipe do sistema de distribuição processual tem 5 desenvolvedores e velocidade média de 30 pontos por sprint. Na próxima sprint, 2 desenvolvedores estarão de férias.

Na Sprint Planning, a conduta mais adequada é

(A) selecionar 30 pontos, pois a velocidade média não deve ser alterada.

(B) selecionar 45 pontos, compensando as férias com horas extras.

\(C) reestimar todas as histórias com valores menores, para que caibam 30 pontos.

(D) cancelar a sprint até o retorno dos desenvolvedores.

(E) considerar a capacidade reduzida e selecionar menos pontos, por exemplo cerca de 18, proporcional aos 3 desenvolvedores disponíveis.

---

## Questão 14

Para estimar novas histórias, a equipe escolheu "consultar processo pelo número CNJ" como história de referência de 2 pontos e uma história mais trabalhosa como referência de 8 pontos. Cada nova história é comparada a essas duas para decidir se é maior, menor ou parecida.

Essa prática

(A) é inadequada, porque estimativas ágeis devem ser absolutas, em horas.

(B) corresponde à Análise de Pontos de Função, que compara funcionalidades com uma tabela de complexidade.

\(C) obriga a equipe a usar exclusivamente dias ideais.

(D) aplica a estimativa relativa por comparação (triangulação), que é a base dos story points.

(E) só é válida se as histórias de referência mudarem de valor a cada sprint.

---

## Questão 15

Analise as afirmativas sobre estimativa ágil.

I\. O Planning Poker é uma variação da técnica Wideband Delphi, que busca o consenso de especialistas a partir de estimativas independentes seguidas de discussão.

II. Para calcular a velocidade, somam-se os pontos de todas as histórias iniciadas na sprint, inclusive as que ficaram parcialmente prontas.

III. Na estimativa por afinidade (affinity estimation), a equipe organiza rapidamente muitos itens em grupos de tamanho parecido, comparando-os entre si, o que é útil para estimar um backlog grande.

Está correto o que se afirma em

(A) I, apenas.

(B) II, apenas.

\(C) I e III, apenas.

(D) II e III, apenas.

(E) I, II e III.

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
| 9 | |
| 10 | |
| 11 | |
| 12 | |
| 13 | |
| 14 | |
| 15 | |
