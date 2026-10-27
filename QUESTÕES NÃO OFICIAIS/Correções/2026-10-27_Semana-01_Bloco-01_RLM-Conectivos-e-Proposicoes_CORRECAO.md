---
tipo: correcao
fonte: autoral
disciplina: ["RLM"]
assunto: "Conectivos lógicos e proposições (15 questões)"
semana: 1
data: 2026-10-27
acertos: 8
total: 15
---

# Correção · RLM · Conectivos lógicos e proposições · 15 questões

**Data:** 27/10/2026 · **Semana 1** · **Placar: 8/15 (53%)** · 7 erros · 0 em branco
**Respostas lidas das anotações do PDF (confirmadas no chat):** 1-C · 2-B · 3-E · 4-A · 5-C · 6-B · 7-A · 8-C · 9-B · 10-D · 11-D · 12-C · 13-D · 14-B · 15-C

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

> **Observação:** as questões 3, 4 e 5 foram explicadas durante o estudo, antes da resposta final, e contam como **acertos assistidos**. Nas questões 8 e 11 vale a **primeira resposta**, dada antes da explicação.

| Questão | Assunto | Sua | Gabarito | Resultado |
|---|---|---|---|---|
| 1 | O que é proposição | C | D | ❌ |
| 2 | Quando a condicional é falsa | B | B | ✅ |
| 3 | Negação do "e" (De Morgan) | E | E | ✅ (assistido) |
| 4 | Negação do "se… então" | A | A | ✅ (assistido) |
| 5 | Equivalência: contrapositiva | C | C | ✅ (assistido) |
| 6 | Nº de linhas da tabela-verdade | B | D | ❌ |
| 7 | Valor lógico (p, q, r dados) | A | C | ❌ |
| 8 | Tautologia | C | E | ❌ |
| 9 | Bicondicional (dedução) | B | B | ✅ |
| 10 | Ou exclusivo + condicional | D | A | ❌ (atenção) |
| 11 | Cadeia de condicionais | D | E | ❌ (atenção) |
| 12 | Validade de argumentos | C | C | ✅ |
| 13 | Negação de "todo" | D | D | ✅ |
| 14 | Leitura de código (Python) | B | B | ✅ |
| 15 | Condicional falsa (dedução) | C | A | ❌ |

**Por bloco:** Conceito e tabela 1/3 · Negação e equivalência 4/4 · Valor lógico e tautologia 0/2 · Dedução 3/6 · Código 1/1

**Comparação:** é o primeiro bloco só de RLM. Em 21/10 você errou o silogismo do "se… então" por negar o antecedente. Hoje acertou a Q12, que cobra exatamente isso, e acertou todas as negações e equivalências. **Evolução clara.** Os erros novos são de dois tipos: **pressa na marcação** (Q10 e Q11: o raciocínio estava certo e a letra marcada estava errada) e **detalhes de tabela** (Q1, Q6, Q7 e Q8).

---

## Questão 1 · ❌ Errou

Assinale a opção que apresenta uma proposição lógica.

(A) Que horas começa a audiência de conciliação?

(B) Protocole a petição até as 18h.

❌ (C) Esta frase é falsa. ← sua resposta

✅ **(D) O Tribunal de Justiça da Paraíba tem sede em João Pessoa.**

(E) x + 3 = 10.

**Onde você se confundiu:** você anotou "ideia de estado" na (C). Ela parece uma afirmação, mas é um **paradoxo**: se for verdadeira, então é falsa; se for falsa, então é verdadeira. Ela não consegue ter **um** valor lógico, então não é proposição. A (D) é declarativa e tem um valor definido (V).

- **(A):** pergunta.
- **(B):** ordem.
- **(E):** sentença aberta. O valor depende de x, então não é V nem F por si só.

📌 **Proposição = frase declarativa com um único valor, V ou F.** Não são proposição: pergunta, ordem, exclamação, sentença aberta (com variável) e paradoxo ("esta frase é falsa").

---

## Questão 2 · ✅ Acertou

Considere a proposição: "Se o processo foi distribuído, então o relator foi sorteado."

Essa proposição é falsa quando

(A) o processo não foi distribuído e o relator foi sorteado.

✅ **(B) o processo foi distribuído e o relator não foi sorteado.** ← sua resposta

\(C) o processo não foi distribuído e o relator não foi sorteado.

(D) o processo foi distribuído e o relator foi sorteado.

(E) o relator foi sorteado, independentemente da distribuição.

Você anotou "V F = F", que é exatamente a regra. Nas alternativas (A) e (C) o antecedente é F, e a condicional fica V. A (D) é V → V = V.

📌 **A → B só é falsa em V → F.** Em Boole: A → B = A' + B.

---

## Questão 3 · ✅ Acertou (assistido)

Considere a afirmação: "O servidor entregou o relatório e o sistema foi atualizado."

A negação lógica dessa afirmação é:

(A) O servidor não entregou o relatório e o sistema não foi atualizado.

(B) Se o servidor entregou o relatório, então o sistema foi atualizado.

\(C) O servidor entregou o relatório ou o sistema não foi atualizado.

(D) O servidor não entregou o relatório e o sistema foi atualizado.

✅ **(E) O servidor não entregou o relatório ou o sistema não foi atualizado.** ← sua resposta

Resolvida juntos com bits: ~(1100 · 1010) = ~1000 = 0111, e só a (E) dá 0111. A (A) é a pegadinha: nega as partes e mantém o "e" (dá 0001).

📌 **De Morgan: (A · B)' = A' + B'.** Nega as partes **e troca o conectivo**.

---

## Questão 4 · ✅ Acertou (assistido)

Considere a afirmação: "Se o juiz despachar o processo hoje, então a secretaria publicará a decisão amanhã."

A negação lógica dessa afirmação é:

✅ **(A) O juiz despachará o processo hoje e a secretaria não publicará a decisão amanhã.** ← sua resposta

(B) Se o juiz não despachar o processo hoje, então a secretaria não publicará a decisão amanhã.

\(C) Se a secretaria não publicar a decisão amanhã, então o juiz não terá despachado o processo hoje.

(D) O juiz não despachará o processo hoje ou a secretaria publicará a decisão amanhã.

(E) O juiz não despachará o processo hoje e a secretaria publicará a decisão amanhã.

(d' + p)' = d · p'. As alternativas (C) e (D) são **equivalentes** à frase, não a negação dela. A (B) é a inversa e a (E) nega a parte errada.

📌 **~(A → B) = A ∧ ~B** ("quem o segurança barra": fez A e não fez B).

---

## Questão 5 · ✅ Acertou (assistido)

Considere a regra de contingência de um tribunal: "Se o sistema PJe está fora do ar, então o protocolo é feito no balcão."

Uma afirmação logicamente equivalente a essa regra é:

(A) Se o protocolo é feito no balcão, então o sistema PJe está fora do ar.

(B) Se o sistema PJe não está fora do ar, então o protocolo não é feito no balcão.

✅ **(C) Se o protocolo não é feito no balcão, então o sistema PJe não está fora do ar.** ← sua resposta

(D) O sistema PJe está fora do ar e o protocolo é feito no balcão.

(E) O sistema PJe está fora do ar ou o protocolo é feito no balcão.

Sua anotação estava perfeita: S = ~a ∨ b e (C) = b ∨ ~a. A (A) é a recíproca, a (B) é a inversa e a (E) não tem o "não" no a.

📌 **A → B ⇔ ~B → ~A ⇔ ~A ∨ B.** Recíproca (B → A) e inversa (~A → ~B) nunca são equivalentes.

---

## Questão 6 · ❌ Errou

Uma regra de negócio de um sistema do tribunal foi formalizada pela proposição composta

[(P ∧ Q) ∨ R] → [(S ↔ ~T) ∨ P]

em que P, Q, R, S e T são proposições simples.

O número de linhas da tabela-verdade dessa proposição é

(A) 10.

❌ (B) 16. ← sua resposta

\(C) 25.

✅ **(D) 32.**

(E) 64.

**Onde você se confundiu:** você anotou "2⁴". A fórmula 2ⁿ estava certa, mas a contagem de n não. As proposições simples **diferentes** são cinco: P, Q, R, S e T. Então 2⁵ = 32. Provavelmente você descontou o T por causa do "~" (ou o P repetido duas vezes). Mas **~T não é uma proposição nova**, e o T continua sendo uma variável. O P repetido conta **uma vez** só.

- **(E) 64:** pegadinha de quem conta o P duas vezes (2⁶).
- **(A) 10 e (C) 25:** contas sem sentido (2 × 5 e 5²).

📌 **Linhas = 2ⁿ, com n = proposições simples diferentes.** Letra repetida conta uma vez; letra negada (~T) também conta.

---

## Questão 7 · ❌ Errou

Sabe-se que a proposição p é verdadeira e que as proposições q e r são falsas. Considere as proposições compostas a seguir.

I\. (p ∧ q) → r

II. (p ∨ q) → r

III. ~p ↔ (q ∨ r)

É verdadeiro o que se afirma em

❌ (A) I, apenas. ← sua resposta

(B) II, apenas.

✅ **(C) I e III, apenas.**

(D) II e III, apenas.

(E) I, II e III.

**Onde você se confundiu:** I e II estavam certos nas suas anotações (I = V, II = F). O erro foi no **III**, que você avaliou como F:

```
~p      = F
q ∨ r   = F ∨ F = F
F ↔ F   = V   ← os dois lados iguais
```

O ↔ é verdadeiro quando os lados são **iguais**, inclusive F e F. Você aprendeu isso na Q9 (que acertou), mas aqui o F ↔ F pareceu "falso".

- **I:** (V ∧ F) → F = F → F = V.
- **II:** (V ∨ F) → F = V → F = F.

📌 **↔ = XNOR: V quando iguais.** F ↔ F = **V**. Em código: `a == b`.

---

## Questão 8 · ❌ Errou

Uma proposição composta é uma tautologia quando é verdadeira para todas as combinações de valores lógicos de suas proposições simples.

Assinale a opção que apresenta uma tautologia.

(A) (p ∨ q) → p

(B) p ∧ ~p

❌ (C) (p → q) → (q → p) ← sua resposta (primeira)

(D) p ↔ q

✅ **(E) p → (p ∨ q)**

**Onde você se confundiu:** você marcou por eliminação. Converteu a (C) corretamente, (p·q') + (q' + p), mas não simplificou nem testou. Ela vira **p + q'**, que dá 0 com p = 0 e q = 1. Na (E): p' + p + q = 1 + q = **1** sempre. Depois da explicação você circulou "A' + A = V", que é o pulo do gato.

- **(A):** dá p + q', que é 0 com p = 0 e q = 1.
- **(B):** contradição (sempre F). Você eliminou certo.
- **(D):** dá F quando os lados são diferentes.

📌 **Tautologia aparece quando a simplificação chega em x + x' (= 1).** A recíproca (A → B) → (B → A) **não** é tautologia. Antes de marcar, teste um caso com números.

---

## Questão 9 · ✅ Acertou

Considere verdadeira a afirmação: "O recurso é admitido se, e somente se, o preparo foi recolhido no prazo."

Sabe-se que o recurso não foi admitido. Logo,

(A) o preparo foi recolhido no prazo.

✅ **(B) o preparo não foi recolhido no prazo.** ← sua resposta

\(C) nada se pode concluir sobre o preparo.

(D) o preparo foi recolhido, mas fora do prazo.

(E) o recurso pode ter sido inadmitido mesmo com o preparo recolhido no prazo.

Sua conta em Boole estava certa: S = ab + a'b', com a = F e S = V, dá b = F. Você também eliminou a (D) corretamente, porque ela extrapola: "não recolhido no prazo" não garante "recolhido fora do prazo".

📌 **"Considere verdadeira" = S = V.** Na ↔, um lado F obriga o outro a ser F.

---

## Questão 10 · ❌ Errou (atenção)

Considere verdadeiras as afirmações:

- "Ou Ana é analista, ou Bruno é técnico, mas não ambos."
- "Se Bruno é técnico, então Carla é juíza."

Sabe-se que Carla não é juíza. Logo,

✅ **(A) Ana é analista e Bruno não é técnico.**

(B) Ana não é analista e Bruno é técnico.

\(C) Ana é analista e Bruno é técnico.

❌ (D) Ana não é analista e Bruno não é técnico. ← sua resposta

(E) Bruno é técnico e Carla é juíza.

**Onde você se confundiu:** suas anotações estão **certas**: Ana = V e Bruno = F. Mesmo assim, o círculo foi para a (D), que diz "Ana **não** é analista". É o mesmo erro de atenção da Q11: o raciocínio estava certo, a marcação não. O caminho:

```
Carla = F
Bruno → Carla = V  →  Bruno' + F = V  →  Bruno = F
Ana ⊕ Bruno = V   →  Ana ⊕ F = V      →  Ana = V
```

Na (D), Ana e Bruno são F ao mesmo tempo, o que **viola o "ou… ou"**: com os dois F, a primeira afirmação fica falsa.

📌 **"Ou… ou" (XOR) verdadeiro: um lado é o oposto do outro.** E antes de marcar, **releia a alternativa e confira com o que você deduziu**.

---

## Questão 11 · ❌ Errou (atenção)

Considere verdadeiras as premissas a seguir.

- P1: Se o sistema migrar para a nuvem, a equipe será treinada.
- P2: Se a equipe for treinada, o cronograma será prorrogado.
- P3: O cronograma não foi prorrogado.

A partir dessas premissas, conclui-se corretamente que

(A) o sistema migrou para a nuvem e a equipe não foi treinada.

(B) a equipe foi treinada, mas o sistema não migrou para a nuvem.

\(C) o sistema não migrou para a nuvem, mas a equipe foi treinada.

❌ (D) nada se pode concluir, pois nenhuma premissa afirma um fato positivo. ← sua resposta (primeira)

✅ **(E) o sistema não migrou para a nuvem e a equipe não foi treinada.**

**Onde você se confundiu:** segundo você mesmo, foi pressa na leitura. A (D) apresenta um motivo "técnico" que não existe: **fato negativo também é fato**. O caminho é c = F → t = F → m = F, voltando negando a cadeia (modus tollens duas vezes).

📌 **Fato negativo também é fato.** Na cadeia de condicionais, comece pelo fato solto e volte negando: em `x' + y = V`, se y = F, então x = F.

---

## Questão 12 · ✅ Acertou

Assinale a opção que apresenta um argumento válido.

(A) Se chove, a sessão é virtual. Não choveu. Logo, a sessão não foi virtual.

(B) Se chove, a sessão é virtual. A sessão foi virtual. Logo, choveu.

✅ **(C) Chove ou a sessão é presencial. Não choveu. Logo, a sessão é presencial.** ← sua resposta

(D) Chove ou a sessão é presencial. Choveu. Logo, a sessão não é presencial.

(E) Se chove, a sessão é virtual. Logo, se a sessão é virtual, choveu.

No "ou", se um lado é F, o outro tem que ser V.

- **(A):** nega o antecedente. **Foi o seu erro de 21/10, e hoje você não caiu.**
- **(B):** afirma o consequente.
- **(D):** o "ou" inclusivo aceita os dois juntos.
- **(E):** é a recíproca.

📌 **Só há dois caminhos válidos na condicional:** ir pela seta (A, logo B) ou voltar negando (não B, logo não A).

---

## Questão 13 · ✅ Acertou

Considere a afirmação: "Todos os servidores do setor de TI concluíram o curso de LGPD."

A negação lógica dessa afirmação é:

(A) Nenhum servidor do setor de TI concluiu o curso de LGPD.

(B) Todos os servidores do setor de TI não concluíram o curso de LGPD.

\(C) Algum servidor que concluiu o curso de LGPD não é do setor de TI.

✅ **(D) Pelo menos um servidor do setor de TI não concluiu o curso de LGPD.** ← sua resposta

(E) Algum servidor do setor de TI concluiu o curso de LGPD.

Você chegou sozinho, só com as dicas: o "todo" é um "e" gigante, e (s1 · s2 · s3)' = s1' + s2' + s3'. As alternativas (A) e (B) exigem demais ("nenhum"), a (C) muda o grupo e a (E) não desmente.

📌 **~(Todo A é B) = Algum A não é B.** Nunca "nenhum".

---

## Questão 14 · ✅ Acertou

Um analista revisa o trecho de código Python a seguir, usado para classificar processos em uma fila de triagem.

```python
processo_urgente = False
prazo_vencido = True
tem_advogado = False

if not (processo_urgente or prazo_vencido) or tem_advogado:
    print("A")
elif processo_urgente != prazo_vencido:
    print("B")
else:
    print("C")
```

Ao executar o trecho, será impresso:

(A) A

✅ **(B) B** ← sua resposta

\(C) C

(D) A e, em seguida, B

(E) Nada é impresso.

No `if`: not (F or T) or F = F. No `elif`: F != T = True, porque `!=` entre booleanos é XOR. `if/elif/else` executa um bloco só.

📌 **`not (a or b)` nega o resultado inteiro** (De Morgan). E `!=` entre booleanos = XOR.

---

## Questão 15 · ❌ Errou

Sabe-se que é **falsa** a afirmação: "Se Pedro é juiz, então Rita é promotora ou Sílvia é advogada."

Com base nessa informação, é verdadeira a afirmação:

✅ **(A) Pedro é juiz e Sílvia não é advogada.**

(B) Pedro não é juiz ou Rita é promotora.

❌ (C) Rita é promotora ou Sílvia é advogada. ← sua resposta

(D) Se Pedro é juiz, então Sílvia é advogada.

(E) Pedro é juiz se, e somente se, Rita é promotora.

**Onde você se confundiu:** suas anotações estavam certas: Pedro = V e consequente = F. Mas a (C) é **copiada do consequente**, que é justamente a parte falsa. Com p = V, r = F e s = F:

| Alt. | Conta | Valor |
|---|---|---|
| (A) p · s' | V · V | **V** ✅ |
| (B) p' + r | F + F | F |
| \(C) r + s | F + F | F |
| (D) p' + s | F + F | F |
| (E) p ↔ r | V ↔ F | F |

A (A) não fala da Rita, e não precisa: basta que tudo o que ela afirma seja verdadeiro.

📌 **Condicional falsa → antecedente V e consequente F.** Se o consequente é um "ou", **todas** as partes são F. Depois, teste cada alternativa com os valores. Não escolha pelo texto.

---

## Para o caderno de erros

| Assunto | Por que errei | Regra certa |
|---|---|---|
| Proposição (Q1) | Achei que "esta frase é falsa" afirmava algo | Proposição tem um único valor V ou F. Paradoxo, pergunta, ordem e sentença aberta não são |
| Tabela-verdade (Q6) | Contei 4 variáveis (2⁴) | n = proposições simples diferentes: P, Q, R, S, T = 5 → 32. ~T conta, repetida conta 1 vez |
| Bicondicional (Q7) | Avaliei F ↔ F como F | ↔ é V quando os lados são iguais: F ↔ F = V |
| Tautologia (Q8) | Marquei por eliminação, sem simplificar | Procurar x + x' (= 1). Testar um caso antes de marcar |
| XOR (Q10) | Deduzi certo e marquei a letra errada | Releio a alternativa e confiro com o que deduzi |
| Cadeia (Q11) | Pressa: aceitei "fato negativo não conclui" | Fato negativo é fato. Voltar negando a cadeia |
| Condicional falsa (Q15) | Copiei o consequente | Antecedente V, consequente F. Testar as alternativas com os valores |

---

## O que estudar agora

| Quando | O que fazer |
|---|---|
| **Hoje · 22:40 (revisão)** | Reler as 7 regras 📌 dos erros acima. Refazer Q6, Q7 e Q15 sem olhar a correção |
| **Qua 28/10 · revisão** | Revisão espaçada de 7 dias das regras de 21/10 (lógica e argumentação). Refazer Q8 e Q10 |
| **Qui 29/10 · almoço** | RLM: 10 questões FGV de equivalências e negações (QConcursos/TEC, filtro FGV · RLM · 2022+). Usar o método de Boole: frase → letras → A' + B → simplificar → comparar |
| **Sáb 31/10 · almoço** | RLM: argumentação e diagramas lógicos (todo/algum/nenhum), próximo item da prioridade 1 |
| **Dom 01/11 · simulado** | Em toda questão de lógica, antes de marcar, **releia a alternativa e confira com o que deduziu** |
