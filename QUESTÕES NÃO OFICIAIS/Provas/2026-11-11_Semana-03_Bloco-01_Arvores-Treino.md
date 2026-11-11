---
tipo: bloco
fonte: autoral
status: corrigido
disciplina: ["Algoritmos, POO, SOLID e GoF"]
assunto: "Estruturas de dados: árvores · treino pós-diagnóstico (busca, remoção, folhas, recursão + percursos, AVL, degeneração, limites)"
semana: 3
data: 2026-11-11
---

# Bloco · Algoritmos · Árvores · treino (15 questões)

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

> Treino depois do diagnóstico de 10/11 (5/10). Questões 1 a 11: os quatro pontos errados (contar folhas, buscar, remover, recursão em código). Questões 12 a 15: o que você já acertou (percursos, AVL, degeneração, limites). Nas questões, **altura** = número de arestas do caminho mais longo da raiz até uma folha (a raiz está no nível 0). **Desenhe a árvore antes de ler as alternativas.** Marque "?" no que não souber e pontinho nas candidatas. Nunca deixe em branco.

## Questão 1

O sistema e-LOTAÇÃO representa a hierarquia de unidades de uma comarca na árvore a seguir, em que R é a raiz:

```
              R
         /    |    \
        S     T     U
      / | \         |
     V  W  X        Y
        |
        Z
```

O número de folhas, o número de nós internos e o grau da árvore são, respectivamente:

(A) 4, 5 e 3;

(B) 5, 4 e 3;

\(C) 1, 8 e 3;

(D) 5, 4 e 2;

(E) 4, 4 e 3.

---

## Questão 2

O sistema e-MANDADOS guarda os números dos mandados em uma árvore binária de busca, sem balanceamento, montada com a inserção, nesta ordem, das chaves 52, 30, 75, 18, 41, 60, 88, 35, 47 e 44. O analista Murilo localizou a chave 44 utilizando o algoritmo de busca próprio da árvore binária de busca.

A sequência de nós visitados, da raiz até encontrar a chave, é:

(A) 52, 30, 18, 41, 35, 47, 44;

(B) 52, 30, 75, 18, 41, 60, 88, 35, 47, 44;

\(C) 52, 30, 41, 35, 47, 44;

(D) 52, 30, 41, 47, 44;

(E) 18, 30, 35, 41, 44.

---

## Questão 3

No sistema e-PERÍCIAS, uma árvore binária de busca, sem balanceamento, foi montada com a inserção, nesta ordem, das chaves 70, 40, 90, 20, 55, 80, 95, 50 e 60. A analista Lívia buscou a chave 58, que não está na árvore, pelo algoritmo de busca da árvore binária de busca.

O número de nós comparados até a busca concluir que a chave não existe e a posição em que a chave 58 seria inserida são, respectivamente:

(A) 9 nós, pois uma chave ausente obriga a percorrer a árvore inteira;

(B) 3 nós, e a chave seria inserida como filho direito do 55;

\(C) 4 nós, e a chave seria inserida como filho esquerdo do 60;

(D) 4 nós, e a chave seria inserida como filho direito do 60;

(E) 5 nós, e a chave seria inserida como filho esquerdo do 50.

---

## Questão 4

O analista Otávio revisa o método a seguir, do sistema SISPAUTA, escrito em Java, que procura uma chave em uma árvore binária de busca:

```java
No busca(No r, int x) {
    while (r != null && r.chave != x) {
        System.out.print(r.chave + " ");
        if (x < r.chave) r = r.esq;
        else r = r.dir;
    }
    return r;
}
```

O método foi chamado com a raiz da árvore a seguir e x = 36:

```
            25
          /    \
        12      40
       /  \    /  \
      6   18  33   47
         /      \
        15       36
```

Ao final da execução, o método:

(A) imprime 25 40 33 36 e retorna o nó de chave 36;

(B) imprime 25 40 33 e retorna o nó de chave 36;

\(C) imprime 25 12 40 33 e retorna o nó de chave 36;

(D) imprime 25 40 33 e retorna null;

(E) imprime 6 12 15 18 25 33 e retorna o nó de chave 36.

---

## Questão 5

A árvore binária de busca do sistema e-DEPÓSITOS foi montada com a inserção, nesta ordem, das chaves 50, 25, 80, 10, 35, 65, 90, 60, 70 e 62. A analista Sílvia removeu a chave 50, que está na raiz e tem dois filhos, usando o **sucessor em ordem** para ocupar o lugar do nó removido.

Após a remoção, a nova raiz e a nova posição do nó 62 são, respectivamente:

(A) 65, e o 62 passa a ser filho esquerdo do 70;

(B) 80, e o 62 não muda de posição;

\(C) 35, e o 62 não muda de posição;

(D) 62, e o 60 passa a ser filho direito do 65;

(E) 60, e o 62 passa a ser filho esquerdo do 65.

---

## Questão 6

No sistema e-ALVARÁS, a árvore binária de busca foi montada com a inserção, nesta ordem, das chaves 30, 15, 45, 8, 22, 40, 50, 19, 26 e 24. O analista Paulo removeu a chave 30, que está na raiz e tem dois filhos, usando desta vez o **antecessor em ordem** para ocupar o lugar do nó removido.

Após a remoção, a árvore fica assim:

(A) o 26 passa a ser a raiz, e o 24 passa a ser filho direito do 22;

(B) o 22 passa a ser a raiz, e o 26 passa a ser filho direito do 19;

\(C) o 40 passa a ser a raiz, por ser o menor valor da subárvore direita;

(D) o 15 passa a ser a raiz, por ser o filho esquerdo da raiz removida;

(E) o 24 passa a ser a raiz, por ser a última chave inserida na subárvore esquerda.

---

## Questão 7

A árvore binária de busca do sistema e-CARTAS foi montada com a inserção, nesta ordem, das chaves 44, 22, 66, 11, 33, 77 e 88. Em seguida, a analista Joana removeu a chave 77 e, depois, a chave 11.

O percurso em pré-ordem da árvore resultante é:

(A) 44, 22, 11, 33, 66, 88;

(B) 44, 22, 33, 66;

\(C) 44, 22, 33, 66, 88;

(D) 22, 33, 44, 66, 88;

(E) 33, 22, 88, 66, 44.

---

## Questão 8

Em uma revisão técnica do sistema e-INDEX, que usa árvores como índices em memória, a equipe de desenvolvimento de um Tribunal de Justiça analisou as afirmativas a seguir.

I\. Em uma árvore binária de busca, o maior valor está no nó alcançado descendo sempre à direita a partir da raiz, e esse nó pode ter filho esquerdo.

II. Em uma árvore binária de busca, toda folha contém um valor menor que o valor da raiz.

III. Uma árvore com 12 nós tem exatamente 11 arestas, seja ela binária ou n-ária.

Está correto o que se afirma em

(A) I, apenas.

(B) II, apenas.

\(C) III, apenas.

(D) I e III, apenas.

(E) I, II e III.

---

## Questão 9

O analista Rodrigo encontrou o método recursivo a seguir no sistema SISCOR, escrito em Java:

```java
int g(No n) {
    if (n == null) return 0;
    if (n.esq == null && n.dir == null) return 0;
    return 1 + g(n.esq) + g(n.dir);
}
```

O método foi chamado com a raiz da árvore binária a seguir:

```
          30
        /    \
      20      45
     /       /  \
   10      40    50
             \
              42
```

O valor retornado e o que o método calcula são, respectivamente:

(A) 4, o número de nós internos (que não são folhas) da árvore;

(B) 7, o número de nós da árvore;

\(C) 3, o número de folhas da árvore;

(D) 3, a altura da árvore;

(E) 2, o número de nós com dois filhos.

---

## Questão 10

A analista Helena encontrou a função recursiva a seguir no sistema e-JURIS, escrita em Python:

```python
def h(no):
    if no is None:
        return -1
    return 1 + max(h(no.esq), h(no.dir))
```

A função foi chamada com a raiz da árvore binária a seguir:

```
        8
       / \
      3   10
     / \    \
    1   6    14
       / \   /
      4   7 13
```

O valor retornado e o que a função calcula são, respectivamente:

(A) 9, o número de nós da árvore;

(B) 4, a altura da árvore, pois o caminho mais longo tem 4 nós;

\(C) 4, o número de folhas da árvore;

(D) 3, a altura da árvore, contada em arestas;

(E) 2, o nível do nó 6.

---

## Questão 11

O sistema e-SESSÕES mantém os códigos das sessões de julgamento em uma árvore binária de busca, sem balanceamento, montada com a inserção, nesta ordem, das chaves 40, 20, 60, 10, 30, 50, 70, 25 e 65.

O número de folhas e a altura da árvore resultante são, respectivamente:

(A) 2 e 3;

(B) 4 e 4;

\(C) 5 e 3;

(D) 9 e 3;

(E) 4 e 3.

---

## Questão 12

O sistema e-NOTIFICA organiza as categorias de notificação na árvore binária a seguir:

```
          M
        /   \
       F     T
      / \     \
     B   H     W
        /
       G
```

O percurso em pós-ordem dessa árvore é:

(A) M, F, B, H, G, T, W;

(B) B, F, G, H, M, T, W;

\(C) B, G, H, F, W, T, M;

(D) M, F, T, B, H, W, G;

(E) W, T, M, H, G, F, B.

---

## Questão 13

O analista Vinícius verifica se a árvore binária de busca a seguir, do sistema e-AGENDA, atende à condição de uma árvore AVL. Considere que a altura de uma subárvore vazia é −1.

```
         50
        /  \
      30    70
     /  \     \
    20   40    80
                 \
                  90
```

A condição AVL é violada no nó:

(A) 50, pois a subárvore direita tem mais nós que a subárvore esquerda;

(B) 70, pois a diferença entre as alturas de suas subárvores é 2;

\(C) 80, pois ele tem apenas um filho;

(D) 90, pois é a folha mais profunda da árvore;

(E) nenhum, pois toda árvore binária de busca é balanceada.

---

## Questão 14

Na migração do sistema e-ARQUIVO, as chaves 100, 90, 80, 70, 60, 50, 40, 30, 20 e 10 foram inseridas, nessa ordem, em uma árvore binária de busca sem balanceamento. Em seguida, o analista Igor buscou a chave 10.

A altura da árvore e o número de nós comparados na busca são, respectivamente:

(A) 3 e 4, pois a árvore fica balanceada com 10 chaves;

(B) 9 e 10, pois a árvore degenera em uma lista que cresce sempre para a direita;

\(C) 10 e 1, pois o menor valor fica na raiz;

(D) 1 e 10, pois todos os nós ficam no mesmo nível;

(E) 9 e 10, pois a árvore degenera em uma lista que cresce sempre para a esquerda.

---

## Questão 15

A equipe da analista Clara vai armazenar 20 registros do sistema e-CONCILIA em uma árvore binária, com a raiz no nível 0.

A menor e a maior altura possíveis para essa árvore são, respectivamente:

(A) 4 e 19;

(B) 4 e 20;

\(C) 5 e 19;

(D) 3 e 19;

(E) 10 e 19.

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
