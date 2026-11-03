---
tipo: bloco
fonte: autoral
status: pendente
disciplina: ["RLM"]
assunto: "Conjuntos e diagramas de Venn"
semana: 2
data: 2026-11-03
---

# Bloco · RLM · Conjuntos e diagramas de Venn (15 questões)

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

> Assunto único: conjuntos (2 e 3 conjuntos, "no mínimo/no máximo", operações, pertinência × inclusão e conjuntos em Python). Marque "?" no que não souber e nunca deixe em branco.

## Questão 1

Em uma vara cível, foram analisados 60 processos. Sabe-se que:

- 35 processos têm pedido de tutela de urgência;
- 28 processos têm pedido de gratuidade de justiça;
- 12 processos têm os dois pedidos.

O número de processos que têm **somente um** dos dois pedidos é

(A) 9.

(B) 23.

\(C) 39.

(D) 51.

(E) 63.

---

## Questão 2

Dos 80 servidores da Secretaria de TI de um tribunal, sabe-se que:

- 40 fizeram o curso de LGPD;
- 35 fizeram o curso de Segurança da Informação;
- 30 fizeram o curso de Gestão de Riscos;
- 15 fizeram LGPD e Segurança;
- 12 fizeram LGPD e Gestão de Riscos;
- 10 fizeram Segurança e Gestão de Riscos;
- 5 fizeram os três cursos.

O número de servidores que **não fizeram nenhum** dos três cursos é

(A) 7.

(B) 5.

\(C) 12.

(D) 18.

(E) 22.

---

## Questão 3

Uma pesquisa com advogados que atuam no tribunal perguntou quais sistemas eles usam: X, Y e Z. Sabe-se que:

- 20 usam X e Y;
- 15 usam X e Z;
- 18 usam Y e Z;
- 8 usam os três sistemas.

Considere que, nos três primeiros itens, estão incluídos os que usam os três sistemas.

O número de advogados que usam **exatamente dois** desses sistemas é

(A) 8.

(B) 21.

\(C) 37.

(D) 45.

(E) 29.

---

## Questão 4

Em um levantamento com 50 servidores de uma comarca, verificou-se que 36 usam o Microsoft Teams diariamente e 29 usam o e-mail institucional diariamente.

Com base apenas nessas informações, o número **mínimo** e o número **máximo** de servidores que usam diariamente as duas ferramentas são, respectivamente,

(A) 7 e 29.

(B) 15 e 29.

\(C) 15 e 36.

(D) 0 e 29.

(E) 21 e 36.

---

## Questão 5

Um cartório judicial tem 120 processos em andamento. Desses, 70 têm recurso interposto e 45 têm perícia designada.

O número **máximo** de processos que podem não ter recurso interposto nem perícia designada é

(A) 5.

(B) 25.

\(C) 45.

(D) 50.

(E) 75.

---

## Questão 6

Considere os conjuntos:

- A = {1, 2, 3, 4, 5, 6}
- B = {4, 5, 6, 7, 8}
- C = {2, 4, 8, 10}

O conjunto (A − B) ∪ (B ∩ C) é

(A) {1, 2, 3, 4, 8}.

(B) {1, 2, 3}.

\(C) {4, 8}.

(D) {1, 2, 3, 4, 5, 6, 8}.

(E) {7, 8}.

---

## Questão 7

Seja o conjunto universo U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12}. Considere:

- A = conjunto dos múltiplos de 2 em U;
- B = conjunto dos múltiplos de 3 em U.

O número de elementos do complementar de (A ∪ B) em relação a U é

(A) 2.

(B) 8.

\(C) 6.

(D) 10.

(E) 4.

---

## Questão 8

Um sistema processual tem 5 módulos opcionais, que podem ser habilitados ou não para cada unidade judiciária, de forma independente.

O número de configurações diferentes em que **pelo menos um** módulo opcional fica habilitado é

(A) 5.

(B) 10.

\(C) 31.

(D) 32.

(E) 25.

---

## Questão 9

Considere o conjunto A = {1, 2, {3}}.

Assinale a afirmativa **correta**.

(A) 3 ∈ A.

(B) {3} ∈ A.

\(C) {3} ⊂ A.

(D) {1, 3} ⊂ A.

(E) ∅ ∈ A.

---

## Questão 10

Um analista usou conjuntos em Python para comparar os conciliadores cadastrados em duas varas.

```python
vara_civel    = {"Ana", "Bia", "Caio", "Davi"}
vara_criminal = {"Caio", "Davi", "Edu"}

x = vara_civel ^ vara_criminal
y = vara_civel - vara_criminal

print(len(x), len(y), len(x - y))
```

A saída exibida pelo programa é

(A) 2 2 1

(B) 5 3 2

\(C) 3 2 0

(D) 3 2 1

(E) 1 2 3

---

## Questão 11

Os números de três listas de processos foram guardados em conjuntos Python.

```python
a = {1, 2, 3, 4, 5}
b = {4, 5, 6, 7}
c = {1, 5, 7, 8}

todos = a & b & c
so_a  = a - (b | c)
uniao = a | b | c

print(len(todos), len(so_a), len(uniao))
```

A saída exibida pelo programa é

(A) 1 3 8

(B) 1 2 8

\(C) 2 2 8

(D) 1 2 13

(E) 0 2 8

---

## Questão 12

Em um setor com 45 servidores, todos usam pelo menos um dos sistemas A ou B. Sabe-se que:

- o número de servidores que usam **somente** A é o dobro do número dos que usam **somente** B;
- 9 servidores usam os dois sistemas.

O número de servidores que usam o sistema A é

(A) 12.

(B) 24.

\(C) 21.

(D) 36.

(E) 33.

---

## Questão 13

Em um treinamento sobre teoria dos conjuntos, foram apresentadas as afirmativas a seguir, sendo A e B conjuntos quaisquer de um mesmo universo e n(X) o número de elementos de um conjunto finito X.

Assinale a afirmativa **INCORRETA**.

(A) A − B = B − A, para quaisquer conjuntos A e B.

(B) O complementar de (A ∪ B) é igual à interseção dos complementares de A e de B.

\(C) A ∩ ∅ = ∅.

(D) Se A ⊂ B, então A ∪ B = B.

(E) n(A ∪ B) = n(A) + n(B) − n(A ∩ B), para A e B finitos.

---

## Questão 14

Uma pesquisa de satisfação com os usuários de um tribunal mostrou que:

- 60% usam o Balcão Virtual;
- 45% usam o atendimento presencial;
- 20% não usam nenhum dos dois.

O percentual de usuários que usam **apenas um** desses dois canais é

(A) 25%.

(B) 35%.

\(C) 55%.

(D) 80%.

(E) 15%.

---

## Questão 15

Em um tribunal com 100 servidores, sabe-se que 80 usam o Teams, 70 usam o SEI e 60 usam o PJe.

O número **mínimo** de servidores que usam as três ferramentas é

(A) 0.

(B) 30.

\(C) 60.

(D) 10.

(E) 50.

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
