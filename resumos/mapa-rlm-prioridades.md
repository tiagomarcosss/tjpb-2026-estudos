# Mapa de RLM · Prioridades de estudo (TJPB 2026 · FGV · Analista de TI)

**Criado em:** 26/10/2026 · **Peso na prova:** 10 questões (10%) · **Meta:** 8 acertos

> A ordem de prioridade é uma **recomendação**, não estatística oficial: não existe ranking público de incidência da FGV em RLM para tribunais de TI. Critérios usados: (1) núcleo que a FGV mais cobra segundo cursinhos; (2) pontos fracos do `contexto-tjpb.md`; (3) custo-benefício. Para confirmar com dados: QConcursos/TEC, filtro **FGV · RLM · Analista · 2022+**.

---

## 1. Conteúdo oficial (edital, Anexo II, área de TI)

1. Conjuntos numéricos · 2. Razões e proporções · 3. Regra de três simples e composta · 4. Porcentagem · 5. Juros simples e compostos · 6. Equações, inequações e sistemas de equações · 7. Funções · 8. Sequências · 9. Matrizes e determinantes · 10. Probabilidade · 11. Análise combinatória · 12. Estatística descritiva · 13. Proposições lógicas · 14. Conectivos · 15. Tabelas-verdade · 16. Equivalências e negações · 17. Argumentação lógica · 18. Diagramas lógicos · 19. Resolução de problemas envolvendo raciocínio lógico-matemático.

Fonte: [Edital TJPB 2026 – FGV, p. 34](https://conhecimento.fgv.br/sites/default/files/concursos/edital-tjpb_19.10-versao-final.pdf)

---

## 2. Ordem de prioridade

### 🔴 Prioridade 1 · Muito alta (núcleo FGV + pontos fracos)

| # | Assunto | Item | Por quê |
|---|---|---|---|
| 1 | Lógica proposicional: proposições, conectivos, tabela-verdade, **equivalências e negações** | 13–16 | Núcleo FGV; errei "se… então" em 21/10 |
| 2 | Argumentação lógica e diagramas lógicos (todo/algum/nenhum, silogismos, validade, falácias) | 17, 18 | Ponto fraco nº 3 |
| 3 | Porcentagem, razões e proporções, regra de três (divisão proporcional) | 2, 3, 4 | Ponto fraco nº 6; base da matemática |
| 4 | Problemas de raciocínio: associação, verdades/mentiras, ordenação/filas, mesas circulares, casa dos pombos | 19 | 30 das 56 questões da Aula 04; filas = ponto fraco nº 8 |
| 5 | Sequências: periódicas, numéricas/recorrência, calendário | 8 | 17 das 56 questões da Aula 04; técnica fixa |

### 🟠 Prioridade 2 · Alta

| # | Assunto | Item | Observação |
|---|---|---|---|
| 6 | Análise combinatória (PFC, permutação, arranjo, combinação) | 11 | Antes de probabilidade |
| 7 | Probabilidade | 10 | Depende da combinatória |
| 8 | Equações, inequações e sistemas | 6 | Ferramenta para os problemas da P1 |
| 9 | Conjuntos (numéricos e operações, "no mínimo") | 1 | Rápido |

### 🟢 Prioridade 3 · Média

| # | Assunto | Item | Observação |
|---|---|---|---|
| 10 | Estatística descritiva (média, mediana, moda, desvio-padrão) | 12 | Ajuda também em BI |
| 11 | Juros simples e compostos | 5 | Fórmula direta |
| 12 | Funções (1º e 2º grau) | 7 | Só o básico |
| 13 | Matrizes e determinantes | 9 | Operações básicas e determinante 2×2/3×3 |

### Ordem prática (almoço, RLM em dias alternados)

| Ciclo | Assuntos | Meta |
|---|---|---|
| 1º | 1 → 2 → 3 | Fechar os 3 pontos fracos |
| 2º | 4 → 5 | Usar a Aula 04 (56 questões com gabarito) |
| 3º | 6 → 7 → 8 → 9 | Combinatória e probabilidade em sequência |
| 4º | 10 → 13 | Básico + revisão dos ciclos 1 e 2 |

---

## 3. Aula 04 · Problemas de Raciocínio (56 questões FGV)

Arquivo: `PROVAS OFICIAIS (estudo)/2026-10-26_FGV-RLM_Aula04-Problemas-de-Raciocinio_56-questoes.pdf` (questões oficiais FGV compiladas; gabarito na última página).

| # | Assunto | Questões | Qtd | Técnica-chave |
|---|---|---|---|---|
| 1 | Sequências periódicas (letras/algarismos) | 9, 10, 11, 12, 13, 43, 51 | 7 | Ciclo → resto da divisão. Resto 0 = último item do ciclo |
| 2 | Calendário (dia da semana) | 26, 28, 29, 33, 49, 53 | 6 | Dias passados mod 7 (contar dias passados, não datas) |
| 3 | Horas e intervalos | 27, 30, 31, 32, 45, 55 | 6 | Tudo em minutos; linha do tempo com a hora marcada = 0 |
| 4 | Ordenação e filas | 16, 18, 20, 21, 25, 48 | 6 | Desenhar e reescrever a cada passo. Entre A e B = posB − posA − 1 |
| 5 | Casa dos pombos / pior caso | 37, 38, 40, 41, 42, 54 | 6 | Pior caso + 1. n objetos em k caixas → alguma tem ≥ ⌈n/k⌉ |
| 6 | Verdades e mentiras | 2, 34, 35, 36, 46 | 5 | Supor cada uma verdadeira e buscar contradição. "Todos erraram" = negar cada frase |
| 7 | Orientação espacial e deslocamentos | 5, 17, 23, 24, 50 | 5 | Eixos (+/−). Para voltar, inverter o vetor resultante |
| 8 | Associação lógica (tabela) | 1, 14, 15, 44 | 4 | Tabela com ✗; sobrando mais de uma opção, testar casos |
| 9 | Sequências numéricas por regra/recorrência | 3, 6, 7, 8 | 4 | Calcular termo a termo; em recorrência, isolar o termo anterior |
| 10 | Disposição circular | 19, 22, 52 | 3 | Fixar uma pessoa; esquerda/direita **de quem está sentado**, olhando o centro |
| 11 | Contagem em códigos (letra + número) | 4, 47 | 2 | Código → número absoluto: (letra − 1) × bloco + número |
| 12 | Conjuntos e "no mínimo/no máximo" | 39, 56 | 2 | Interseção mínima = A + B − Total; caso extremo |

Mistos: Q33 (calendário + soma de PA), Q34 e Q46 (verdade/mentira com calendário).
