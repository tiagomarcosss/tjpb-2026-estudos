---
tipo: bloco
fonte: autoral
status: pendente
disciplina: ["Algoritmos, POO, SOLID e GoF"]
assunto: "Estruturas de dados: árvores (terminologia, n-ária, binária, BST, percursos, AVL, heap) (diagnóstico)"
semana: 3
data: 2026-11-10
---

# Bloco · Algoritmos · Árvores (10 questões · diagnóstico)

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

> Prova diagnóstica, feita antes da teoria, para medir o que ficou da faculdade. Assunto único: árvores. Nas questões, **altura** = número de arestas do caminho mais longo da raiz até uma folha (a raiz está no nível 0). Marque "?" no que não souber e pontinho nas candidatas. Nunca deixe em branco.

## Questão 1

O sistema SIGEP-PB organiza a estrutura administrativa do Tribunal na árvore a seguir, em que J é a raiz:

```
              J
           /  |  \
          A   F   M
         / \      |
        B   C     N
                 / \
                P   Q
```

O grau da árvore, a sua altura e o número de folhas são, respectivamente:

(A) 2, 3 e 5;

(B) 3, 4 e 5;

\(C) 3, 3 e 5;

(D) 3, 3 e 4;

(E) 9, 3 e 5.

---

## Questão 2

O analista Rafael inseriu, nesta ordem, as chaves 50, 30, 70, 20, 40, 60, 80 e 35 em uma árvore binária de busca inicialmente vazia, sem nenhum balanceamento, no sistema e-PRAZOS.

O percurso em pré-ordem da árvore resultante é:

(A) 50, 30, 20, 40, 35, 70, 60, 80;

(B) 20, 30, 35, 40, 50, 60, 70, 80;

\(C) 20, 35, 40, 30, 60, 80, 70, 50;

(D) 50, 30, 70, 20, 40, 60, 80, 35;

(E) 50, 70, 80, 60, 30, 40, 35, 20.

---

## Questão 3

O sistema e-CONSULTA mantém os números dos processos de uma vara em uma árvore binária de busca, em que valores menores ficam à esquerda. A analista Tânia precisa gerar um relatório com todos os números em ordem crescente, sem executar nenhum algoritmo de ordenação depois de percorrer a árvore.

Para isso, a analista deve usar o percurso:

(A) em pré-ordem, pois ele visita primeiro a raiz, que contém o menor valor da árvore;

(B) em pós-ordem, pois ele visita primeiro as folhas, que contêm os menores valores;

\(C) em nível (largura), pois ele visita os nós da esquerda para a direita, nível a nível;

(D) em pré-ordem, visitando a subárvore direita antes da subárvore esquerda;

(E) em ordem (in-order), pois ele visita a subárvore esquerda, depois a raiz e depois a subárvore direita.

---

## Questão 4

No sistema e-PROTOCOLO, os números de protocolo são gerados em sequência crescente e inseridos, à medida que chegam, em uma árvore binária de busca simples, sem balanceamento. Após alguns meses, com centenas de milhares de protocolos, o analista Eduardo notou que as buscas ficaram muito lentas.

A explicação correta e uma solução adequada são:

(A) a árvore binária de busca tem busca O(log n) em qualquer caso, e a lentidão deve ter outra causa, como o banco de dados;

(B) as chaves inseridas em ordem crescente degeneram a árvore em uma lista, com busca O(n), e uma árvore AVL manteria a busca em O(log n);

\(C) as chaves inseridas em ordem crescente geram uma árvore completa, com busca O(n log n), e uma heap resolveria o problema;

(D) a árvore degenerou, com busca O(n²), e uma lista ordenada resolveria o problema, com busca O(1);

(E) as chaves inseridas em ordem crescente geram uma árvore cheia, e a troca por uma árvore AVL não alteraria a complexidade da busca.

---

## Questão 5

A analista Patrícia inseriu as chaves 30, 20 e 10, nessa ordem, em uma árvore AVL inicialmente vazia, no módulo de agendamento do sistema e-AUDIÊNCIA. Após a terceira inserção, a árvore ficou desbalanceada.

A operação que restaura o balanceamento e a nova raiz da árvore são, respectivamente:

(A) rotação simples à esquerda e 10;

(B) rotação dupla esquerda-direita e 20;

\(C) nenhuma operação, pois o fator de balanceamento da raiz é 1, e 30;

(D) rotação simples à direita e 20;

(E) rotação simples à esquerda e 20.

---

## Questão 6

A equipe do analista Leonardo vai armazenar os dados de um cadastro do sistema e-PERITOS em uma árvore binária de altura 4 (raiz no nível 0).

O número máximo de nós e o número máximo de folhas que essa árvore pode ter são, respectivamente:

(A) 31 e 16;

(B) 16 e 8;

\(C) 15 e 8;

(D) 32 e 16;

(E) 31 e 15.

---

## Questão 7

A árvore binária de busca do sistema e-CUSTAS foi montada com a inserção, nesta ordem, das chaves 45, 25, 65, 15, 35, 55, 75, 50 e 60. O analista Fernando precisa remover a chave 45, que está na raiz e tem dois filhos, usando o **sucessor em ordem** para ocupar o lugar do nó removido.

Após a remoção, a nova raiz da árvore será:

(A) 35, que é o maior valor da subárvore esquerda;

(B) 65, que é o filho direito da raiz removida;

\(C) 75, que é o maior valor da árvore;

(D) 50, que é o menor valor da subárvore direita;

(E) 25, que é o filho esquerdo da raiz removida.

---

## Questão 8

O sistema e-URGENTE organiza os pedidos de liminar em uma max-heap armazenada em vetor, com índices a partir de 0, em que os filhos do nó de índice i ficam nos índices 2i + 1 e 2i + 2. O vetor atual é:

[90, 70, 80, 40, 50, 60]

A analista Débora inseriu um pedido com prioridade 85, usando o procedimento padrão de inserção em heap.

Após a inserção, o vetor será:

(A) [90, 70, 80, 40, 50, 60, 85];

(B) [85, 90, 80, 40, 50, 60, 70];

\(C) [90, 85, 80, 70, 60, 50, 40];

(D) [90, 85, 80, 40, 50, 60, 70];

(E) [90, 70, 85, 40, 50, 60, 80].

---

## Questão 9

O analista Caio encontrou o método recursivo a seguir no sistema SISDOC, escrito em Java:

```java
int f(No n) {
    if (n == null) return 0;
    if (n.esq == null && n.dir == null) return 1;
    return f(n.esq) + f(n.dir);
}
```

O método foi chamado com a raiz da árvore binária a seguir:

```
            8
          /   \
         4     12
        / \      \
       2   6      14
          /
         5
```

O valor retornado e o que o método calcula são, respectivamente:

(A) 7, o número de nós da árvore;

(B) 3, o número de folhas da árvore;

\(C) 3, a altura da árvore;

(D) 4, o número de nós internos da árvore;

(E) 2, o número de nós com dois filhos.

---

## Questão 10

Em um treinamento sobre estruturas de dados para a equipe de desenvolvimento de um Tribunal de Justiça, foram apresentadas as afirmativas a seguir.

I\. Toda árvore é um grafo conexo e sem ciclos; uma árvore com n nós tem exatamente n − 1 arestas.

II. Em uma árvore binária de busca, o menor valor está sempre armazenado em uma folha.

III. Em uma árvore n-ária, cada nó pode ter mais de dois filhos; a árvore binária é o caso particular em que cada nó tem, no máximo, dois filhos.

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
