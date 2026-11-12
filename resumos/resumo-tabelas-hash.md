---
tipo: resumo
disciplina: ["Algoritmos, POO, SOLID e GoF"]
assunto: "Tabelas hash (colisões, fator de carga, remoção, equals/hashCode, chaves em Python, hash × árvore)"
data: 2026-11-11
atualizado: 2026-11-11
---

# Tabelas hash

> 🎯 Pra que serve · 🏛️ Onde é usado · 🤔 Por que é assim · 🔧 Conceitos técnicos · 📌 Regra FGV

## Assunto

| | |
|---|---|
| 🎯 **Pra que serve** | Achar um dado pela chave **calculando** a posição, sem procurar: busca, inserção e remoção em O(1) no caso médio |
| 🏛️ **Onde é usado** | `HashMap`/`HashSet` (Java), `dict`/`set` (Python), caches, índices em memória, detecção de duplicados |
| 🤔 **Por que é assim** | A função de hash espalha as chaves pelo vetor. Como há mais chaves possíveis que posições, colisões são inevitáveis, e o desempenho depende de como elas são tratadas e de quão cheia está a tabela |
| 🔧 **Conceitos técnicos** | Função de hash, colisão, encadeamento separado, endereçamento aberto (sondagem linear, quadrática, hash duplo), fator de carga, rehash, lápide (*tombstone*), contrato `equals`/`hashCode`, chave imutável |

## 1. A ideia

```
h(k) = k mod m      (m = número de posições)
m = 5: h(12) = 2 · h(7) = 2 · h(3) = 3
```

**Colisão** = duas chaves na mesma posição (12 e 7). Sempre acontece; o que muda é **como tratar**.

## 2. Tratamento de colisões

| | **Encadeamento separado** | **Endereçamento aberto** |
|---|---|---|
| Ideia | Cada posição guarda uma **lista** | Tudo no **próprio vetor**; na colisão, procura outra posição livre |
| Variações | Inserir no **fim** ou no **início** da lista (o enunciado diz qual) | **Sondagem linear** (+1, +2...) · quadrática (+1², +2²...) · hash duplo (2ª função) |
| Fator de carga > 1? | **Sim** (as listas crescem) | **Não** (no máximo 1 chave por posição) |
| Remoção | Tira da lista | Precisa de lápide (item 4) |

**Encadeamento** (m = 5, inserir no **fim**, chaves 12, 7, 3, 22, 18):

```
0:
1:
2: 12 → 7 → 22
3: 3 → 18
4:
```

Inserindo no **início**, a posição 2 ficaria 22 → 7 → 12.

**Sondagem linear** (m = 8, h = k mod 8, chaves 9, 17, 10, 25):

| Chave | h(k) | Tentativas | Fica em | Posições examinadas |
|---|---|---|---|---|
| 9 | 1 | 1 livre | 1 | 1 |
| 17 | 1 | 1 ocupada → 2 livre | 2 | 2 |
| 10 | 2 | 2 ocupada → 3 livre | 3 | 2 |
| 25 | 1 | 1, 2, 3 ocupadas → 4 livre | 4 | **4** |

📌 Sondagem linear: **conte a posição inicial** entre as examinadas e **volte ao 0** depois da última posição. Chaves vizinhas se empilham (agrupamento primário).

## 3. Fator de carga e complexidade

**α = n ÷ m** (chaves ÷ posições) = **média de chaves por posição**. Ex.: 900 chaves em 600 posições → α = 1,5 (possível só com encadeamento).

| Situação | Busca |
|---|---|
| Caso **médio** (boa função, α controlado) | **O(1)** |
| **Pior caso** (todas na mesma posição, ex.: função que devolve sempre o mesmo valor) | **O(n)**: vira uma lista só |

Quando α passa de um limite (o `HashMap` do Java usa 0,75), a tabela faz **rehash**: vetor maior e chaves redistribuídas. É o que mantém a busca média em O(1).

📌 **Hash é O(1) só no caso médio; pior caso O(n).** "A tabela hash garante O(1)" é falso.

## 4. Remoção no endereçamento aberto

A busca na sondagem linear **para na primeira posição vazia**. No exemplo do item 2, removendo o 17 (posição 2) e deixando a casa **vazia**:

```
buscar 25: h = 1 → tem 9, não é → posição 2 VAZIA → para: "não existe" ❌
           (o 25 está na posição 4)
```

Solução: marcar como **"removido"** (lápide/*tombstone*). A busca **passa por cima**, e a inserção pode **reaproveitar** a casa.

📌 Endereçamento aberto: **remoção marca "removido", não esvazia**. Senão, as chaves deslocadas para depois dela ficam inalcançáveis.

## 5. Java: `equals` e `hashCode`

`HashSet`/`HashMap`: **1º `hashCode()`** escolhe a posição · **2º `equals()`** compara só dentro dela.

| Contrato | Se quebrar |
|---|---|
| `a.equals(b)` verdadeiro → **mesmo `hashCode()`** | Objetos "iguais" caem em posições diferentes, nunca são comparados, e o Set aceita os dois |
| Mesmo `hashCode()` **não** obriga `equals` verdadeiro | Nada quebra: é só colisão |

📌 **Sobrescreveu `equals`, sobrescreva `hashCode`** com os mesmos campos. O `hashCode` padrão vem do objeto, não do conteúdo.

## 6. Python: chaves de `dict` e `set`

| Pode (imutável, *hashable*) | Não pode (mutável) |
|---|---|
| `int`, `str`, `float`, `bool`, **`tuple`** (de imutáveis), `frozenset` | **`list`**, `dict`, `set` → **`TypeError: unhashable type`** |

📌 Chave precisa ser **imutável** (se mudasse, o hash mudaria e o dado se perderia). Chave composta: **tupla**, não lista.

## 7. Hash × árvore balanceada

| Demanda | Estrutura | Por quê |
|---|---|---|
| Busca por **chave exata**, muitas vezes | **Hash** (`HashMap`, `dict`) | O(1) médio |
| **Ordem**, **faixa** ("entre X e Y"), menor/maior | **Árvore balanceada** (`TreeMap`, AVL, rubro-negra) | O(log n) e chaves ordenadas |

📌 **Hash não tem ordem.** "Listar em ordem" ou "entre duas datas" pede árvore.

## Pegadinhas FGV

| A alternativa diz… | A verdade |
|---|---|
| "garante O(1)" | Só no caso médio; pior caso O(n) |
| "fator de carga = posições livres" | É chaves ÷ posições (média por posição) |
| "com encadeamento, α não passa de 1" | Passa; quem não passa é o endereçamento aberto |
| "basta sobrescrever equals()" | O Set usa o hashCode() **antes** do equals() |
| "a lista de colisões fica ordenada" | Só se a implementação fizer isso; lista simples não é ordenada |
| "remoção: marca como vazio" | Marca como **removido** |
