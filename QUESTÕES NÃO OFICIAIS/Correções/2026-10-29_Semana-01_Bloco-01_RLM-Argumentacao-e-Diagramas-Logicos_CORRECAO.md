---
tipo: correcao
fonte: autoral
disciplina: ["RLM"]
assunto: "Argumentação lógica e diagramas lógicos (15 questões)"
semana: 1
data: 2026-10-29
acertos: 9
total: 15
---

# Correção · RLM · Argumentação lógica e diagramas lógicos · 15 questões

**Data:** 29/10/2026 · **Semana 1** · **Placar: 9/15 (60%)** · 4 erros · 2 em branco

**Respostas lidas das anotações do PDF:** 1-B · 2-C · 3-E · 4-E · 5-A · 6-B · 7-D · 8-A · 9-em branco (?) · 10-C · 11-C · 12-A · 13-D · 14-D · 15-em branco (?)

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

> **Como este bloco foi feito:** começou como diagnóstico (você disse que não sabia o assunto), virou treino depois da teoria e dos 11 exemplos resolvidos no chat. **Assistidas:** Q2 e Q11 (eu montei o caminho das setas) e Q6 (eu desempatei entre B e D). **Pontinho = acerto com dúvida:** Q12. **"?" = não sabia:** Q9 e Q15, ambas de conjuntos ("estudar conjuntos, não lembro").

| Questão | Assunto | Sua | Gabarito | Resultado |
|---|---|---|---|---|
| 1 | Silogismo: todo + algum | B | B | ✅ |
| 2 | Silogismo: nenhum + todo (corrente de setas) | C | D | ❌ (assistida) |
| 3 | Afirmar o consequente com "todo" | E | E | ✅ |
| 4 | Validade × verdade (I, II, III) | E | C | ❌ |
| 5 | Modus tollens | A | A | ✅ |
| 6 | Qual argumento é válido | B | B | ✅ (assistida) |
| 7 | Falácia: apelo à popularidade | D | D | ✅ |
| 8 | Falácias: associação | A | A | ✅ |
| 9 | Diagrama de Venn com números | — | C | ⬜ em branco (?) |
| 10 | Silogismo: algum + nenhum | C | E | ❌ |
| 11 | Silogismo com 3 premissas ("não pode ser garantida") | C | C | ✅ (assistida) |
| 12 | Equivalência de "todo" ("não é equivalente") | A | A | ✅ (com dúvida) |
| 13 | Negação de "nenhum" | D | D | ✅ |
| 14 | Silogismo com indivíduo (Ana) | D | B | ❌ |
| 15 | Leitura de código Python: conjuntos | — | E | ⬜ em branco (?) |

**Por tipo:**

| Tipo | Questões | Placar |
|---|---|---|
| Silogismos (todo/algum/nenhum) | 1, 2, 10, 11, 14 | 2/5 (uma assistida) |
| Validade e formas de argumento | 3, 4, 5, 6 | 3/4 (uma assistida) |
| Falácias | 7, 8 | 2/2 |
| Equivalência e negação com quantificador | 12, 13 | 2/2 |
| Conjuntos e Venn | 9, 15 | 0/2 (em branco) |

**Sem as assistidas:** 7 acertos em 12 questões (58%).

**Comparação:** o bloco anterior de RLM (27/10, conectivos e proposições) teve 8/15 (53%). Hoje foram 9/15 (60%) num assunto que, de manhã, você dizia não saber. Falácias e negação/equivalência com quantificador saíram limpas. Os erros vieram de **três escorregões de anotação** (letras parecidas, apóstrofo no lugar errado, contrapositiva sem negar os dois lados) e de **um conceito** (validade × verdade). Conjuntos ficou em branco porque o assunto não foi estudado.

---

## Questão 1 · ✅ Acertou

Sabe-se que:

- Todo juiz do tribunal é bacharel em Direito.
- Algum servidor do tribunal é juiz.

Com base apenas nessas informações, é necessariamente verdadeiro que

(A) todo servidor do tribunal é bacharel em Direito.

✅ **(B) algum servidor do tribunal é bacharel em Direito.** ← sua resposta

\(C) algum bacharel em Direito não é juiz.

(D) todo bacharel em Direito é servidor do tribunal.

(E) nenhum servidor do tribunal que não seja juiz é bacharel em Direito.

Você montou J → D e a ficha S·J, e a seta empurrou D = V. (A), (D) e (E) são "todo/nenhum" sem caminho de setas; (C) pede um bacharel que não é juiz, e o x é juiz.

📌 Ficha do x (S·J) + seta J → D: esquerdo V empurra o direito → o x é S·D → "algum servidor é bacharel".

---

## Questão 2 · ❌ Errou (assistida)

Considere verdadeiras as afirmações a seguir.

- Nenhum processo físico tramita no PJe.
- Todo processo de execução fiscal da comarca tramita no PJe.

Assinale a conclusão que decorre necessariamente dessas afirmações.

(A) Algum processo físico é de execução fiscal.

(B) Todo processo que tramita no PJe é de execução fiscal.

❌ (C) Nenhum processo que tramita no PJe é de execução fiscal. ← sua resposta

✅ **(D) Nenhum processo de execução fiscal da comarca é físico.**

(E) Todo processo que não tramita no PJe é físico.

**Onde se confundiu:** as suas setas estavam **certas**: P_F → J', P_e → J e as contrapositivas J → P_F' e J' → P_e'. O problema foram as **letras parecidas**. Você usou P_F (físico) e P_e (execução), e na hora de comparar a seta **J → P_F'** ("o que está no PJe não é físico") leu como **J → P_e'**, que é a alternativa (C). Ela não tem caminho: no PJe pode haver execução fiscal à vontade.

O caminho certo: **P_e → J → P_F'** (execução fiscal → está no PJe → não é físico) = "nenhum processo de execução fiscal é físico".

📌 **Use letras bem diferentes** (F, J, E), nunca duas letras com o mesmo início. Só "todo/nenhum" nas premissas → resposta pela **corrente de setas**.

---

## Questão 3 · ✅ Acertou

Durante uma conversa no setor de pessoal, um servidor apresentou o seguinte raciocínio:

"Todo analista judiciário é servidor público. Carlos é servidor público. Logo, Carlos é analista judiciário."

Sobre esse argumento, é correto afirmar que

(A) é válido, pois as duas premissas são verdadeiras.

(B) é válido, pois a conclusão decorre da primeira premissa por contraposição.

\(C) é inválido, pois a primeira premissa é falsa.

(D) é válido somente se Carlos tiver sido aprovado em concurso para analista.

✅ **(E) é inválido, pois as premissas permitem que Carlos seja servidor público sem ser analista judiciário.** ← sua resposta

A → S com S = V: o lado direito V não puxa nada (afirmar o consequente). (C) acerta o "inválido" pelo motivo errado (a premissa é verdadeira).

📌 Afirmar o consequente (A → B; B; logo A) é inválido. A alternativa precisa acertar o veredito **e** o motivo.

---

## Questão 4 · ❌ Errou

Em uma capacitação sobre lógica aplicada à redação de decisões, foram feitas as afirmativas a seguir sobre argumentos.

I\. Um argumento válido com todas as premissas verdadeiras tem, necessariamente, conclusão verdadeira.

II. Um argumento cuja conclusão é verdadeira é, necessariamente, válido.

III. Um argumento válido pode ter conclusão falsa, desde que pelo menos uma de suas premissas seja falsa.

Está correto o que se afirma em

(A) I, apenas.

(B) II, apenas.

✅ **(C) I e III, apenas.**

(D) II e III, apenas.

❌ (E) I, II e III. ← sua resposta

**Onde se confundiu:** no item II você anotou "F/V → V" e marcou como verdadeiro. Você testou **uma linha** da seta "premissas → conclusão" e viu que, com a conclusão V, ela nunca dá V → F. Mas validade não é sobre a situação de agora: é sobre a **forma**. Um argumento é inválido se existe **alguma** situação possível com premissas V e conclusão F, mesmo que nesta a conclusão tenha dado V por sorte.

Exemplo: "Todo gato é mamífero. Rex é mamífero. Logo, Rex é gato." Se o Rex for mesmo um gato, a conclusão é V, mas o argumento é **inválido** (afirmar o consequente: o Rex poderia ser um cachorro).

I e III estavam certos na sua anotação (V → V e F → F).

📌 **Conclusão verdadeira não torna o argumento válido. Premissa falsa não o torna inválido.** Válido = em **nenhuma** situação possível as premissas são V e a conclusão F.

---

## Questão 5 · ✅ Acertou

Considere verdadeira a proposição:

"Se o sistema de peticionamento foi atualizado, então o backup noturno foi executado."

Sabe-se, ainda, que o backup noturno **não** foi executado.

Com base nessas informações, conclui-se que

✅ **(A) o sistema de peticionamento não foi atualizado.** ← sua resposta

(B) o sistema de peticionamento foi atualizado.

\(C) o backup noturno será executado na próxima noite.

(D) nada se pode concluir sobre a atualização do sistema de peticionamento.

(E) o sistema de peticionamento foi atualizado, mas o backup falhou.

P → B com B = F: o direito F puxa o esquerdo para F (modus tollens). (D) é a isca de quem acha que "negar sempre dá em nada".

📌 Modus tollens: A → B; não B; logo não A. (F puxa para trás.)

---

## Questão 6 · ✅ Acertou (assistida)

Assinale a opção que apresenta um argumento **válido**.

(A) Se o juiz deferir a liminar, o réu será intimado. O réu foi intimado. Logo, o juiz deferiu a liminar.

✅ **(B) O recurso foi protocolado no prazo ou foi declarado intempestivo. O recurso não foi declarado intempestivo. Logo, o recurso foi protocolado no prazo.** ← sua resposta

\(C) Se a audiência for presencial, haverá sala reservada. A audiência não foi presencial. Logo, não houve sala reservada.

(D) Alguns servidores são analistas. Alguns analistas são programadores. Logo, alguns servidores são programadores.

(E) O sistema estava lento ou a rede estava instável. O sistema estava lento. Logo, a rede não estava instável.

Você resolveu a (B) sozinho (P + D, com D = F, obriga P = V) e ficou na dúvida com a (D), porque multiplicou S·A · A·P. Duas premissas com "algum" são **duas pessoas**: não se multiplicam. (A) afirma o consequente, (C) nega o antecedente, (E) usa "ou" simples, que aceita os dois V.

📌 **Duas premissas com "algum" = x e y separados: nada se conclui. Toda ligação passa por uma seta.**

---

## Questão 7 · ✅ Acertou

Em uma reunião de planejamento, um gestor defendeu:

"Devemos adotar esse framework no tribunal. Afinal, a maioria dos tribunais do país já o utiliza."

O raciocínio do gestor contém a falácia conhecida como

(A) ataque à pessoa (*ad hominem*).

(B) generalização apressada.

\(C) falsa causa (*post hoc*).

✅ **(D) apelo à popularidade (*ad populum*).** ← sua resposta

(E) falso dilema.

O argumento é "a maioria usa". Não ataca pessoa (A), não parte de poucos casos (B), não fala de causa (C) nem reduz a duas opções (E).

📌 Ad populum = "todo mundo faz / a maioria usa" como prova.

---

## Questão 8 · ✅ Acertou

Considere os argumentos a seguir, ouvidos nos corredores de um fórum.

1. "Desde que o novo servidor entrou na equipe, o sistema caiu duas vezes. Logo, ele é o responsável pelas quedas."
2. "Conversei com três advogados que reclamaram do PJe. Portanto, todos os advogados reprovam o sistema."
3. "Ou migramos todo o acervo para a nuvem ainda este mês, ou o tribunal ficará sem sistema."

Associe cada falácia ao argumento correspondente.

( ) Falso dilema

( ) Falsa causa (*post hoc*)

( ) Generalização apressada

A sequência correta, de cima para baixo, é

✅ **(A) 3 – 1 – 2.** ← sua resposta

(B) 1 – 3 – 2.

\(C) 2 – 1 – 3.

(D) 3 – 2 – 1.

(E) 1 – 2 – 3.

Você marcou 3 e 2 e eliminou pelas alternativas que sobravam, uma boa economia de tempo.

📌 Falso dilema = só duas opções · Falsa causa = veio depois, logo foi causado por · Generalização = poucos casos → todos.

---

## Questão 9 · ⬜ Em branco (não sabia: "estudar conjuntos, não lembro")

A Diretoria de TI de um tribunal tem 40 servidores. Sabe-se que:

- 25 fizeram o curso de Java;
- 18 fizeram o curso de Python;
- 7 não fizeram nenhum dos dois cursos.

O número de servidores que fizeram os dois cursos é

(A) 3.

(B) 7.

✅ **(C) 10.**

(D) 11.

(E) 15.

**Como resolver:**

1. Fizeram **pelo menos um** curso: 40 − 7 = **33**.
2. Java + Python conta duas vezes quem fez os dois: 25 + 18 = 43.
3. A sobra é a interseção: 43 − 33 = **10**.

Conferindo: só Java = 25 − 10 = 15 · só Python = 18 − 10 = 8 · 15 + 10 + 8 + 7 = 40 ✔

A (A) = 3 é a isca de quem esquece os 7 que não fizeram nada (25 + 18 − 40).

📌 **Total − nenhum = A + B − ambos.** Comece pelo centro (ambos) e confira somando todas as regiões.

---

## Questão 10 · ❌ Errou

Considere verdadeiras as premissas:

- Algum conciliador do CEJUSC é advogado.
- Nenhum advogado é servidor efetivo do tribunal.

Assinale a conclusão que decorre necessariamente dessas premissas.

(A) Nenhum conciliador do CEJUSC é servidor efetivo do tribunal.

(B) Todo advogado é conciliador do CEJUSC.

❌ (C) Algum servidor efetivo do tribunal é conciliador do CEJUSC. ← sua resposta

(D) Algum advogado não é conciliador do CEJUSC.

✅ **(E) Algum conciliador do CEJUSC não é servidor efetivo do tribunal.**

**Onde se confundiu:** a montagem estava perfeita: ficha C·A (V, V) e seta A → S', com **S' = V**. O tropeço foi na leitura do valor. "S' = V" quer dizer que o servidor é **F** (o x **não** é servidor). Ao comparar com as alternativas, você provavelmente leu como "servidor = V", e por isso a (C) (S·C) pareceu caber e a (E) (C·S') foi riscada. O pontinho na (C) mostra que você desconfiou.

Ficha correta do x: **C = V · A = V · S = F** → "algum conciliador **não** é servidor" ✔

📌 **Ao anotar a ficha, escreva sempre o valor da letra positiva:** S = F, nunca S' = V. Assim a comparação com a alternativa fica direta.

---

## Questão 11 · ✅ Acertou (assistida)

Considere verdadeiras as afirmações:

- Todos os oficiais de justiça são servidores.
- Nenhum servidor é estagiário.
- Alguns estagiários são estudantes de Direito.

Assinale a conclusão que **não** pode ser garantida a partir dessas afirmações.

(A) Nenhum oficial de justiça é estagiário.

(B) Alguns estudantes de Direito não são servidores.

✅ **(C) Nenhum estudante de Direito é oficial de justiça.** ← sua resposta

(D) Alguns estudantes de Direito são estagiários.

(E) Alguns estudantes de Direito não são oficiais de justiça.

Você anotou "E e O não têm ligação": D só aparece no "algum", então não sai nenhuma seta de D. (A) tem caminho O → S → E'; (B), (D) e (E) cabem na ficha do x (E, D, S = F, O = F).

📌 **"Algum" se testa no x; "todo/nenhum" se testa no caminho de setas.** Letra que só aparece no "algum" não tem seta saindo dela.

---

## Questão 12 · ✅ Acertou (com dúvida)

Considere a afirmação:

"Todo processo sigiloso tem acesso restrito."

Assinale a opção que **não** é logicamente equivalente a essa afirmação.

✅ **(A) Todo processo de acesso restrito é sigiloso.** ← sua resposta

(B) Se um processo é sigiloso, então ele tem acesso restrito.

\(C) Nenhum processo sigiloso deixa de ter acesso restrito.

(D) Todo processo que não tem acesso restrito não é sigiloso.

(E) Não existe processo sigiloso sem acesso restrito.

Você montou S → R e a contrapositiva R' → S', e a (A) ficou R → S: a recíproca. As outras quatro dizem a mesma coisa (proíbem S·R').

📌 **Contrapositiva vale (B' → A'); recíproca não (B → A).** O "todo" não inverte.

---

## Questão 13 · ✅ Acertou

Sabe-se que é **falsa** a afirmação:

"Nenhum recurso julgado pela 1ª Câmara Cível foi provido."

Com base nisso, é necessariamente verdadeiro que

(A) todos os recursos julgados pela 1ª Câmara Cível foram providos.

(B) nenhum recurso julgado pela 1ª Câmara Cível foi desprovido.

\(C) algum recurso julgado pela 1ª Câmara Cível não foi provido.

✅ **(D) pelo menos um recurso julgado pela 1ª Câmara Cível foi provido.** ← sua resposta

(E) a maioria dos recursos julgados pela 1ª Câmara Cível foi provida.

Você chegou em R = V e P = V (existe um recurso provido) e marcou "maioria" e "todos" como extrapolação. Muito bem.

📌 Negação de "nenhum A é B" = "algum (pelo menos um) A é B". Nunca "todo" nem "a maioria".

---

## Questão 14 · ❌ Errou

Considere verdadeiras as premissas:

- Toda pessoa lotada na Diretoria de TI tem acesso ao data center.
- Nenhum estagiário tem acesso ao data center.
- Ana é estagiária.

Conclui-se, corretamente, que

(A) Ana não é servidora do tribunal.

✅ **(B) Ana não é lotada na Diretoria de TI.**

\(C) Ana é lotada na Diretoria de TI, mas não tem acesso ao data center.

❌ (D) toda pessoa sem acesso ao data center é estagiária. ← sua resposta

(E) nada se pode concluir sobre a lotação de Ana.

**Onde se confundiu (dois pontos, ambos na anotação):**

1. **Contrapositiva sem negar os dois lados.** Você escreveu L → D e, ao lado, **D' → L**. O certo é **D' → L'**. Com a sua versão, a Ana (estagiária → sem acesso → "lotada") parecia lotada na TI, e a (B), que é a certa, foi riscada.
2. **A (D) é a recíproca.** "Nenhum estagiário tem acesso" = E → D'. A (D) diz D' → E ("todo sem acesso é estagiário"), a seta virada **sem negar**. Pode haver um servidor de outro setor sem acesso ao data center.

Caminho certo para a Ana: **E = V** → (E → D') **D = F** → (L → D, F puxa para trás) **L = F** → "Ana não é lotada na TI".

📌 **Contrapositiva: vira a seta E nega os dois lados (L → D = D' → L').** Virar sem negar é a recíproca, e não vale.

---

## Questão 15 · ⬜ Em branco (não sabia: "estudar conjuntos")

Um analista usou conjuntos em Python para montar, em código, o diagrama de Venn dos cursos feitos pela equipe.

```python
java   = {"Ana", "Bruno", "Carla", "Davi", "Elisa"}
python = {"Carla", "Davi", "Fabio", "Gil"}

ambos    = java & python
so_java  = java - python
qualquer = java | python

print(len(ambos), len(so_java), len(qualquer))
```

A saída exibida pelo programa é

(A) 2 3 9

(B) 2 5 7

\(C) 7 3 2

(D) 3 2 7

✅ **(E) 2 3 7**

**Como resolver** (você já tinha contado 5 e 4 na margem):

| Operação | Significa | Resultado | `len` |
|---|---|---|---|
| `java & python` | está nos dois (interseção) | {Carla, Davi} | **2** |
| `java - python` | está em java e não em python | {Ana, Bruno, Elisa} | **3** |
| `java \| python` | está em pelo menos um, sem repetir (união) | 5 + 4 − 2 | **7** |

A (A) = 9 é a isca de quem soma 5 + 4 sem tirar os repetidos (conjunto não guarda duplicata).

📌 **Python: `&` = interseção · `|` = união sem repetir · `-` = só o primeiro · `^` = só um dos dois.** len(A | B) = len(A) + len(B) − len(A & B).

---

## Para o caderno de erros

| Assunto | Por que errei | Regra certa |
|---|---|---|
| Silogismo só com todo/nenhum (Q2) | Usei P_F e P_e e troquei uma pela outra ao comparar | Letras bem diferentes (F, J, E). Corrente: E → J → F' = "nenhum E é F" |
| Validade × verdade (Q4) | Testei uma linha da seta e achei que conclusão V garante validade | Válido = nenhuma situação possível com premissas V e conclusão F. Conclusão V por sorte não prova nada |
| Silogismo algum + nenhum (Q10) | Anotei "S' = V" e li como "servidor = V" | Anotar o valor da letra positiva (S = F). Algum C é A + nenhum A é S → algum C não é S |
| Contrapositiva e recíproca (Q14) | Escrevi D' → L (sem negar o L) e aceitei a recíproca D' → E | A → B = B' → A' (nega os dois). B → A não vale |
| Conjuntos / Venn (Q9 e Q15, em branco) | Assunto não estudado | Total − nenhum = A + B − ambos. Python: &, \|, -, ^ |

---

## O que estudar agora

| Quando | O que fazer |
|---|---|
| Hoje · 19h–20h50 | Estimativa ágil (Planning Poker, story points, T-shirt) + bloco só desse assunto |
| Hoje · 22:40 (revisão) | **Criar os cartões de 28/10 no Anki** (adiado do início da sessão) e os de hoje (setas, x, contrapositiva × recíproca, validade, conjuntos). Reler as regras 📌 da Q2, Q4, Q10 e Q14. Refazer Q10 e Q14 sem olhar, escrevendo a ficha com valor da letra positiva |
| Sex 30/10 · almoço | Português Módulo 0 A2 (verbo, advérbio, locuções adverbiais) |
| Sáb 31/10 | RLM conjuntos (Venn com 2 e 3 conjuntos, "no mínimo/no máximo") + revisão da semana, se você pedir o bloco misto |
| Dom 01/11 · 13h | 1º simulado oficial (TJ-MS 2024 ou TJ-AP 2024). Nas questões de silogismo: letras diferentes, "algum" com ponto, "nenhum" com o não só no segundo |
