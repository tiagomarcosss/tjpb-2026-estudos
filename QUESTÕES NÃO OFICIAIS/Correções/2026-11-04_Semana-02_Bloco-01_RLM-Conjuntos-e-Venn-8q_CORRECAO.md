---
tipo: correcao
fonte: autoral
disciplina: ["RLM"]
assunto: "Conjuntos e diagramas de Venn, sem mínimo e máximo (8 questões)"
semana: 2
data: 2026-11-04
acertos: 4
total: 8
---

# Correção · RLM · Conjuntos e diagramas de Venn · 8 questões

**Data:** 04/11/2026 · **Semana 2** · **Placar: 4/8 (50%)** · 2 erros · 2 "não sabia" ("?")

**Respostas lidas das anotações do PDF:** 1-B · 2-A · 3-D · 4-C · 5-? · 6-B · 7-? · 8-E

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

> **Como li as marcas:** na Q4 há um pontinho ao lado da (C), a circulada (acerto com dúvida), e a conta (3 5 7) − (3 6 9 12) com o 3 riscado. Na Q5 e na Q7 há só um "?" grande, sem letra marcada. Na Q6 você escreveu a legenda J, P, S, JP, JS, PS, JPS ao lado dos dados. Na Q8 você riscou (A), (C) e (D) e circulou (E).

| Questão | Assunto | Sua | Gabarito | Resultado |
|---|---|---|---|---|
| 1 | 2 conjuntos: nenhum | B | B | ✅ |
| 2 | Porcentagem: somente o site | A | D | ❌ |
| 3 | 2 conjuntos com equação: somente X | D | E | ❌ |
| 4 | Operações: (A ∩ B) − C | C | C | ✅ (com dúvida) |
| 5 | Pertinência × inclusão | ? | A | ⬜ não sabia |
| 6 | 3 conjuntos: exatamente uma | B | B | ✅ |
| 7 | Exatamente um, dois e três | ? | A | ⬜ não sabia |
| 8 | Conjuntos em Python | E | E | ✅ |

**Por tipo:**

| Tipo | Questões | Placar |
|---|---|---|
| Venn com números (2 e 3 conjuntos) | 1, 2, 3, 6, 7 | 2/5 |
| Operações e notação (∩, −, ∈, ⊂) | 4, 5 | 1/2 (com dúvida) |
| Conjuntos em Python | 8 | 1/1 |

**Comparação:** primeiro bloco de conjuntos corrigido (o bloco 01 de 03/11 ainda está sem respostas). Em 29/10, conjuntos (Q9) e conjuntos em Python (Q15) ficaram em branco. Hoje você **acertou o Python** e **acertou o Venn de 3 conjuntos sozinho** (em 03/11, o "exatamente dois" foi assistido). Nos dois erros o método estava certo e a execução falhou: na Q2, o meio foi tirado do **círculo errado**; na Q3, as regiões foram montadas certo, mas uma foi **subtraída** em vez de somada.

---

## Questão 1 · ✅ Acertou

Dos 75 servidores de uma comarca, 40 participaram do treinamento sobre o PJe, 30 participaram do treinamento sobre o Balcão Virtual e 12 participaram dos dois treinamentos.

O número de servidores dessa comarca que não participaram de nenhum dos dois treinamentos é

(A) 5.

✅ **(B) 17.** ← sua resposta

(C) 28.

(D) 46.

(E) 58.

**Por quê:** pelo menos um = 40 + 30 − 12 = 58 · nenhum = 75 − 58 = **17**. Iscas: (A) 5 = 75 − 70 (esqueceu de descontar os 12 contados duas vezes) · (C) 28 = somente PJe · (D) 46 = exatamente um (28 + 18) · (E) 58 = pelo menos um.

📌 **Nenhum = total − (A + B − ambos).** A interseção entra duas vezes na soma A + B, por isso é descontada uma vez.

---

## Questão 2 · ❌ Errou

Uma pesquisa com os usuários dos serviços digitais de um tribunal mostrou que:

- 50% usam o aplicativo;
- 45% usam o site;
- 30% não usam nenhum dos dois.

O percentual de usuários que usam **somente o site** é

❌ **(A) 25%.** ← sua resposta

(B) 45%.

(C) 15%.

✅ **(D) 20%.**

(E) 70%.

**Conta certa, em 3 passos:**

| Passo | Conta | Resultado |
|---|---|---|
| 1. Pelo menos um | 100 − 30 | 70% |
| 2. Os dois (meio) | 50 + 45 − 70 | 25% |
| 3. **Somente o site** (lua do site) | 45 − 25 | **20%** |

**Onde você se confundiu (segundo você):** o método estava todo certo, inclusive o meio de 25%. No último passo você tirou o meio do **círculo errado**: fez 50 − 25 = 25%, que é **somente o aplicativo**, quando a pergunta pedia somente o **site** (45 − 25). Foi erro de atenção, não de conteúdo. E a banca sabe disso: 25% está nas alternativas justamente para pegar quem pega o círculo do lado errado (e também quem para no meio, porque o meio também é 25%).

**Como evitar:** antes do último passo, circule no enunciado a palavra que vem depois de "somente" (aqui, **site**) e escreva a conta já com o nome: "só site = 45 − 25". Com o rótulo escrito, fica difícil usar o 50.

📌 **"Somente B" = círculo de B − meio.** No último passo, escreva o nome do conjunto pedido ao lado da conta, para não usar o número do outro círculo.

---

## Questão 3 · ❌ Errou

Um levantamento com 62 advogados que atuam em uma comarca verificou que todos peticionam por pelo menos um dos sistemas X e Y. Sabe-se que:

- o número de advogados que peticionam pelo sistema X é o dobro do número dos que peticionam pelo sistema Y;
- 10 advogados peticionam pelos dois sistemas.

O número de advogados que peticionam **somente** pelo sistema X é

(A) 24.

(B) 48.

\(C) 14.

❌ **(D) 10.** ← sua resposta

✅ **(E) 38.**

**Conta certa:**

| Passo | Conta | Resultado |
|---|---|---|
| 1. Nomear | Y = x · X = 2x (círculos inteiros, com o meio dentro) | — |
| 2. Fórmula da união | 62 = 2x + x − 10 → 3x = 72 | x = 24 · X = 48 |
| 3. **Somente X** | 48 − 10 | **38** |

**Onde você se confundiu (segundo você):** você montou `x − 1 + 10 − 2(2x − 10) = 62`. A ideia de somar as **regiões** do Venn está certa, e esse é um caminho ótimo. O problema está nos **sinais**: as regiões não se descontam, elas **se somam**.

**O seu caminho, consertado (método das regiões):**

| Região | Quanto vale | Por quê |
|---|---|---|
| Somente Y | **x − 10** | Y inteiro (x) menos o meio |
| Meio (os dois) | **10** | dado |
| Somente X | **2x − 10** | X inteiro (2x) menos o meio |

Como todos usam pelo menos um sistema, as três regiões juntas são o total:

**(x − 10) + 10 + (2x − 10) = 62** → 3x − 10 = 62 → 3x = 72 → **x = 24**

E a resposta sai direto da região pedida: somente X = 2x − 10 = 48 − 10 = **38**.

**O que deu errado na sua equação:**

- O "**− 2(2x − 10)**": as regiões do Venn **não se sobrepõem**, então cada uma entra **uma vez e com sinal de mais**. Nada se subtrai aqui. Com o −2(…), a conta vira x − 1 + 10 − 4x + 20 = 62 → −3x = 33 → x negativo. Isso é sinal de que a equação está errada.
- O "**x − 1**": deve ter sido o **x − 10** (somente Y) escrito pela metade.

**A fórmula da união é a mesma coisa, só que pelos círculos inteiros:**

| Método | Equação | Quando usar |
|---|---|---|
| **Regiões** (o seu) | somente Y + meio + somente X = total → (x − 10) + 10 + (2x − 10) = 62 | Quando a pergunta pede um "somente": a resposta já sai pronta |
| **União** | círculo X + círculo Y − meio = total → 2x + x − 10 = 62 | Quando a pergunta pede um círculo inteiro |

As duas dão 3x − 10 = 62. O "− meio" da fórmula da união existe porque, somando os círculos inteiros, o meio é contado duas vezes (uma em X e outra em Y), e você tira uma. No método das regiões, o meio só aparece uma vez, então não se tira nada.

Iscas da questão: (A) 24 = Y inteiro · (B) 48 = X inteiro · \(C) 14 = somente Y · (D) 10 = meio.

📌 **Regiões do Venn se somam, nunca se subtraem: somente Y + meio + somente X (+ nenhum) = total.** Só na fórmula pelos círculos inteiros aparece o "− meio". Se o x der negativo ou quebrado, a equação está errada.

---

## Questão 4 · ✅ Acertou (com dúvida)

Considere os conjuntos:

- A = {2, 3, 5, 7, 11}
- B = {1, 3, 5, 7, 9}
- C = {3, 6, 9, 12}

O conjunto (A ∩ B) − C é

(A) {3, 5, 7}.

(B) {3}.

✅ **\(C) {5, 7}.** ← sua resposta

(D) {2, 11}.

(E) {5, 7, 9}.

**Por quê:** sua anotação está certa. A ∩ B = {3, 5, 7} (o que está nos dois) · tirar o que está em C: só o 3 → **{5, 7}**. Iscas: (A) esqueceu de tirar o C · (B) ficou com o que saiu · (D) é A − B · (E) colocou o 9, que nem está em A. Pode confiar mais: o método que você anotou é exatamente o certo.

📌 **Resolver o parêntese primeiro. A − C = os elementos de A que não estão em C** (o que está só em C, como 6, 9 e 12, é ignorado).

---

## Questão 5 · ⬜ Não sabia ("?")

Considere o conjunto A = {0, {1}, 2} e as afirmativas a seguir.

I\. {1} ∈ A.

II\. 1 ∈ A.

III\. {0, 2} ⊂ A.

IV\. {{1}} ⊂ A.

Está correto o que se afirma em

✅ **(A) I, III e IV, apenas.**

(B) I e II, apenas.

\(C) II e IV, apenas.

(D) III e IV, apenas.

(E) I, II, III e IV.

**O que faltou: a diferença entre ∈ e ⊂.** A tem **três** elementos: `0`, `{1}` e `2`. O `{1}` é um elemento só, como uma caixa com o 1 dentro.

| Símbolo | Compara | Como testar | Em Python (pense em lista) |
|---|---|---|---|
| **∈** (pertence) | **elemento** com conjunto | o objeto aparece **do jeito que está** na lista de A? | `x in A` |
| **⊂** (está contido) | **conjunto** com conjunto | tire as chaves de fora: **cada coisa de dentro** está na lista de A? | `B <= A` (issubset) |

| Item | Teste | Resultado |
|---|---|---|
| I. {1} ∈ A | "{1}" aparece na lista de A? Sim | **V** |
| II. 1 ∈ A | "1" solto aparece na lista? Não, só dentro da caixa {1} | **F** |
| III. {0, 2} ⊂ A | tirando as chaves: 0 está em A? sim · 2 está em A? sim | **V** |
| IV. {{1}} ⊂ A | tirando as chaves de fora sobra {1}: está em A? sim | **V** |

Analogia de dev: A = `[0, [1], 2]`. `[1] in A` → True · `1 in A` → False. O 1 está dentro de uma sublista, não solto na lista.

📌 **∈ liga elemento a conjunto (procure o objeto igualzinho na lista). ⊂ liga conjunto a conjunto (tire as chaves de fora e confira cada item).** Pegadinha FGV: elemento que é conjunto, como {1}.

---

## Questão 6 · ✅ Acertou

A Secretaria de Tecnologia da Informação de um tribunal tem 120 servidores. Um levantamento sobre as linguagens de programação que eles dominam mostrou que:

- 50 dominam Java;
- 45 dominam Python;
- 40 dominam JavaScript;
- 18 dominam Java e Python;
- 15 dominam Java e JavaScript;
- 12 dominam Python e JavaScript;
- 6 dominam as três linguagens.

Nos pares acima, estão incluídos os que dominam as três linguagens.

O número de servidores que dominam **exatamente uma** dessas três linguagens é

(A) 27.

✅ **(B) 63.** ← sua resposta

\(C) 96.

(D) 24.

(E) 135.

**Por quê:** centro = 6 · faixas: JP = 18 − 6 = 12, JS = 15 − 6 = 9, PS = 12 − 6 = 6 · somente J = 50 − 12 − 9 − 6 = 23, somente P = 45 − 12 − 6 − 6 = 21, somente S = 40 − 9 − 6 − 6 = 19 → 23 + 21 + 19 = **63**. Iscas: (A) 27 = exatamente duas · \(C) 96 = pelo menos uma · (D) 24 = nenhuma · (E) 135 = soma simples. A legenda J, P, S, JP… que você escreveu ao lado ajudou: é o mesmo hábito das letras do silogismo.

📌 **De dentro para fora:** centro → faixas (par − centro) → somente (círculo − duas faixas − centro).

---

## Questão 7 · ⬜ Não sabia ("?")

Em uma escola judicial, 80 servidores foram consultados sobre três cursos de capacitação: A, B e C. Sabe-se que:

- 10 servidores fizeram os três cursos;
- 25 servidores fizeram **exatamente dois** cursos;
- 5 servidores não fizeram nenhum dos três cursos.

O número de servidores que fizeram **exatamente um** desses cursos é

✅ **(A) 40.**

(B) 45.

\(C) 50.

(D) 30.

(E) 65.

**O que faltou:** perceber que "exatamente" já separa as pessoas em grupos **que não se repetem**. Cada servidor está em um grupo só:

| Grupo | Quantos |
|---|---|
| Nenhum | 5 |
| Exatamente um | **x** |
| Exatamente dois | 25 |
| Os três | 10 |
| **Total** | **80** |

5 + x + 25 + 10 = 80 → **x = 40**. Aqui **não** se usa a fórmula com pares, porque ninguém foi contado duas vezes. É o contrário da Q6, onde "Java e Python" incluía o centro. Iscas: (B) 45 esqueceu o "nenhum" · \(C) 50 esqueceu os três · (D) 30 tirou os três duas vezes · (E) 65 esqueceu os de exatamente dois.

📌 **"Exatamente um/dois/três" e "nenhum" são fatias separadas: total = nenhum + exat. 1 + exat. 2 + exat. 3.** Já "A e B" (sem o "exatamente") inclui o centro.

---

## Questão 8 · ✅ Acertou

Um analista usou conjuntos em Python para comparar os mediadores cadastrados em duas varas.

```python
civel   = {"Ana", "Bruno", "Carla", "Diego", "Elisa"}
familia = {"Carla", "Diego", "Fernanda", "Gustavo"}

ambos    = civel & familia
so_civel = civel - familia
todos    = civel | familia

print(len(todos), len(ambos), len(so_civel), "Fernanda" in so_civel)
```

A saída exibida pelo programa é

(A) 9 2 3 False

(B) 7 2 3 True

\(C) 7 3 2 False

(D) 7 2 5 False

✅ **(E) 7 2 3 False** ← sua resposta

**Por quê:** todos = 5 + 4 − 2 = 7 · ambos = {Carla, Diego} = 2 · so_civel = {Ana, Bruno, Elisa} = 3 · Fernanda só está em `familia`, então não está em `so_civel` → False. Boa eliminação: riscou (A), que somou 5 + 4 sem descontar, (C) e (D), e desempatou B × E pelo `in`. Em 29/10, conjuntos em Python ficaram em branco.

📌 **`|` união · `&` interseção · `-` diferença · `in` testa pertinência (∈) e devolve True/False.**

---

## Para o caderno de erros

| Assunto | Por que errei | Regra certa |
|---|---|---|
| Venn · "somente" (Q2) | Método certo, mas tirei o meio do círculo errado (50 − 25 = só aplicativo) | Somente B = B − meio. Escrever o nome do conjunto pedido ao lado da última conta |
| Venn com equação (Q3) | Montei as regiões, mas subtraí uma delas: −2(2x − 10) | Regiões se somam: (x − 10) + 10 + (2x − 10) = 62. "− meio" só na fórmula dos círculos inteiros |
| Pertinência × inclusão (Q5) | Não sabia (?) | ∈ = elemento (procure igualzinho na lista) · ⊂ = conjunto (tire as chaves de fora e confira cada item) |
| Exatamente um/dois/três (Q7) | Não sabia (?) | Fatias separadas: total = nenhum + exat. 1 + exat. 2 + exat. 3 |

## O que estudar agora

| Quando | O quê |
|---|---|
| **Almoço (hoje)** | Português B2: verbo e complementos (teoria) |
| **Bloco 1 · 19h** | Próximo assunto da Semana 2: SAFe ou Testes |
| **Bloco 2 · 20h** | Continuação do assunto do Bloco 1 (questões) |
| **Revisão · 22:40** | Reler as 4 regras 📌 dos erros e **refazer Q2, Q3, Q5 e Q7 sem olhar**. Na Q3, escrever a equação inteira no papel. Anki: 4 cartões novos (um por regra) |
| **Domingo 08/11 · 13h** | 1º simulado oficial. Em Venn, perguntar antes de marcar: "pediu o círculo, o meio ou o somente?" |

Mínimo e máximo ficaram **fora de propósito** (decisão sua em 04/11: chance baixa de cair). Se aparecer no simulado, use só a fórmula: meio mínimo = A + B − total · meio máximo = o menor conjunto.
