---
tipo: correcao
fonte: oficial
banca: FGV
prova: "Simulado 02 (ALE-RO 2026 · Análise e Desenvolvimento de Sistemas)"
disciplina: ["Português", "RLM", "Engenharia de Software e Ágil", "APF, SAFe e Testes", "Arquitetura e System Design", "Banco de Dados e SQL", "Linguagens e Frameworks", "Segurança", "DevOps e Nuvem", "Algoritmos, POO, SOLID e GoF", "Discursiva"]
assunto: "Simulado 02 · 60 objetivas oficiais FGV na estrutura do TJPB + Discursiva 01 · correção comentada e diagnóstico"
semana: 4
data: 2026-11-16
acertos: 30
total: 60
---

# Correção · Simulado 02 · FGV · 60 objetivas (estrutura do TJPB) + Discursiva 01

**Feito em:** 16/11/2026 (segunda) · **Semana 4** · **Placar: 30/60 (50%)** · Português 5/10 · RLM 6/10 · Específicas 19/40 · **Discursiva: 15/40 (estimativa)**

**Meta da objetiva no TJPB:** 36/60 (60%, edital 10.12 com a 1ª retificação). **Faltaram 6 questões.** Discursiva: mínimo de 24/40. **Faltaram 9 pontos.**

> **Questões oficiais da FGV** (Assembleia Legislativa de Rondônia, edital de 2025, prova de 2026, Analista Legislativo · TI · Análise e Desenvolvimento de Sistemas, Tipo 1), renumeradas na estrutura do TJPB e corrigidas pelo gabarito **definitivo**. Nenhuma das 60 foi anulada. **Discursiva: autoral, no estilo FGV, não oficial**, corrigida pelo espelho escrito em 04/11, antes da sua resposta.

> **Como li as marcas (15 fotos):** vale o **cartão de respostas**, que bate com os círculos do caderno nas 60 questões. **Pontinho = candidata/dúvida.** **"?" = não sabia** (acerto com "?" conta como chute, igual a branco). **X = alternativa riscada.** Nas questões 15, 16, 19, 20, 28 e 40 não há círculo no caderno, só o "?": usei a letra do cartão. O horário de início e fim não foi anotado no cartão, então não dá para avaliar o tempo.

---

## 1. Placar

| Parte | Acertos | Só o que você sabia (sem os chutes certos) | Meta TJPB | Simulado 01 (09/11) |
|---|---|---|---|---|
| Português | **5/10** | 5/10 | 8 | 2/10 |
| RLM | **6/10** | 4/10 | 8 | 6/10 |
| Específicas | **19/40** | 17/40 | 33–35 | 19/40 |
| **Total** | **30/60 (50%)** | **26/60 (43%)** | 36 para aprovar | 27/60 (19 sem chutes) |
| Discursiva | **15/40** (estimativa) | | 24 mínimo · 30+ meta | não feita |

**Pela confiança da marcação:**

| Tipo | Quantas | Questões | Simulado 01 |
|---|---|---|---|
| ✅ Acerto firme | **17** | 4, 6, 11, 13, 14, 18, 23, 27, 29, 35, 37, 43, 44, 47, 49, 55, 57 | 5 |
| ✅ Acerto com dúvida (pontinho) | 9 | 8, 9, 10, 21, 22, 24, 52, 54, 60 | 14 |
| ✅ Acerto com "?" (chute, não conta como saber) | 4 | 12, 16, 31, 33 | 8 |
| ❌ Erro com "?" (não sabia) | 16 | 5, 15, 19, 20, 28, 32, 34, 38, 39, 40, 41, 42, 48, 51, 53, 59 | 18 |
| ❌ Erro com pontinho (dúvida) | 7 | 1, 3, 7, 36, 45, 46, 50 | 4 |
| ❌ **Erro convicto** (sem marca de dúvida) | **7** | 2, 17, 25, 26, 30, 56, 58 | 11 |

> **O que melhorou:** os acertos firmes passaram de 5 para 17 e os erros convictos caíram de 11 para 7. O total subiu 3 questões, mas o que você **sabe de verdade** (sem chute) subiu de 19 para 26.

> ⚠️ **O que não melhorou: você riscou a alternativa certa 5 vezes** (Q1, Q5, Q26, Q36 e Q38; eram 4 no Simulado 01). Em nenhuma das 5 há a "prova escrita" ao lado do X, que é o que o protocolo de 12/11 exige. Nessas 5, a resposta certa saiu da disputa antes da hora; com ela ainda entre as candidatas, o placar poderia chegar a 35.

**Pelo que já foi estudado (teoria + bloco corrigido):**

| Situação do assunto | Questões | Acertos | Simulado 01 |
|---|---|---|---|
| **Já estudado** | 5, 8, 13, 21, 22, 23, 24, 25, 26, 29, 30, 49, 60 | **9/13 (69%)** | 5/11 (45%) |
| Ainda não estudado | as outras 47 | 21/47 (45%) | 22/49 (45%) |

> No que você já estudou, o aproveitamento subiu de 45% para 69%. No que ainda não estudou, ficou igual (45%), como era de esperar. **4 erros foram em assunto já estudado: Q25 (validação de requisitos), Q26 (fases do RUP), Q30 (lista encadeada × vetor) e Q5 (coesão: retomada por cognato).** Esses viram prioridade de revisão.

**Pelo edital (Anexo I · Cargo 5 + Fundamentos de TI comuns):** 58 das 60 questões caem no TJPB. **Fora do edital: Q45 (notação IDEF1X) e Q48 (CMMI/MPS.BR)**: só registradas, não estudar. **Placar só do que cai no TJPB: 30/58 (52%).** Duas são limítrofes e contei como "cai": Q56 (comando `systemctl`; o edital do seu cargo traz só "Sistemas operacionais" na parte comum) e Q58 (frameworks de arquitetura corporativa; o edital fala em "padrões de arquitetura corporativa").

**Por área, dentro das Específicas:**

| Área | Questões | Acertos | Observação |
|---|---|---|---|
| Engenharia de requisitos e processos | 21–26, 60 | **5/7** | Estudado. Erros: validação (25) e RUP (26) |
| UML | 27, 28, 57 | 2/3 | Erro: composição (28) |
| Estruturas de dados e GoF | 29, 30, 33 | 2/3 | Erro: lista × vetor (30), já estudado |
| Banco de dados e modelagem | 31, 32, 45, 46, 47 | 2/5 | Assunto das Semanas 4 e 5 (começa agora) |
| **Arquitetura de computadores e fundamentos de programação** | 35–44 | **4/10** | Está como ⚪ na Semana 10 do plano. Foram 10 das 40 questões nesta prova |
| Integração e arquitetura (SOAP, balanceador, arquitetura corporativa) | 34, 58, 59 | 0/3 | Semanas 6 e 7 |
| Segurança, riscos e continuidade | 50–55 | 3/6 | Semana 11 |
| Métricas e maturidade (APF, CMMI) | 48, 49 | 1/2 | APF firme; CMMI fora do edital |
| Sistemas operacionais | 56 | 0/1 | Erro convicto, com a pista no enunciado |

---

## 2. Tabela-resumo

| Q | Assunto | Sua | Gabarito | Resultado | Edital |
|---|---|---|---|---|---|
| 1 | Plural de modéstia ("Fechemos") | A | C | ❌ (com dúvida) · riscou a certa | cai |
| 2 | Finalidade do segmento | D | B | ❌ convicto | cai |
| 3 | Interpretação (INCORRETA) | C | D | ❌ (com dúvida) | cai |
| 4 | Inferência (incredulidade) | A | A | ✅ | cai |
| 5 | Coesão: retomada por cognato | C? | D | ❌ não sabia · riscou a certa | cai |
| 6 | Semântica: fim × finalidade (INADEQUADA) | B | B | ✅ | cai |
| 7 | Parônimos (INDEVIDA) | C | A | ❌ (com dúvida) | cai |
| 8 | Coesão: pronome pessoal × relativo (NÃO) | C | C | ✅ (com dúvida) | cai |
| 9 | Eufemismo | A | A | ✅ (com dúvida) | cai |
| 10 | Problemas de construção da frase | A | A | ✅ (com dúvida) | cai |
| 11 | Porcentagem: lucro total | A | A | ✅ | cai |
| 12 | Posição em fila | B? | B | ✅ chute | cai |
| 13 | Lógica: condicional e contrapositiva | C | C | ✅ | cai |
| 14 | Conversão de unidades (litro → m³) | B | B | ✅ | cai |
| 15 | Probabilidade com permutação | E? | B | ❌ não sabia | cai |
| 16 | Sequência em círculo | D? | D | ✅ chute | cai |
| 17 | Sistema de equações (rodas) | A | C | ❌ convicto | cai |
| 18 | Geometria: perímetro e área | B | B | ✅ | cai |
| 19 | Sistema de equações e razão | C? | E | ❌ não sabia | cai |
| 20 | Função piso (maior inteiro) | E? | A | ❌ não sabia | cai |
| 21 | Requisitos: conflito e negociação | A | A | ✅ (com dúvida) | cai |
| 22 | Requisitos: GORE, FURPS+ e RNF | A | A | ✅ (com dúvida) | cai |
| 23 | Prototipação descartável | B | B | ✅ | cai |
| 24 | Requisitos: análise | D | D | ✅ (com dúvida) | cai |
| 25 | Requisitos: validação | B | C | ❌ convicto · ⚠️ já estudado | cai |
| 26 | RUP: fase de Elaboração | C | D | ❌ convicto · riscou a certa · ⚠️ já estudado | cai |
| 27 | UML: diagrama de sequência | E | E | ✅ | cai |
| 28 | UML: composição | B? | E | ❌ não sabia | cai |
| 29 | Tabela hash | D | D | ✅ | cai |
| 30 | Lista duplamente encadeada × vetor | D | B | ❌ convicto · ⚠️ já estudado | cai |
| 31 | Normalização: 1FN e anomalia | E? | E | ✅ chute | cai |
| 32 | Níveis de modelagem de dados | E? | D | ❌ não sabia | cai |
| 33 | GoF: Singleton | D? | D | ✅ chute | cai |
| 34 | SOAP: WSDL | E? | B | ❌ não sabia | cai |
| 35 | CPU | D | D | ✅ | cai |
| 36 | Gargalo de Von Neumann | E | D | ❌ (com dúvida) · riscou a certa | cai |
| 37 | Dispositivo de saída | C | C | ✅ | cai |
| 38 | Soma binária sem sinal: carry | B? | C | ❌ não sabia · riscou a certa | cai |
| 39 | Complemento de dois: overflow | E? | C | ❌ não sabia | cai |
| 40 | Octal → binário | B? | E | ❌ não sabia (ver observação) | cai |
| 41 | Compilação × interpretação | A? | C | ❌ não sabia | cai |
| 42 | Função × procedimento | E? | D | ❌ não sabia | cai |
| 43 | Passagem por referência | C | C | ✅ | cai |
| 44 | Memória ROM (firmware) | D | D | ✅ | cai |
| 45 | Notação IDEF1X | E | D | ❌ (com dúvida) | **fora** |
| 46 | Integridade referencial | A | B | ❌ (com dúvida) | cai |
| 47 | SQL: INSERT | E | E | ✅ | cai |
| 48 | CMMI / MPS.BR | A? | D | ❌ não sabia | **fora** |
| 49 | Ponto de função | C | C | ✅ | cai |
| 50 | ISO 27005: tratamento do risco | C | E | ❌ (com dúvida) | cai |
| 51 | Risco residual | C? | D | ❌ não sabia | cai |
| 52 | Controle de acesso: RBAC | A | A | ✅ (com dúvida) | cai |
| 53 | Continuidade: RTO e RPO | D? | C | ❌ não sabia | cai |
| 54 | Segregação de funções | C | C | ✅ (com dúvida) | cai |
| 55 | ISO 27002: proprietário do ativo | C | C | ✅ | cai |
| 56 | Linux: systemctl disable | E | B | ❌ convicto | cai (limítrofe) |
| 57 | UML: diagrama de objetos | D | D | ✅ | cai |
| 58 | Arquitetura corporativa: Zachman | D | B | ❌ convicto | cai (limítrofe) |
| 59 | Balanceador: afinidade de sessão | C? | D | ❌ não sabia | cai |
| 60 | Modelo cascata | D | D | ✅ (com dúvida) | cai |

---

## 3. Questão a questão

# Língua Portuguesa (5/10)

> **Texto-base das 10 questões** (última página de *Os Sertões*, de Euclides da Cunha):
>
> **Canudos não se rendeu**
>
> Fechemos este livro.
>
> Canudos não se rendeu. Exemplo único em toda a história, resistiu até ao esgotamento completo. Expugnado palmo a palmo, na precisão integral do termo, caiu no dia 5, ao entardecer, quando caíram os seus últimos defensores, que todos morreram. Eram quatro apenas: um velho, dois homens feitos e uma criança, na frente dos quais rugiam raivosamente 5 mil soldados.
>
> Forremo-nos à tarefa de descrever os seus últimos momentos. Nem poderíamos fazê-lo. Esta página, imaginamo-la sempre profundamente emocionante e trágica; mas cerramo-la vacilante e sem brilhos.
>
> Vimos como quem vinga uma montanha altíssima. No alto, a par de uma perspectiva maior, a vertigem...
>
> Ademais, não desafiaria a incredulidade do futuro a narrativa de pormenores em que se amostrassem mulheres precipitando-se nas fogueiras dos próprios lares, abraçadas aos filhos pequeninos...
>
> [...] Caiu o arraial a 5. No dia 6 acabaram de o destruir desmanchando-lhe as casas, 5.200, cuidadosamente contadas.

## Questão 1 · ❌ Errou (com dúvida) · riscou a certa

A primeira frase do texto – "Fechemos este livro" – aparece escrita na primeira pessoa do plural porque

(A) se refere ao autor e aos seus possíveis leitores. ← sua resposta (com pontinho)

(B) está ligada à pessoa do autor e ao grupo de pessoas que o auxiliavam.

✅ **\(C) se trata de um plural enfático, já que se trata de uma ação praticada pelo autor do livro.**

(D) se liga às pessoas do autor e do editor do texto.

(E) se prende a todos os futuros leitores da obra.

**Depende de:** interpretação e pessoas do discurso (Português, **Módulo H**: blocos feitos em 12/11, teoria ainda pendente).

**Por que errou:** você pôs pontinho em A, B e E e riscou a palavra "enfático" na (C). A ideia de "autor + leitor" parece natural (o leitor também fecha o livro), mas olhe os outros verbos do texto: "Forremo-nos", "imaginamo-la", "cerramo-la", "Vimos". O leitor não "imaginou a página" nem a "cerrou vacilante": quem fez tudo isso foi **só o autor**. É o **plural de modéstia** (o autor diz "nós" no lugar de "eu"), que a banca chamou de "plural enfático". O X em "enfático" não tinha prova: a palavra era estranha, não errada.

📌 **"Nós" em texto de um autor só: teste se o leitor poderia praticar todas as ações. Se não pode (imaginar, escrever, encerrar a obra), é plural de modéstia: "nós" = o autor.**

---

## Questão 2 · ❌ Errou (convicto)

"Eram quatro apenas: um velho, dois homens feitos e uma criança, na frente dos quais rugiam raivosamente 5 mil soldados."

Com esse segmento, o autor pretende

(A) indicar o despreparo dos habitantes de Canudos diante de um poderoso inimigo.

✅ **(B) demonstrar o heroísmo dos defensores do povoado de Canudos diante da tropa do Exército brasileiro.**

\(C) mostrar o fanatismo dos moradores de Canudos, já que não havia a menor chance de resistência.

(D) destacar a crueldade das tropas, já que os adversários não tinham a menor chance de enfrentá-los. ← sua resposta

(E) comprovar a veracidade de sua narrativa, dando pormenores da situação narrada.

**Depende de:** finalidade de um segmento (**Módulo H**; mesmo tipo da Q2 do Simulado 01 e da questão do chat de 12/11, as duas erradas).

**Por que errou:** você sublinhou "raivosamente 5 mil soldados" e ficou com a parte dos soldados. Mas o **sujeito** do segmento são os quatro ("Eram quatro apenas") e a frase vem logo depois da tese do texto: "Canudos não se rendeu. Exemplo único em toda a história, resistiu até ao esgotamento completo". O contraste 4 × 5 mil serve para engrandecer **quem resistiu**. Além disso, a (D) diz que eles "não tinham a menor chance de enfrentá-los", e o texto diz que enfrentaram até o último cair.

📌 **Finalidade de um segmento: ligue a frase à tese do texto (aqui, o título). O sujeito da frase mostra de quem o autor está falando. Terceira vez que a "finalidade" cai e é errada: é prioridade na teoria do H.**

---

## Questão 3 · ❌ Errou (com dúvida)

"Forremo-nos à tarefa de descrever os seus últimos momentos. Nem poderíamos fazê-lo. Esta página, imaginamo-la sempre profundamente emocionante e trágica; mas cerramo-la vacilante e sem brilhos."

Assinale a afirmativa **incorreta** sobre esse segmento do texto.

(A) O autor se nega a relatar os últimos acontecimentos pela impossibilidade de fazê-lo.

(B) O verbo "descrever" está empregado em lugar de "narrar", já que se trata de uma sequência de acontecimentos.

\(C) O narrador mostra sua decepção diante dos acontecimentos que ele imaginara grandiosos. ← sua resposta

✅ **(D) O escritor mostra a impossibilidade de descrever os fatos por sua exagerada crueldade.**

(E) O texto indica a limitação do autor do texto diante de alguns.

**Depende de:** interpretação com comando negativo (**Módulo H** + estratégia "INCORRETA").

**Por que errou:** o método estava certo: você circulou "incorreta" e deu ✓ em A, B, D e E. O erro foi dar ✓ na (D). O trecho diz "Nem poderíamos fazê-lo", mas **não diz que o motivo é a crueldade**: o motivo é a limitação de quem escreve ("cerramo-la vacilante e sem brilhos"), exatamente o que a (E) afirma. D e E dão **causas diferentes** para a mesma coisa, então as duas não podem ser verdadeiras. A (C) tem redação frouxa (o autor imaginou a *página* "emocionante e trágica", não os acontecimentos "grandiosos"), e foi isso que você circulou; mas a ideia de expectativa frustrada está no texto ("imaginamo-la… mas cerramo-la…").

📌 **Em "incorreta" de interpretação, desconfie da alternativa que acrescenta uma causa ("por sua exagerada crueldade") que o trecho não dá. Se duas alternativas explicam o mesmo fato por causas diferentes, uma delas é a falsa (regra de 30/10).**

---

## Questão 4 · ✅ Acertou

"Ademais, não desafiaria a incredulidade do futuro a narrativa de pormenores em que se amostrassem mulheres precipitando-se nas fogueiras dos próprios lares, abraçadas aos filhos pequeninos..."

A incredulidade dos leitores futuros se deve

✅ **(A) à presença de ações humanamente inimagináveis.** ← sua resposta

(B) à falta de documentos que comprovem os fatos narrados.

\(C) à ausência de outros depoimentos que confirmem o que é relatado.

(D) ao fato de as ações narradas não terem sido presenciadas pelo autor, mas somente contadas a ele.

(E) ao exagero das histórias contadas sobre esse episódio da história nacional.

**Confirmação:** acerto firme, com B, C e E riscadas. O que o leitor do futuro não acreditaria é o próprio fato (mães se atirando ao fogo com os filhos). Documentos (B), depoimentos (C), testemunho indireto (D) e exagero (E) não aparecem no texto: são extrapolações.

📌 **Inferência: a causa tem de estar no trecho. Alternativa que traz elemento novo (documentos, depoimentos, exagero) é extrapolação.**

---

## Questão 5 · ❌ Não sabia ("?") · riscou a certa

"Eram quatro apenas: um velho, dois homens feitos e uma criança, na frente dos quais rugiam raivosamente 5 mil soldados."

Nesse segmento o termo "dos quais" retoma um termo anterior – "um velho, dois homens feitos e uma criança".

Nas opções a seguir, de citações diversas, há termos destacados que são referidos na continuidade da frase. Assinale aquela em que essa segunda referência é feita por um termo cognato.

(A) "Muitos julgam cumprir o seu dever pronunciando <u>aforismos abstratos</u> para uso alheio em vez de pregar por meio de exemplo." (Ibsen)

(B) "<u>Qualquer coisa</u> que faças, faze-o com prudência e considera o fim." (Gesta Romanorum)

\(C) "Nunca fazemos bem <u>alguma coisa</u> enquanto não paramos de pensar na maneira de fazê-la." (W. Hazlitt) ← sua resposta

✅ **(D) "Viver é <u>raciocinar</u>. E o raciocínio é o supremo bem da vida. Quem raciocina não sofre." (Joracy Camargo)**

(E) "Água, <u>água</u> por toda a parte, e nenhuma gota para beber." (Coleridge)

**Depende de:** coesão: formas de retomada (**Módulo G, estudado em 12/11**) + vocabulário ("cognato").

**Por que errou:** o "?" está em cima de "cognato", ou seja, faltou o significado da palavra. **Cognato = palavra da mesma família, com o mesmo radical**: raciocinar → raciocínio → raciocina. Em (C), "alguma coisa" é retomada por "la", que é **pronome** (como em B, com "o"). Em (E), a palavra é só repetida. Você riscou a (D) sem saber o que o comando pedia: sem entender o comando, não dá para riscar nada.

📌 **Cognato = mesmo radical (viver/vida, raciocinar/raciocínio). Retomada pode ser por pronome (o, la, ele), por repetição, por sinônimo ou por cognato. Palavra desconhecida no comando: não risque nenhuma alternativa; procure a que é "diferente das outras".**

---

## Questão 6 · ✅ Acertou

O texto traz uma série de vocábulos cultos, próprios da época do livro.

Assinale a frase em que a substituição de um termo abrangente por um mais simples foi feita de forma **inadequada**.

(A) "O absurdo é o mistério dos <u>incrédulos/descrentes</u>." (Mário da Silva Brito)

✅ **(B) "<u>A finalidade/O término</u> da humanidade é produzir grandes homens." (Renan)** ← sua resposta

\(C) "<u>O irreligioso/O ateu</u> é como o enjeitado que não conhece o seu pai, é como o animal bruto, comensal do banquete da natureza, que não cuida nem pergunta pelo seu benfeitor." (Marquês de Maricá)

(D) "A vida é cheia de <u>obrigatoriedades/obrigações</u> que a gente cumpre por mais vontade que tenha de as infringir deslavadamente." (Machado de Assis)

(E) "Os mortos param no cemitério, e lá vai ter a afeição dos vivos, com as suas flores e <u>recordações/lembranças</u>." (Memorial de Aires, Machado de Assis)

**Confirmação:** acerto firme, com o método certo (✓ em C, D e E). "Finalidade" é objetivo; "término" é o fim no tempo. A troca muda o sentido da frase. Nas outras, o par é de sinônimos no contexto.

📌 **"Fim" tem dois sentidos (objetivo e término). "Finalidade" só tem o primeiro. Em questão de substituição, teste a troca dentro da frase.**

---

## Questão 7 · ❌ Errou (com dúvida)

"Ademais, não desafiaria a incredulidade do futuro a narrativa de pormenores em que se amostrassem mulheres precipitando-se nas fogueiras...".

Nessa frase, o vocábulo "amostrassem" equivale a "mostrassem".

Assinale a frase em que houve troca **indevida** entre parônimos, com relação às palavras sublinhadas.

✅ **(A) "Pode-se precisar <u>espiar</u> não somente más ações, mas erros da própria natureza." (Marquês de Custine) / espiar / expiar.**

(B) "É de altos espíritos <u>aspirar</u> a coisas altas." (Cervantes) / aspirar / expirar.

\(C) "A descrença é fenômeno alheio à vontade do eleitor; a <u>abstenção</u> é propósito." (A Semana, Machado de Assis) / abstenção / abstração. ← sua resposta

(D) "A ternura não embarga a <u>discrição</u> nem esta diminui aquela." (Memorial de Aires, Machado de Assis) / descrição / discrição.

(E) "Era <u>esperto</u> e arguto: entendia as coisas sem largo dispêndio de palavras." (Papéis Avulsos, Machado de Assis) / esperto / experto.

**Depende de:** semântica: parônimos (parte do **Módulo G** que não teve bloco próprio).

**Por que errou:** você deu ✓ na (A), isto é, achou que "espiar" estava certo ali. **Espiar = olhar escondido. Expiar = pagar por uma culpa.** "Más ações" e "erros" se **expiam**: a frase usou a palavra errada. Na (C), "abstenção" (deixar de votar) está certa: o texto fala do eleitor. O método de V/F funcionou; faltou conhecer o par.

📌 **Espiar (espreitar) × expiar (pagar a culpa) · aspirar (almejar) × expirar (soltar o ar, vencer o prazo) · discrição (reserva) × descrição (ato de descrever) · esperto (vivo) × experto (perito) · abstenção (não participar) × abstração.**

---

## Questão 8 · ✅ Acertou (com dúvida)

"Caiu o arraial a 5. No dia 6 acabaram de o destruir desmanchando-lhe as casas, 5.200, cuidadosamente contadas."

Nesse último parágrafo do texto, o termo "arraial" foi substituído, na continuidade do texto, pelo pronome pessoal "o".

Assinale a frase abaixo em que o termo sublinhado **não** é repetido na sequência da frase por um pronome pessoal.

(A) "A <u>natureza</u> nunca traiu o coração que a amou." (William Wordsworth)

(B) "Ponha o pé com cuidado sobre a <u>crosta terrestre</u> – ela é fina." (Edna St. Vicente Milley)

✅ **\(C) "A <u>vida</u> que a gente vive não deixa a gente viver." (Álvaro Pacheco)** ← sua resposta

(D) "Qual pode ser a <u>vida</u> que começa pelos gritos da mãe, que a dá, e o choro do filho que a recebe?" (Baltasar Gracián)

(E) "Não penso na <u>idade</u>, ela cuida de si." (Tatiana Belinky)

**Depende de:** coesão: retomada por pronome (**Módulo G, estudado em 12/11**).

**Confirmação:** em (C), "vida" só é retomada por "que", **pronome relativo**. Nas outras há pronome pessoal: "a amou" (A), "ela é fina" (B), "a dá… a recebe" (D), "ela cuida" (E). Você ficou em dúvida com a (E), mas marcou os pronomes nas frases e decidiu certo.

📌 **Pronome pessoal: ele/ela, o/a, lhe. "Que" depois de substantivo é pronome relativo, outra classe. Numa "NÃO", ache o item que usa um recurso diferente dos demais.**

---

## Questão 9 · ✅ Acertou (com dúvida)

"Esta página, imaginamo-la sempre profundamente emocionante e trágica; mas cerramo-la vacilante e sem brilhos." Nessa frase, o autor evitou usar expressões negativas ou agressivas, substituindo-as por "vacilante e sem brilhos".

As frases abaixo mostram processos de atenuar expressões consideradas agressivas, prejudiciais ou desagradáveis.

Assinale a opção em que esse processo foi realizado de forma adequada.

✅ **(A) O jogador, quando criança, morava num bairro miserável. / numa área socioeconômica baixa.** ← sua resposta

(B) O horário dos coletores de lixo no bairro estava marcado às 9 horas / lixeiros.

\(C) A empresa reconhece problemas na nova distribuição de empregos / de desemprego.

(D) A indústria reconhece estar falida / com fluxo de caixa altamente positivo.

(E) O foguete lançado chocou-se prematuramente contra o solo / despencou.

**Confirmação:** eufemismo é trocar o termo duro por um mais suave, **sem mudar o fato**. Só a (A) faz isso. Em (B), (C) e (E), a troca vai do suave para o duro (direção contrária). Em (D), muda o sentido: "fluxo de caixa altamente positivo" é o oposto de "falida".

📌 **Eufemismo: duro → suave, mesmo fato. Conferir a direção da troca e se o sentido foi mantido.**

---

## Questão 10 · ✅ Acertou (com dúvida)

Um texto, às vezes, perde leitores por ser mal construído, o que não ocorre com o texto.

Assinale a frase a seguir, mal-estruturada, que mostra seu problema de escrita perfeitamente identificado.

✅ **(A) Sabemos todos que você comprou um carro novo e, por isso, pode estacionar teu carro no meu prédio. / Mistura de pessoas pronominais.** ← sua resposta

(B) Você e sua esposa estão convidados para a festa na minha casa de praia. / Ambiguidade.

\(C) Embora a chuva tenha durado pouco tempo, foi o suficiente para encher algumas ruas. / Uso inadequado de conectivos.

(D) Todos os moradores da cidade requereram mais policiamento nas ruas. / Mau emprego de formas verbais.

(E) Como havia tempestade, o avião teve que aterrissar em outro aeroporto do estado. / A segunda frase não é uma sequência lógica da primeira.

**Confirmação:** "você" pede 3ª pessoa ("seu carro"); "teu" é de 2ª. Você circulou "teu" e escreveu "seu" ao lado: exatamente o defeito. Nas outras, o rótulo não confere: (B) não é ambígua, (C) usa "embora" corretamente, (D) "requereram" está certo, (E) tem causa e consequência coerentes.

📌 **Uniformidade de tratamento: você → seu, lhe, o. Tu → teu, te. Misturar é erro de construção (liga com "pronomes pela norma", ponto fraco 2).**

---

# Raciocínio Lógico-Matemático (6/10)

## Questão 11 · ✅ Acertou

Alberto comprou um carro por 50.000 reais e o vendeu com lucro de 40%. Em seguida, comprou outro carro por 75.000 reais e o vendeu com lucro de 10%.

O lucro total de Alberto nessas duas transações foi de

✅ **(A) 22%.** ← sua resposta

(B) 25%.

\(C) 28%.

(D) 36%.

(E) 50%.

**Confirmação:** acerto firme, com a conta na margem. Lucro = 40% de 50.000 + 10% de 75.000 = 20.000 + 7.500 = 27.500. Investido = 125.000. 27.500 ÷ 125.000 = 22%. A pegadinha era fazer a média de 40% e 10% (25%, alternativa B) ou somar (50%, alternativa E).

📌 **Porcentagem total de duas operações com bases diferentes = (soma dos lucros) ÷ (soma dos custos). Nunca a média simples das taxas.**

---

## Questão 12 · ✅ Acertou, mas com "?" (chute)

João e Manoel estão em uma fila. Há 17 pessoas antes de João, 22 pessoas entre João e Manoel e 14 pessoas depois de Manoel. Eles percebem que Francisco, um amigo comum é a pessoa central da fila, ou seja, há tantas pessoas antes de Francisco quantas depois dele.

O número de pessoas entre Francisco e Manoel é

(A) 11.

✅ **(B) 12.** ← sua resposta

\(C) 13.

(D) 14.

(E) 15.

**Depende de:** raciocínio sequencial: posições em fila (ponto fraco 15, ainda sem bloco).

**Como resolver com segurança:** dê um **número de posição** a cada um. João = 18º (17 antes). Manoel = 18 + 22 + 1 = 41º. Total = 41 + 14 = 55. O central é o 28º (27 antes, 27 depois). Entre o 28º e o 41º: 41 − 28 − 1 = **12**. Na sua margem aparece "18 + 22 = 40": faltou somar 1 (o próprio Manoel ocupa uma posição). O resultado saiu certo, mas por um caminho com erro, daí o "?".

📌 **Fila: transforme tudo em posição. "k pessoas antes" = posição k + 1. "Entre a posição a e a b" = b − a − 1. Central de n (ímpar) = (n + 1) ÷ 2.**

---

## Questão 13 · ✅ Acertou

Considere verdadeiras as afirmações:

- Se o cão não ladra, Maria dorme.
- Se o cão ladra, Joana não sai de casa.

Considere também como verdadeira que: Joana sai de casa.

É correto concluir que

(A) o cão ladra e Maria dorme.

(B) o cão ladra e Maria não dorme.

✅ **\(C) o cão não ladra e Maria dorme.** ← sua resposta

(D) o cão não ladra e Maria não dorme.

(E) se Joana sai de casa então Maria não dorme.

**Depende de:** lógica proposicional (**estudada**; firme desde o Simulado 01).

**Confirmação:** acerto firme, com os valores V/F escritos nas setas. Joana sai → a segunda condicional tem consequente falso → o antecedente é falso → o cão **não** ladra → pela primeira, Maria dorme.

📌 **Condicional verdadeira com consequente falso obriga antecedente falso (contrapositiva). Começar sempre pela premissa simples.**

---

## Questão 14 · ✅ Acertou

Em julho de 2025 o Brasil atingiu a produção de 5 milhões de barris de petróleo por dia (Fonte: Agência Brasil em 01/09/2025).

Considere que 1 barril de petróleo seja equivalente a 160 litros.

A produção diária de petróleo nesse mês em metros cúbicos foi de

(A) 80.000.

✅ **(B) 800.000.** ← sua resposta

\(C) 8.000.000.

(D) 80.000.000.

(E) 800.000.000.

**Confirmação:** acerto firme, com potências de 10 na margem. 5 × 10⁶ barris × 160 L = 8 × 10⁸ L. Como 1 m³ = 1.000 L, divide por 10³: 8 × 10⁵ = 800.000 m³.

📌 **1 m³ = 1.000 litros. Em conta com muitos zeros, usar potência de 10, como você fez.**

---

## Questão 15 · ❌ Não sabia ("?")

Ana, Bernardo, César e Débora vão ocupar 4 poltronas vizinhas de uma fila do cinema. O lugar de cada um será decidido por sorteio. Entretanto, Ana deseja ficar ao lado de Bernardo e não gostaria de ficar ao lado de César.

Nesse sorteio, a probabilidade de que os desejos de Ana sejam atendidos é

(A) 1/2.

✅ **(B) 1/3.**

\(C) 2/3.

(D) 1/4.

(E) 3/4. ← sua resposta (só no cartão; no caderno ficou o "?")

**Depende de:** combinatória e probabilidade (RLM, ainda não estudado; ponto fraco 13b desde o Simulado 01).

**Como resolver:** total de filas = 4! = 24. **Ana ao lado de Bernardo:** trate "AB" como um bloco: 3 blocos se arrumam de 3! = 6 modos, vezes 2 (AB ou BA) = 12. **Tire os casos em que César também está ao lado de Ana:** Ana no meio de Bernardo e César (BAC ou CAB) forma um bloco de 3, mais a Débora: 2 × 2 = 4. Favoráveis = 12 − 4 = 8. Probabilidade = 8/24 = **1/3**.

📌 **"Juntos" = bloco (multiplica pelas ordens internas). "Juntos, mas não ao lado de outro" = total do bloco − casos em que o outro também encosta. Probabilidade = favoráveis ÷ total (n!).**

---

## Questão 16 · ✅ Acertou, mas com "?" (chute)

Os números inteiros 1, 2, 3, ..., 19 são escritos nessa ordem em volta de um círculo no sentido anti-horário. Uma borracha está sobre o número 1. A borracha inicia seu movimento, também no sentido anti-horário, apagando o número onde está, pulando os dois números seguintes e apagando o próximo. A borracha continua seu movimento em volta do círculo, repetindo o mesmo procedimento, volta após volta, até que sobrem apenas dois números.

A soma desses dois números é

(A) 17.

(B) 19.

\(C) 21.

✅ **(D) 23.** ← sua resposta

(E) 25.

**Depende de:** raciocínio sequencial (ponto fraco 15).

**Como resolver:** só simulando, e você começou certo (a lista de 19 a 1 com riscos está na margem). **1ª volta:** apaga 1, 4, 7, 10, 13, 16, 19. **2ª volta** (pula 2 e 3): apaga 5, 9, 14, 18. Sobram 2, 3, 6, 8, 11, 12, 15, 17. **Depois:** apaga 6, 12, 2 → sobram 3, 8, 11, 15, 17 → apaga 11, 3 → sobram 8, 15, 17 → apaga 17. Restam **8 e 15**: soma 23. O cuidado é que, a partir da 2ª volta, só se contam os números **que ainda existem**.

📌 **Problema de "apaga e pula" em círculo: escrever a lista, riscar de verdade e, a cada volta, pular só os que sobraram. Não tem fórmula: é simulação organizada (2 a 3 minutos).**

---

## Questão 17 · ❌ Errou (convicto)

Um grupo de crianças em bicicletas e triciclos passou em frente à casa de Joana. Em cada veículo havia uma única criança. Joana contou 11 crianças e 28 rodas.

O número de triciclos que passou em frente à casa de Joana foi

(A) 4. ← sua resposta

(B) 5.

✅ **\(C) 6.**

(D) 7.

(E) 8.

**Depende de:** sistema de duas equações (RLM, matemática básica; ainda sem bloco).

**Por que errou:** na margem você testou "8 e 4": 8 bicicletas (16 rodas) + 4 triciclos (12 rodas) = 28 rodas. As rodas fecharam, mas **8 + 4 = 12 crianças, e são 11**. Você conferiu só uma das duas condições. O caminho rápido: se as 11 fossem bicicletas, seriam 22 rodas. Faltam 6 rodas, e cada triciclo acrescenta 1 roda: **6 triciclos** (e 5 bicicletas: 10 + 18 = 28).

📌 **Duas condições (cabeças e rodas): a resposta tem de fechar as DUAS. Atalho: suponha tudo do tipo menor; cada troca acrescenta a diferença. Erro convicto em conta: reler o enunciado e conferir cada número antes de marcar (regra de 27/10).**

---

## Questão 18 · ✅ Acertou

Para caminhar 1,2 quilômetro em seu quintal retangular, Mariana tem que caminhar 30 vezes o comprimento ou 10 vezes o perímetro do quintal.

A área do quintal de Mariana, em metros quadrados, é

(A) 600.

✅ **(B) 800.** ← sua resposta

\(C) 900.

(D) 1000.

(E) 1200.

**Confirmação:** 1,2 km = 1.200 m. Comprimento = 1.200 ÷ 30 = 40 m. Perímetro = 1.200 ÷ 10 = 120 m → 2 × (40 + largura) = 120 → largura = 20 m. Área = 40 × 20 = **800 m²**. Na margem você usou 12.000 em vez de 1.200 (chegou a 400 e 200) e acertou a letra mesmo assim: confira a conversão de km para m antes de montar a conta.

📌 **1 km = 1.000 m. Perímetro do retângulo = 2 × (comprimento + largura). Converter as unidades antes de montar as equações.**

---

## Questão 19 · ❌ Não sabia ("?")

Márcia pagou um certo valor por 3 picolés e 5 bombons. Bruno pagou o dobro do valor pago por Márcia por 5 picolés e 13 bombons.

A razão entre o valor de 1 picolé e o valor de 1 bombom é igual a

(A) 1.

(B) 3/2.

\(C) 2. ← sua resposta (só no cartão)

(D) 5/2.

✅ **(E) 3.**

**Depende de:** equações e razão (RLM: razão e proporção é o próximo do mapa, depois de porcentagem).

**Por que errou:** a montagem estava **certa**: x = 3p + 5b e 2x = 5p + 13b. O passo seguinte é que travou: você **somou** as duas (3x = 8p + 18b), o que mantém o x na conta. O que resolve é **substituir** o x da primeira na segunda: 2 × (3p + 5b) = 5p + 13b → 6p + 10b = 5p + 13b → **p = 3b**. Razão picolé/bombom = 3.

📌 **Duas equações com uma incógnita "sobrando" (x): substitua, não some. O objetivo é fazer o x desaparecer. Razão entre p e b = isolar p em função de b.**

---

## Questão 20 · ❌ Não sabia ("?")

Para quaisquer números reais x e y, com y ≠ 0, pode-se definir resto(x, y) = x − y ⌊x/y⌋, onde ⌊x/y⌋ representa o maior número inteiro que é menor ou igual a x/y.

O valor de resto(3/5, −2/7) é:

✅ **(A) −9/35.**

(B) −6/35.

\(C) −21/10.

(D) 14/15.

(E) 5/12. ← sua resposta (só no cartão)

**Depende de:** frações e função piso (matemática; não está no mapa de RLM e raramente cai).

**Como resolver:** é só seguir a receita do enunciado. **1)** x/y = (3/5) ÷ (−2/7) = (3/5) × (−7/2) = −21/10 = −2,1. **2)** Maior inteiro menor ou igual a −2,1 é **−3** (e não −2: em número negativo, "menor" é mais para a esquerda). **3)** resto = 3/5 − (−2/7) × (−3) = 3/5 − 6/7 = 21/35 − 30/35 = **−9/35**. A alternativa (C) é o resultado só do passo 1; a (B) é de quem usa −2 no piso.

📌 **Questão com "define-se a operação…": não precisa conhecer o assunto, só aplicar a definição passo a passo. Piso de negativo desce: ⌊−2,1⌋ = −3. Vale o tempo só depois de garantir as mais fáceis.**

---

# Conhecimentos Específicos (19/40)

## Questão 21 · ✅ Acertou (com dúvida)

Em um projeto para desenvolver um novo sistema de gestão de Comissões Parlamentares na Assembleia Legislativa, o Analista de Sistemas identificou um conflito significativo entre a Secretaria-Geral da Mesa (SGM) e a Procuradoria. A SGM exige um requisito de flexibilidade para alterar fluxos de trabalho rapidamente conforme a agenda política, enquanto a Procuradoria exige um requisito de rastreabilidade e imutabilidade processual para garantir a validade legal dos atos, independentemente da celeridade.

Nesse contexto, assinale a opção que apresenta a tarefa da Engenharia de Requisitos mais crítica para resolver o conflito entre a SGM e a Procuradoria e a técnica tipicamente empregada nessa resolução.

✅ **(A) Análise de Requisitos: O uso de Viewpoint Analysis é essencial para mapear as diferentes perspectivas e, em seguida, utilizar a negociação para alcançar um acordo de compromisso.** ← sua resposta

(B) Especificação de Requisitos: A elaboração de um Documento de Requisitos de Software (DRS) no padrão IEEE 830 com alta granularidade resolve o conflito pela formalização estrita das regras.

\(C) Gerenciamento de Requisitos: O emprego de uma Matriz de Rastreabilidade Bidirecional garantirá que todas as alterações flexíveis da SGM sejam controladas sem a necessidade de negociação prévia.

(D) Elicitação de Requisitos: A realização de entrevistas individuais aprofundadas com o Presidente da Casa Legislativa para definir a prioridade política do sistema, eliminando a necessidade de conciliar visões técnicas.

(E) Validação de Requisitos: A utilização de inspeções para verificar a conformidade dos requisitos de flexibilidade com as normas ISO 25010 de Manutenibilidade e Eficiência.

**Depende de:** engenharia de requisitos (**estudada na Semana 1**).

**Confirmação:** conflito entre partes interessadas se resolve na **análise e negociação**. Você riscou C e D pelas palavras certas ("sem a necessidade de negociação prévia", "eliminando a necessidade de conciliar"): foi o protocolo anti-riscar bem aplicado. (B) e (E) não resolvem conflito: documentar ou inspecionar um requisito contraditório não o concilia.

📌 **Conflito entre stakeholders → análise e negociação de requisitos (pontos de vista). Elicitar = descobrir · analisar = classificar, modelar, resolver conflito · especificar = documentar · validar = conferir com o cliente · gerenciar = controlar mudança e rastrear.**

---

## Questão 22 · ✅ Acertou (com dúvida)

O setor de TI da Casa Legislativa está iniciando o projeto de um novo Sistema de Apoio à Consulta Pública e Audiências Interativas, com o objetivo não apenas de aumentar a participação cidadã, mas também cumprir integralmente com as novas exigências da Lei Geral de Proteção de Dados (LGPD) e de Acessibilidade Digital (eMAG). A equipe de Engenharia de Requisitos precisa priorizar e especificar os Requisitos Não Funcionais (RNFs) que são críticos para a aceitação pública e para a conformidade legal do sistema.

Correlacione os conceitos e as técnicas de Engenharia de Requisitos listados na Coluna I da tabela abaixo com suas aplicações e descrições complexas no contexto do setor público/legislativo, apresentadas na Coluna II.

| Coluna I: Conceitos e técnicas de Engenharia de Requisitos | Coluna II: Aplicações e descrições |
|---|---|
| I\. Goal-Oriented Requirements Engineering (GORE) | A. Exige a blindagem de dados pessoais sensíveis de cidadãos em consultas públicas, aplicando a Lei Geral de Proteção de Dados e políticas de sigilo institucional. |
| II. Requisito de confidencialidade | B. O tempo máximo para carregar o inteiro teor de um projeto de lei complexo em consulta popular, medido em picos de acesso após votações importantes, em conformidade com as diretrizes de Acessibilidade. |
| III. Método FURPS+ | C. Utilizado para ligar requisitos de sistema a objetivos estratégicos de alto nível (ex: "Aumento da Transparência Legislativa"), ajudando a justificar e priorizar sistemas de apoio à decisão. |
| IV. Requisito de Desempenho | D. Estrutura robusta para classificação de Requisitos Não Funcionais e outros atributos como Design, Implementação e Operacional. |

A correlação correta, na ordem apresentada, é

✅ **(A) I – C; II – A; III – D; IV – B** ← sua resposta

(B) I – A; II – C; III – D; IV – B

\(C) I – C; II – D; III – A; IV – B

(D) I – B; II – A; III – C; IV – D

(E) I – D; II – C; III – A; IV – B

**Depende de:** requisitos não funcionais (**estudado**); GORE e FURPS+ são novos.

**Confirmação:** você ancorou no que sabia (IV = desempenho = tempo de carga = B, anotado na tabela) e eliminou a (D). GORE = orientado a **objetivos** (goal) → C. Confidencialidade = sigilo de dados → A. FURPS+ = modelo de **classificação** de requisitos → D.

📌 **FURPS+ = Functionality, Usability, Reliability, Performance, Supportability; o "+" são as restrições de design, implementação, interface e físicas. GORE = requisitos derivados de objetivos (goals). Em questão de correlacionar, começar pelo par que você tem certeza.**

---

## Questão 23 · ✅ Acertou

A equipe de TI está desenvolvendo um módulo de consulta de histórico de votações, um sistema de alta complexidade em termos de interface e volume de dados. Os usuários finais (assessores parlamentares e jornalistas) têm dificuldade em articular suas necessidades de interface exata, e o ambiente legislativo exige validação rápida, porém o custo de desenvolver uma solução completa do zero é muito alto.

Considerando a necessidade de obter *feedback* rápido sobre a interface em um ambiente de alto custo de desenvolvimento, assinale a opção que apresenta o tipo de prototipação mais adequado e seu principal objetivo estratégico nesse cenário.

(A) Prototipação Evolutiva: O objetivo é construir o protótipo como a primeira versão do sistema final, garantindo que o investimento inicial seja mantido e evoluído após a validação do usuário.

✅ **(B) Prototipação Descartável: O objetivo é definir e refinar os requisitos de interface e usabilidade (RNF), sendo o código posteriormente descartado para que a implementação final seja feita sobre uma arquitetura robusta.** ← sua resposta

\(C) Modelagem de Casos de Uso: Não é uma forma de prototipação, mas é o método mais eficaz para capturar os requisitos de interface e interação sem a necessidade de construir um modelo visual.

(D) Prototipação de Baixa Fidelidade: O objetivo é construir um modelo interativo completo usando código de produção para validar o desempenho do sistema e a velocidade de carregamento dos dados.

(E) Prototipação Vertical: Foca na validação da arquitetura e das camadas mais profundas (banco de dados e backend), ignorando a interface e a interação com o usuário, que não são críticas para este projeto.

**Depende de:** prototipação na elicitação (**estudada**; era o ponto fraco 10, erro de 26/10).

**Confirmação:** acerto firme em item que você tinha errado em outubro. Usuário que não sabe dizer o que quer + necessidade de feedback rápido sobre a **interface** = protótipo **descartável**: serve para descobrir o requisito e depois é jogado fora. (D) se contradiz ("baixa fidelidade" com "código de produção") e (E) ignora justamente a interface.

📌 **Descartável (throwaway) = esclarecer requisito mal compreendido, depois descarta. Evolutivo = começa pelos requisitos bem compreendidos e vira o sistema. Horizontal = interface inteira, rasa · vertical = uma função, até o banco.**

---

## Questão 24 · ✅ Acertou (com dúvida)

Em um projeto de desenvolvimento de um sistema de controle de frotas para uma empresa de logística, o Analista de Sistemas precisa garantir que os requisitos levantados junto aos motoristas e gerentes sejam claros e consistentes antes de iniciar a fase de design. O Analista descobriu que há requisitos contraditórios sobre a forma como o rastreamento deve ser feito em tempo real *versus* por paradas programadas.

Assinale a opção que apresenta a tarefa da Engenharia de Requisitos primariamente responsável por identificar e resolver inconsistências ou contradições como a descrita, transformando a informação bruta dos *stakeholders* em um modelo coerente.

(A) Elicitação de Requisitos, pois a contradição foi descoberta durante a coleta de dados.

(B) Validação de Requisitos, pois é a tarefa final que aprova formalmente a coerência do documento e o tratamento dos conflitos.

\(C) Gerenciamento de Requisitos, pois a contradição deve ser registrada em um log de problemas e controlada.

✅ **(D) Análise de Requisitos, por tratar o processo de refinar, classificar e modelar os requisitos, incluindo a resolução de conflitos.** ← sua resposta

(E) Especificação de Requisitos, pois a formalização no documento evita que as contradições e conflitos se manifestem.

**Depende de:** engenharia de requisitos (**estudada**).

**Confirmação:** você escreveu "VOLTAR NESSA", ficou entre A e D e decidiu certo. A pista é "transformando a informação bruta em um modelo coerente": a informação bruta **já foi coletada** (isso foi a elicitação, e você anotou "já aconteceu" ao lado da A). Transformar em modelo e resolver conflito é **análise**. É a mesma ideia da Q21.

📌 **Informação bruta → modelo coerente = análise. A elicitação termina quando a informação foi colhida; o conflito aparece nela, mas é resolvido na análise.**

---

## Questão 25 · ❌ Errou (convicto) · ⚠️ assunto já estudado

Em um projeto para o desenvolvimento de um aplicativo governamental de serviço ao cidadão, a equipe de desenvolvimento finalizou a fase de Especificação. Antes de prosseguir para a codificação, o Gerente do Projeto exige uma revisão rigorosa para garantir que o produto a ser construído realmente atenda às necessidades regulamentares e de usuário.

O objetivo principal da tarefa de Validação de Requisitos nesse cenário é

(A) garantir que os requisitos estejam documentados usando o padrão *IEEE 830* e que todas as sentenças estejam na forma "O sistema deverá...".

(B) assegurar a rastreabilidade entre cada requisito de usuário e seus respectivos casos de teste no *design*. ← sua resposta

✅ **\(C) provar que os requisitos definidos são completos, consistentes e que, se implementados corretamente, resultarão em um sistema que satisfaça as necessidades do *stakeholder* e de *compliance*.**

(D) descobrir novos requisitos implícitos por meio da observação do usuário final e da análise de documentos legais.

(E) classificar todos os requisitos como Funcionais ou Não Funcionais e atribuir prioridade usando o método MoSCoW.

**Depende de:** validação de requisitos e V&V (**estudado nas Semanas 1 e 2**).

**Por que errou:** você riscou A, D e E e ficou entre B e C, sem pontinho. **Rastreabilidade** é do **gerenciamento** de requisitos (acompanhar o requisito até o teste e a mudança). Validar é responder "estamos construindo o **produto certo**?": os requisitos estão completos, consistentes e refletem o que o cliente precisa. O enunciado dava a resposta quase pronta: "garantir que o produto a ser construído **realmente atenda às necessidades** regulamentares e de usuário" é a (C) com outras palavras.

📌 **Validação de requisitos = produto certo: completos, consistentes, realistas e de acordo com a necessidade do cliente. Rastreabilidade e controle de mudança = gerenciamento. Antes de marcar, compare a alternativa com a frase do enunciado que descreve o objetivo.**

---

## Questão 26 · ❌ Errou (convicto) · riscou a certa · ⚠️ assunto já estudado

O Processo Unificado de Desenvolvimento (RUP) é organizado em quatro fases principais: Iniciação, Elaboração, Construção e Transição. A equipe de projeto do Legislativo precisa garantir que a primeira iteração do projeto esteja focada na mitigação dos riscos de negócio mais críticos e na definição da linha de base da arquitetura.

Assinale a opção que apresenta a principal fase do RUP responsável por alcançar a Linha de Base da Arquitetura e por detalhar os Casos de Uso Críticos do sistema, solidificando a visão do projeto e mitigando os riscos de alto impacto.

(A) Iniciação: Foca primariamente na delimitação do escopo do projeto, na obtenção de patrocínio e na identificação dos *stakeholders* principais.

(B) Transição: Foca na entrega e aceitação do produto final pelo usuário, incluindo testes de *beta* e homologação.

\(C) Construção: Foca no desenvolvimento iterativo incremental do produto, completando todos os requisitos funcionais e não funcionais restantes. ← sua resposta

✅ **(D) Elaboração: Foca na análise detalhada do domínio do problema, na definição da arquitetura do sistema e na mitigação dos riscos técnicos e de negócio mais urgentes.**

(E) Elaboração e Construção, simultaneamente: Ambas as fases compartilham igualmente a responsabilidade pela definição da arquitetura e do desenvolvimento dos casos de uso críticos.

**Depende de:** RUP: fases (**estudado na Semana 1**; ponto fraco 7, estava em "1/2 para sair").

**Por que errou:** você circulou no enunciado "Linha de Base da Arquitetura" e "Casos de Uso Críticos", que são a definição da **Elaboração**, e mesmo assim pôs X na (D). A própria (D) repete as palavras do enunciado ("definição da arquitetura", "mitigação dos riscos"). A Construção **usa** a arquitetura já estabilizada para construir o resto. O X não tinha prova escrita: é o erro mais caro da prova, porque o conteúdo você já estudou.

📌 **RUP: Iniciação = escopo e viabilidade (o quê e vale a pena?) · Elaboração = ARQUITETURA + riscos + casos de uso críticos · Construção = construir o produto · Transição = entregar ao usuário (beta, treinamento). Palavra "arquitetura" ou "linha de base" = Elaboração.**

---

## Questão 27 · ✅ Acertou

A equipe de desenvolvimento precisa codificar a lógica de interação detalhada para o subsistema de autenticação de um novo portal de transparência. É crucial modelar a sequência cronológica exata das mensagens trocadas entre os objetos (usuário, controlador, *backend* de segurança) para garantir que a transação ocorra na ordem correta.

O diagrama da UML 2.5.1 mais apropriado para modelar a ordem cronológica exata das mensagens e das chamadas de método entre os objetos participantes em uma interação específica é o

(A) Diagrama de Comunicação.

(B) Diagrama de *Timing*.

\(C) Diagrama de Visão Geral de Interação.

(D) Diagrama de Atividades.

✅ **(E) Diagrama de Sequência.** ← sua resposta

**Confirmação:** acerto firme. "Ordem cronológica das mensagens entre objetos" = sequência (linhas de vida na vertical, tempo de cima para baixo). Comunicação mostra as mesmas mensagens com foco nos **vínculos** entre objetos; *timing* foca na mudança de estado ao longo do tempo com restrições de duração.

📌 **Sequência = ordem das mensagens no tempo · comunicação = quem fala com quem (vínculos) · atividades = fluxo de trabalho · tempo (timing) = estado × tempo.**

---

## Questão 28 · ❌ Não sabia ("?")

Ao modelar a estrutura de dados e as relações entre as entidades Projeto de Lei, Emenda e Autor para o novo sistema legislativo, o Analista de Sistemas utilizou um Diagrama de Classes. Foi definido que uma Emenda só pode existir se estiver vinculada a um Projeto de Lei, e que, se o Projeto de Lei for excluído, todas as suas Emendas também o serão.

O tipo de relacionamento da UML 2.5.1 mais adequado para modelar a relação entre as Classes Projeto de Lei e Emenda é a

(A) Agregação Fraca.

(B) Associação de Duas Vias. ← sua resposta (só no cartão)

\(C) Dependência.

(D) Associação Qualificada.

✅ **(E) Composição.**

**Depende de:** POO e UML: relacionamentos (próximo assunto da fila, depois de hash).

**Por que errou:** assunto ainda não estudado. A frase-chave é "só pode existir se estiver vinculada" + "se o todo for excluído, as partes também serão": é a definição de **composição** (todo-parte forte, losango **cheio**). Na agregação (losango vazio), a parte sobrevive sem o todo.

📌 **Composição = a parte não vive sem o todo (apagou o todo, apagou as partes; losango cheio). Agregação = a parte existe sozinha (losango vazio). Pista de prova: "só existe se", "é excluído junto".**

---

## Questão 29 · ✅ Acertou

Em um sistema de apoio à tomada de decisão legislativa, é necessário armazenar uma lista de chaves de acesso de tamanho fixo. O requisito mais crítico do sistema é realizar buscas por chaves específicas no menor tempo possível (complexidade O(1) em média), embora o consumo de memória não seja a principal preocupação.

A estrutura de dados mais eficiente para atender ao requisito de busca com complexidade O(1) em média para chaves, mesmo que envolva um *trade-off* no uso de memória, é

(A) a Lista Encadeada.

(B) a Árvore Binária de Busca Balanceada.

\(C) o *Array* Estático.

✅ **(D) a Tabela Hash.** ← sua resposta

(E) o *Heap* Binário.

**Depende de:** tabela hash (teoria dada em 11/11; o bloco de 8 questões ainda está pendente).

**Confirmação:** você escreveu "FÁCIL". Busca por chave em O(1) **médio**, pagando com memória = hash. Árvore balanceada é O(log n); lista é O(n); vetor só é O(1) pelo **índice**, não pela chave.

📌 **Busca por chave em O(1) médio = tabela hash (pior caso O(n), com muitas colisões). O(1) por índice = vetor. O(log n) = árvore balanceada.**

---

## Questão 30 · ❌ Errou (convicto) · ⚠️ assunto já estudado

Um Analista precisa escolher a estrutura de dados mais eficiente para implementar uma lista de tarefas críticas que requer inserções e remoções rápidas em qualquer ponto da lista, pois a prioridade das tarefas pode mudar a qualquer momento no sistema.

A estrutura de dados que oferece a complexidade temporal mais eficiente O(1) para operações de inserção e remoção no meio da estrutura, assumindo que a posição de inserção ou remoção já é conhecida ou localizada por um ponteiro, é o(a)

(A) *Array* Estático.

✅ **(B) Lista Duplamente Encadeada.**

\(C) Tabela Hash.

(D) *Array* Dinâmico. ← sua resposta

(E) Árvore Binária de Busca.

**Depende de:** listas (**estudado em 11/11**, diagnóstico 8/10; é o ponto fraco 0c: "lista do Python = vetor").

**Por que errou:** você riscou A, C e E e deixou a (B) sem nenhuma marca. Em qualquer **vetor** (estático ou dinâmico), inserir ou remover no meio obriga a **deslocar** todos os elementos seguintes: O(n). O "dinâmico" só resolve o tamanho, não o deslocamento. Na lista **duplamente encadeada**, com o ponteiro do nó na mão, basta religar o anterior e o próximo: O(1). O enunciado deu a pista com a palavra "ponteiro". É o mesmo princípio que você errou em `list.pop(0)` (11/11).

📌 **Vetor (estático ou dinâmico): acesso por índice O(1), inserir/remover no meio O(n) por causa do deslocamento. Lista duplamente encadeada: com o ponteiro do nó, inserir/remover é O(1); achar o nó é O(n). Palavra "ponteiro" ou "nó já localizado" = lista encadeada.**

---

## Questão 31 · ✅ Acertou, mas com "?" (chute)

Um Analista de Sistemas está avaliando o design de uma tabela chamada PROJETOS_AUTORES em um sistema de controle de proposições legislativas. A tabela armazena o Título do Projeto (Título_PL), o Código do Autor (Cod_Autor), o Nome Completo do Autor (Nome_Autor) e a Data de Apresentação (Dt_Apresentacao).

A chave primária é composta por (Título_PL, Cod_Autor).

| Título_PL | Cod_Autor | Nome_Autor | Dt_Apresentacao |
|---|---|---|---|
| PL 10/2025 | 150 | Ana Silva | 2025-03-10 |
| PL 10/2025 | 210 | Bruno Costa | 2025-03-10 |
| PL 10/2025 | 150 | Ana Silva | 2025-04-01 |

Assinale a opção que mostra a Forma Normal (FN) da tabela acima e qual o tipo de anomalia seria observada se fosse necessário alterar o Nome_Autor para todos os projetos de um autor específico.

(A) 1FN (Primeira Forma Normal); a anomalia observada seria a Anomalia de Inserção.

(B) 2FN (Segunda Forma Normal); a anomalia observada seria a Anomalia de Exclusão.

\(C) 2FN (Segunda Forma Normal); a anomalia observada seria a Anomalia de Atualização.

(D) 3FN (Terceira Forma Normal); a anomalia observada seria a Anomalia de Exclusão.

✅ **(E) 1FN (Primeira Forma Normal); a anomalia observada seria a Anomalia de Atualização.** ← sua resposta

**Depende de:** normalização (Semana 4 do plano: é o assunto desta semana).

**O que faltou saber (você ficou entre C e E):** a anomalia você acertou nas duas: **alterar** o nome em várias linhas = anomalia de **atualização**. A dúvida era 1FN × 2FN. A chave é composta (Título_PL, Cod_Autor), mas Nome_Autor depende **só de Cod_Autor**, que é um pedaço da chave. Isso é **dependência parcial**, que viola a 2FN. Então a tabela só chega à **1FN**.

📌 **1FN = valores atômicos · 2FN = 1FN + nenhum atributo depende só de PARTE da chave composta · 3FN = 2FN + nenhum atributo depende de outro atributo não chave (transitiva). Anomalias: inserção, exclusão e atualização (mudar o mesmo dado em várias linhas).**

---

## Questão 32 · ❌ Não sabia ("?")

O Analista de Sistemas está iniciando o projeto de um novo sistema de gestão de Atos Normativos no Senado Federal. A primeira fase da Modelagem de Dados exige uma representação de alto nível das entidades, seus atributos e seus relacionamentos, livre de detalhes físicos ou de implementação.

Assinale a opção que apresenta o nível de modelagem de dados da arquitetura ANSI/SPARC responsável por fornecer uma visão completa das entidades e relacionamentos do negócio, com foco na semântica e no entendimento dos *stakeholders* e o diagrama UML que é frequentemente utilizado para essa finalidade.

(A) Nível Externo; Diagrama de Sequência.

(B) Nível Físico; Diagrama de Componentes.

\(C) Nível Lógico; Diagrama de Atividades.

✅ **(D) Nível Conceitual; Diagrama de Classes.**

(E) Nível Lógico; Diagrama de Casos de Uso. ← sua resposta (com pontinho)

**Depende de:** modelagem de dados (Semana 4) + UML.

**Por que errou:** "alto nível", "livre de detalhes de implementação", "semântica do negócio" = nível **conceitual**. O lógico já escolhe o modelo (tabelas, chaves). E o diagrama UML que mostra entidades, atributos e relacionamentos é o de **classes**; casos de uso mostram atores e funcionalidades, não dados.

📌 **Conceitual = entidades e relacionamentos do negócio, sem tecnologia (DER ou diagrama de classes) · lógico = tabelas, chaves, tipos do modelo relacional · físico = índices, armazenamento, SGBD. ANSI/SPARC: externo (visão de cada usuário), conceitual (o banco inteiro) e interno (físico).**

---

## Questão 33 · ✅ Acertou, mas com "?" (chute)

A equipe de desenvolvimento precisa criar um mecanismo para garantir que o sistema de *cache* de documentos legislativos tenha apenas uma única instância ativa em toda a aplicação, de modo que todas as requisições acessem o mesmo recurso compartilhado, evitando inconsistência de dados.

O Padrão de Projeto da classificação GoF mais apropriado para resolver esse problema, restringindo a instanciação de uma classe a um único objeto, é o(a)

(A) *Factory Method*

(B) *Builder*

\(C) *Observer*

✅ **(D) *Singleton*** ← sua resposta

(E) *Strategy*

**Depende de:** padrões GoF (Semana 3, ainda na fila).

**O que faltou para ser firme:** você sublinhou "única instância" e marcou certo; o "?" mostra que o nome do padrão ainda não está seguro. "Uma única instância" + "ponto global de acesso" = **Singleton** (criacional). É a definição literal: quando o GoF for estudado, esta vira questão de 20 segundos.

📌 **Singleton = uma única instância e um ponto global de acesso a ela (criacional). Factory Method = subclasse decide qual objeto criar · Builder = monta objeto complexo passo a passo · Observer = notifica dependentes · Strategy = troca o algoritmo.**

---

## Questão 34 · ❌ Não sabia ("?")

O sistema do Legislativo Federal precisa disponibilizar um serviço de consulta de projetos de lei para sistemas estaduais, garantindo que a descrição da interface, os tipos de dados e os métodos disponíveis sejam formalmente definidos e compreendidos por qualquer consumidor externo.

O padrão/documento da arquitetura de Web Services baseada em SOAP que é utilizado para descrever a interface e as capacidades operacionais de um Web Service de maneira legível por máquina é o

(A) SOAP

✅ **(B) WSDL**

\(C) UDDI

(D) REST

(E) XML ← sua resposta

**Depende de:** SOA e web services (Semana 6 do plano).

**Por que errou:** assunto ainda não estudado. A pista é o verbo "**descrever** a interface": WSDL = Web Services **Description** Language. XML é só o formato em que o WSDL e o SOAP são escritos.

📌 **SOAP = protocolo das mensagens (envelope XML) · WSDL = contrato que DESCREVE o serviço (operações, tipos, endereço) · UDDI = catálogo para PUBLICAR e DESCOBRIR serviços · REST = estilo de arquitetura sobre HTTP, não usa WSDL.**

---

## Questão 35 · ✅ Acertou

Um Analista de Sistemas está avaliando o desempenho de um servidor para um novo sistema de votação eletrônica da Assembleia Legislativa. A velocidade de processamento das instruções é um fator de forte relevância para o andamento do trabalho.

Para suprir essa necessidade, o componente do *hardware* de um computador que é o principal responsável por executar as instruções dos programas e realizar os cálculos lógicos e aritméticos é a(o)

(A) Memória RAM (*Random Access Memory*).

(B) Unidade de *Input/Output* (I/O).

\(C) Barramento de Dados (*Data Bus*).

✅ **(D) Unidade Central de Processamento (CPU).** ← sua resposta

(E) Disco Rígido (*Hard Disk Drive* - HDD).

**Confirmação:** acerto firme ("FÁCIL"). Executar instruções (unidade de controle) e fazer cálculos lógicos e aritméticos (ULA) = CPU.

📌 **CPU = unidade de controle (busca e decodifica a instrução) + ULA (cálculos lógicos e aritméticos) + registradores.**

---

## Questão 36 · ❌ Errou (com dúvida) · riscou a certa

Ao analisar a arquitetura de Von Neumann, o Analista observa que a eficiência do sistema depende da capacidade da CPU acessar rapidamente tanto as instruções quanto os dados.

A característica fundamental da arquitetura de Von Neumann que representa o principal gargalo de desempenho (o *bottleneck*) observado em sistemas modernos de computação é

(A) o uso de registradores de propósito geral.

(B) a divisão do processador em Unidade de Controle e Unidade Lógica Aritmética.

\(C) a representação de dados em formato binário.

✅ **(D) o compartilhamento de um único barramento entre a memória de instruções e a memória de dados.**

(E) a capacidade de realizar operações de ponto flutuante. ← sua resposta (com pontinho)

**Depende de:** arquitetura de computadores (Fundamentos de TI, parte comum; ⚪ na Semana 10 do plano).

**Por que errou:** você pôs pontinho em B e E e X em C e D. O enunciado dá a pista: a CPU precisa "acessar rapidamente **tanto as instruções quanto os dados**". Em Von Neumann, os dois ficam na **mesma memória** e passam pelo **mesmo caminho** até a CPU; como a CPU é muito mais rápida que esse tráfego, ela fica esperando. Esse é o "gargalo de Von Neumann". Ponto flutuante não tem relação com a arquitetura.

📌 **Von Neumann = programa armazenado: instruções e dados na mesma memória, pelo mesmo barramento → gargalo entre CPU e memória. Harvard = memórias e barramentos separados para instruções e dados.**

---

## Questão 37 · ✅ Acertou

Uma impressora laser foi conectada a um computador para imprimir relatórios de prestação de contas. A impressora aguarda os dados de impressão, vindos do sistema.

No modelo básico de organização do computador, a impressora é classificada como

(A) Armazenamento Volátil.

(B) Unidade Central de Processamento.

✅ **\(C) Saída (*Output*).** ← sua resposta

(D) Entrada (*Input*).

(E) Memória Cache.

**Confirmação:** acerto firme. A impressora **recebe** dados do computador e os entrega ao mundo externo: dispositivo de saída.

📌 **Entrada = leva dados para o computador (teclado, scanner) · saída = traz dados do computador (monitor, impressora) · multifuncional e tela sensível ao toque = entrada e saída.**

---

## Questão 38 · ❌ Não sabia ("?") · riscou a certa

Um programa em *Assembly* está realizando uma operação de soma de dois números inteiros de 8 bits sem sinal: 10100101₂ e 01100010₂.

O resultado binário da soma dos números inteiros e a condição de *overflow* ou *carry* observada em um registrador de 8 bits são:

(A) 00000011₂; *Overflow*.

(B) 11000111₂; Sem *overflow*. ← sua resposta

✅ **\(C) 00000111₂; *Carry* de 1.**

(D) 11000111₂; *Carry* de 1.

(E) 10000111₂; *Overflow*.

**Depende de:** arquitetura de computadores: aritmética binária (parte comum; ⚪ na Semana 10).

**Por que errou:** a soma na sua margem ficou com um dígito a menos (10000111). Coluna por coluna, da direita para a esquerda: 1+0=1 · 0+1=1 · 1+0=1 · 0+0=0 · 0+0=0 · 1+1=**0, vai 1** · 0+1+1=**0, vai 1** · 1+0+1=**0, vai 1**. Resultado: **1 0000 0111** (9 bits). No registrador de 8 bits ficam os 8 da direita, **00000111**, e o 9º bit é o **carry**. Conferência em decimal: 165 + 98 = 263, que passa de 255 (o máximo em 8 bits sem sinal); 263 − 256 = 7 = 00000111. Você riscou a (C), mas a (B) nem batia com a sua própria conta.

📌 **Sem sinal: estourou os n bits = CARRY (o bit que sobra). Com sinal (complemento de dois): resultado com sinal impossível = OVERFLOW. Conferir a soma binária em decimal: 8 bits sem sinal vão de 0 a 255.**

---

## Questão 39 · ❌ Não sabia ("?")

O Analista está debugando uma falha em que a soma de dois números inteiros positivos de 16 bits usando o complemento de dois resulta em um número inesperadamente negativo.

A ocorrência de um resultado negativo ao somar dois números positivos (ou um resultado positivo ao somar dois negativos) em sistemas de Complemento de Dois é um sintoma direto da condição de

(A) *Underflow* (Subfluxo).

(B) *Carry Out* (Vai um para fora do MSB).

✅ **\(C) Aritmética de *Overflow*.**

(D) *Sign Extension* (Extensão de Sinal).

(E) Erro de Ponto Flutuante. ← sua resposta

**Depende de:** arquitetura de computadores: complemento de dois (parte comum; ⚪ na Semana 10).

**Por que errou:** é o par da Q38. Em complemento de dois, o bit mais à esquerda é o **sinal**. Se positivo + positivo dá negativo, o resultado não coube nos bits e "invadiu" o bit de sinal: **overflow aritmético**. O enunciado fala em **inteiros**, então ponto flutuante (E) está fora.

📌 **Complemento de dois: positivo + positivo = negativo (ou negativo + negativo = positivo) → overflow. Soma de sinais diferentes nunca dá overflow. Carry é o conceito para números SEM sinal.**

---

## Questão 40 · ❌ Não sabia ("?") · ver observação

Um número é representado no sistema octal como 17₈. O Analista precisa converter esse número para o sistema binário para entender sua representação na memória.

A representação binária correta do número 17₈ é

(A) 10001₂

(B) 01111₂ ← sua resposta (só no cartão)

\(C) 10111₂

(D) 11111₂

✅ **(E) 001111₂**

**Depende de:** arquitetura de computadores: bases numéricas (parte comum; ⚪ na Semana 10). Você anotou: "estudei na facu e não lembro".

**Como resolver:** cada dígito **octal** vira **3 bits**: 1 → 001 e 7 → 111. Juntando: **001 111**. Em decimal, 17₈ = 1 × 8 + 7 = 15.

**Observação honesta:** a sua alternativa, 01111₂, **também vale 15**: é o mesmo número com um zero à esquerda a menos. A banca manteve a (E) no gabarito definitivo, pela conversão dígito a dígito em grupos de 3 bits. Então, pelo gabarito é erro, mas pelo valor a sua resposta não está errada. Na prova, quando duas alternativas tiverem o mesmo valor, marque a que tem o **formato do método** (grupos de 3 para octal, de 4 para hexadecimal).

📌 **Octal → binário: 3 bits por dígito (0 = 000 … 7 = 111). Hexadecimal → binário: 4 bits por dígito. Binário → octal: agrupar de 3 em 3 a partir da direita.**

---

## Questão 41 · ❌ Não sabia ("?")

O Analista está utilizando Python para um *script* de automação de relatórios. Ele nota que o código é executado linha por linha, sem a necessidade de uma etapa de construção prévia.

O processo de execução de códigos de linguagem de programação que são lidos e executados diretamente, sem a geração de código de máquina intermediário ou otimizado, é a

(A) Compilação ← sua resposta (com pontinho)

(B) Ligação (*Linking*)

✅ **\(C) Interpretação**

(D) Geração de Código Objeto

(E) Análise Sintática (*Parsing*)

**Depende de:** fundamentos de linguagens de programação (parte comum; base para a Semana 8).

**Por que errou:** você sublinhou "linha por linha" e "construção prévia" e marcou o contrário. **Compilar** é justamente a "etapa de construção prévia": traduz o programa inteiro antes e gera um executável. **Interpretar** é ler e executar direto, sem gerar esse executável. O enunciado diz "**sem** a necessidade de uma etapa de construção prévia": isso elimina a (A).

📌 **Compilação = traduz tudo antes, gera executável (C, Go). Interpretação = lê e executa direto, linha a linha (Python, JavaScript). Ligação (linking) = junta os módulos compilados. Atenção ao "sem" do enunciado: ele descreve o que a resposta NÃO é.**

---

## Questão 42 · ❌ Não sabia ("?")

Em uma linguagem procedural como Pascal ou C, o Analista precisa estruturar um bloco de código que realize uma tarefa específica e que não retorne explicitamente um valor para o ponto de chamada, mas pode alterar variáveis globais ou realizar operações de E/S.

O termo usado para designar esse bloco de código que executa uma sequência de comandos, mas que não retorna um valor, é

(A) Função (*Function*).

(B) Módulo (*Module*).

\(C) Classe (*Class*).

✅ **(D) Procedimento (*Procedure*).**

(E) *Subroutine* (Sub-rotina). ← sua resposta (com pontinho)

**Depende de:** fundamentos de programação (parte comum).

**Por que errou:** você riscou "Função" corretamente (função **retorna** valor) e ficou com o termo genérico. **Sub-rotina** é o nome geral de qualquer bloco chamável, e abrange os dois tipos. O nome específico do bloco que **não retorna valor** é **procedimento** (em Pascal, `procedure`; em C, função `void`).

📌 **Sub-rotina = gênero. Função = retorna valor · procedimento = não retorna valor (executa comandos, pode alterar variáveis globais e fazer E/S).**

---

## Questão 43 · ✅ Acertou

Em uma linguagem que suporta passagem de parâmetros por referência, uma função `troca(a, b)` é chamada. O Analista observa que após a execução da função, os valores das variáveis originais x e y (passadas como a e b) são alterados.

Assinale a afirmativa correta a respeito do mecanismo exato da passagem por referência que permite à função alterar o valor da variável original (x ou y) no escopo do chamador.

(A) A função cria cópias temporárias dos valores de x e y e os retorna após a execução.

(B) O compilador duplica as variáveis x e y na *stack* de chamada da função.

✅ **\(C) A função recebe o endereço de memória das variáveis originais e opera diretamente sobre o local de armazenamento delas.** ← sua resposta

(D) O valor de retorno da função é atribuído automaticamente às variáveis de entrada x e y.

(E) A função utiliza variáveis globais para simular a alteração dos parâmetros.

**Confirmação:** acerto firme, com D e E riscadas. Por referência = a função recebe o **endereço** e mexe na variável original. (A) e (B) descrevem passagem por **valor** (cópia).

📌 **Por valor = recebe uma cópia; a original não muda. Por referência = recebe o endereço; a original muda.**

---

## Questão 44 · ✅ Acertou

Para inicializar o *hardware* de um computador e carregar o sistema operacional, é necessário um *software* básico residente em uma memória não volátil.

Assinale o tipo de memória que armazena o *firmware* inicial que é lido, mas que raramente é alterado.

(A) Memória RAM

(B) Memória Cache

\(C) Registradores

✅ **(D) Memória ROM** ← sua resposta

(E) SSD

**Confirmação:** acerto firme, com as outras quatro riscadas. Firmware de inicialização (BIOS/UEFI) fica em memória **não volátil** de leitura: ROM (hoje, memória flash regravável). RAM, cache e registradores são voláteis.

📌 **ROM = não volátil, guarda o firmware de boot (BIOS/UEFI). RAM, cache e registradores = voláteis (perdem o conteúdo sem energia). Hierarquia por velocidade: registradores > cache > RAM > SSD/HD.**

---

## Questão 45 · ❌ Errou (com dúvida) · fora do edital

Um Analista de Sistemas está desenvolvendo o modelo lógico de um banco de dados e precisa representar a relação de identificação entre a entidade DEPARTAMENTO e a entidade FUNCIONARIO_DEPENDENTE.

Na notação IDEF1X, assinale a afirmativa correta sobre o modo como é representada graficamente a entidade FUNCIONARIO_DEPENDENTE em relação à entidade DEPARTAMENTO, indicando que a chave primária de DEPARTAMENTO se torna parte da chave primária de FUNCIONARIO_DEPENDENTE.

(A) O relacionamento é desenhado com uma linha tracejada.

(B) A entidade FUNCIONARIO_DEPENDENTE possui cantos arredondados.

\(C) O relacionamento é desenhado com um ponto de interrogação na ponta.

✅ **(D) O relacionamento é desenhado com uma linha sólida.**

(E) O relacionamento é desenhado com um diamante. ← sua resposta (com pontinho)

**Fora do edital:** a notação IDEF1X não aparece no Anexo I do TJPB (nem no Cargo 5, nem na parte comum). **Só registro: não estudar.**

**Para constar:** em IDEF1X, relacionamento **identificador** (a chave do pai entra na chave do filho) = linha **sólida**; não identificador = linha **tracejada**. O diamante (losango) é da notação de Chen. Detalhe: a (B) também descreve algo verdadeiro em IDEF1X (entidade dependente tem cantos arredondados); a banca ficou com a linha sólida, que é a representação do relacionamento.

---

## Questão 46 · ❌ Errou (com dúvida)

Ao designar um banco de dados para gerenciar Atos Legais, o Analista precisa garantir que cada PARECER emitido esteja sempre associado a um ATO_LEGAL existente, e que não seja possível excluir um ATO_LEGAL se houver PARECERES vinculados a ele.

A regra fundamental do Modelo Relacional que é implementada para garantir que os valores das chaves estrangeiras (PARECER.ID_Ato) sempre correspondam a valores válidos na chave primária da tabela referenciada (ATO_LEGAL.ID_Ato) é a

(A) Integridade de Entidade. ← sua resposta (com pontinho)

✅ **(B) Integridade Referencial.**

\(C) Integridade de Domínio.

(D) Integridade Transacional.

(E) Integridade Semântica.

**Depende de:** modelo relacional: restrições de integridade (Semana 4: é o assunto desta semana).

**Por que errou:** o enunciado entrega a definição: "chaves **estrangeiras** sempre correspondam a valores válidos na chave primária da tabela **referenciada**". Chave estrangeira que **referencia** = integridade **referencial**. Integridade de **entidade** fala da própria tabela: a chave primária não pode ser nula nem repetida. É a mesma regra do ON DELETE do Simulado 01 (Q53): "não excluir o pai com filhos" é o RESTRICT da chave estrangeira.

📌 **Integridade de entidade = PK única e não nula · referencial = toda FK aponta para uma PK existente (ou é nula) · de domínio = o valor respeita o tipo e as regras da coluna. Palavra "estrangeira" ou "referenciada" = referencial.**

---

## Questão 47 · ✅ Acertou

O Analista precisa adicionar um novo registro de ASSESSOR ao banco de dados do Gabinete, informando apenas o seu nome (`Maria Souza`) e a matrícula (9876).

O comando SQL mais adequado para realizar a inserção desse novo registro na tabela ASSESSOR é:

(A) UPDATE ASSESSOR SET Nome = 'Maria Souza', Matricula = 9876.

(B) SELECT * INTO ASSESSOR VALUES ('Maria Souza', 9876).

\(C) ALTER TABLE ASSESSOR ADD ('Maria Souza', 9876).

(D) INSERT NEW ASSESSOR ('Maria Souza', 9876).

✅ **(E) INSERT INTO ASSESSOR (Nome, Matricula) VALUES ('Maria Souza', 9876).** ← sua resposta

**Confirmação:** acerto firme, com A, B e C riscadas. Inserir linha = `INSERT INTO tabela (colunas) VALUES (valores)`. UPDATE altera linhas que já existem; ALTER TABLE muda a **estrutura** (DDL); `INSERT NEW` não existe.

📌 **DML: INSERT INTO … VALUES (nova linha) · UPDATE … SET … WHERE (altera linha) · DELETE FROM … WHERE (apaga linha). DDL: CREATE, ALTER, DROP (estrutura). Listar as colunas quando só algumas são informadas.**

---

## Questão 48 · ❌ Não sabia ("?") · fora do edital

A Assembleia Legislativa está buscando aprimorar seus processos de desenvolvimento e manutenção de sistemas críticos, como o portal de transparência e o sistema de protocolo eletrônico. A liderança de TI decidiu adotar um modelo de maturidade para medir e melhorar a capacidade de seus processos de engenharia de software, visando maior previsibilidade, eficiência e qualidade do produto.

Ao aplicar modelos de avaliação de maturidade de processos de software, como o CMMI ou o MPS.BR, o nível de maturidade caracterizado pela medição quantitativa e pelo controle estatístico dos processos é o

(A) Nível 1 – Inicial ← sua resposta

(B) Nível 2 – Gerenciado

\(C) Nível 3 – Definido

✅ **(D) Nível 4 – Gerenciado Quantitativamente**

(E) Nível 5 – Otimizando

**Fora do edital:** CMMI e MPS.BR não aparecem no Anexo I do TJPB (a parte comum cita COBIT 2019 e ITIL 4). **Só registro: não estudar.**

**Para constar:** a resposta estava no próprio nome ("medição **quantitativa**" → "Gerenciado **Quantitativamente**"). Mesmo sem conhecer o modelo, dava para acertar casando a palavra do enunciado com a da alternativa.

---

## Questão 49 · ✅ Acertou

O Analista de Sistemas precisa estimar o esforço e o custo de um novo módulo de *software* usando uma métrica independente de linguagem de programação.

A seguinte métrica de tamanho de *software* é baseada na funcionalidade entregue ao usuário, sendo independente da linguagem de implementação:

(A) Linhas de Código (*Lines of Code* - LOC).

(B) Complexidade Ciclomática.

✅ **\(C) Ponto de Função (*Function Point* - FP).** ← sua resposta

(D) *Effort* (Esforço, em *Person-Months*).

(E) *Bugs* por Módulo.

**Depende de:** APF (**estudada nas Semanas 1 e 2**).

**Confirmação:** acerto firme. É a mesma regra que você errou no Simulado 01 (Q27, PF × story points) e agora acertou sem dúvida: ponto de função mede a **funcionalidade pela visão do usuário**, independente de tecnologia e de linguagem. LOC depende da linguagem; esforço é resultado da estimativa, não medida de tamanho.

📌 **Ponto de função = tamanho funcional, pela visão do usuário, independente de linguagem, tecnologia e time. LOC = depende da linguagem.**

---

## Questão 50 · ❌ Errou (com dúvida)

A alta administração de um órgão público determinou que o risco de vazamento de dados de um novo sistema deve ser reduzido a um nível aceitável, mas que ainda assim permitirá a continuidade da operação. Após a avaliação, o risco residual foi considerado alto, exigindo a implementação de novos controles.

O tratamento de risco decidido pela alta administração do órgão é

(A) Aceitar o Risco

(B) Reter o Risco

\(C) Evitar o Risco ← sua resposta (com pontinho)

(D) Compartilhar o Risco

✅ **(E) Modificar o Risco**

**Depende de:** gestão de riscos, ISO/IEC 27005 (parte comum; Semana 11 do plano).

**Por que errou:** no dia a dia, "evitar o risco" soa como "diminuir o risco". Na norma, **evitar** é **abandonar a atividade** que gera o risco (não lançar o sistema). O enunciado diz que o risco deve ser "**reduzido**" e que a operação **continua**, com "**novos controles**": isso é **modificar** (também chamado de mitigar ou reduzir).

📌 **ISO 27005, quatro tratamentos: MODIFICAR (reduzir com controles) · RETER (aceitar conscientemente) · EVITAR (desistir da atividade) · COMPARTILHAR (seguro, terceirização). "Reduzir" + "implementar controles" + "a operação continua" = modificar.**

---

## Questão 51 · ❌ Não sabia ("?")

Ao realizar uma análise de riscos, um analista identificou que a vulnerabilidade de *Cross-Site Scripting* em um portal de serviços tem uma probabilidade de ocorrência classificada como *média* e um impacto potencial classificado como *Alto*. A organização utiliza uma matriz de riscos 5X5 (Muito Baixa, Baixa, Média, Alta, Muito Alta). Para tratar este risco, foi implementado um WAF, que reduz a probabilidade de exploração de *Média* para *Baixa*.

Considerando a abordagem da ISO/IEC 27005, o termo técnico para o risco após a implementação do WAF e antes da decisão final de aceitação ou tratamento adicional é

(A) Risco Inerente

(B) Risco Bruto

\(C) Risco Aceitável ← sua resposta

✅ **(D) Risco Residual**

(E) Risco Mitigado

**Depende de:** gestão de riscos, ISO/IEC 27005 (parte comum; Semana 11).

**Por que errou:** o risco que **sobra depois do tratamento** é o **residual**. "Aceitável" é um **julgamento** que vem depois (o enunciado diz "antes da decisão final de aceitação"). A questão anterior (Q50) usou o termo no próprio enunciado: "o risco **residual** foi considerado alto". Vale olhar as questões vizinhas do mesmo assunto: às vezes uma entrega o vocabulário da outra.

📌 **Risco inerente (ou bruto) = antes dos controles · risco residual = o que resta depois do tratamento · depois a direção decide se o residual é aceitável (aceitação do risco).**

---

## Questão 52 · ✅ Acertou (com dúvida)

Um sistema de controle de acesso lógico da Assembleia Legislativa de Rondônia utiliza um modelo onde os direitos de acesso de um usuário a um recurso são concedidos com base em sua função ou cargo dentro da organização. Este modelo simplifica a administração e garante que as permissões estejam alinhadas com as responsabilidades de cada função ou cargo.

Esse modelo de controle de acesso lógico é o

✅ **(A) Controle de Acesso Baseado em Papéis (*Role-Based Access Control* - RBAC)** ← sua resposta

(B) Controle de Acesso Obrigatório (*Mandatory Access Control* - MAC)

\(C) Controle de Acesso Discricionário (*Discretionary Access Control* - DAC)

(D) Controle de Acesso Baseado em Atributos (*Attribute-Based Access Control* - ABAC)

(E) Controle de Acesso Orientado a Tarefas (*Task-Based Access Control* - TBAC)

**Depende de:** controle de acesso (regra registrada em 09/11, depois do erro na Q42 do Simulado 01).

**Confirmação:** você errou este assunto no Simulado 01 e agora acertou, ficando em dúvida só com o ABAC. "Função ou cargo" = papel = **RBAC**. O ABAC decide por **atributos** combinados (do usuário, do recurso, do horário, do local), não só pelo cargo.

📌 **Pelo cargo/função = RBAC · por rótulo e habilitação = MAC · o dono decide = DAC · por atributos e contexto (hora, local, tipo de dado) = ABAC.**

---

## Questão 53 · ❌ Não sabia ("?")

Após uma análise de impacto no negócio (*Business Impact Analysis* - BIA), identificou-se que um sistema de emissão de certidões governamentais não pode ficar indisponível por mais de 8 horas, e que, após a recuperação, a perda máxima de dados aceitável é de 4 horas.

As métricas do Plano de Continuidade de Negócio (PCN) que foram estabelecidas por essas restrições, respectivamente, são:

(A) *Recovery Time Objective* (RTO) e *Maximum Tolerable Downtime* (MTD).

(B) *Maximum Tolerable Downtime* (MTD) e *Recovery Point Objective* (RPO).

✅ **\(C) *Recovery Time Objective* (RTO) e *Recovery Point Objective* (RPO).**

(D) *Work Recovery Time* (WRT) e *Maximum Data Loss* (MDL). ← sua resposta

(E) *Recovery Point Objective* (RPO) e *Recovery Time Objective* (RTO).

**Depende de:** continuidade de negócios (parte comum; Semana 11).

**Por que errou:** assunto ainda não estudado. São duas siglas que caem sempre juntas. **RTO** = quanto **tempo** o sistema pode ficar parado até voltar (8 h). **RPO** = até que **ponto** no passado se aceita perder dados (4 h; define a frequência do backup). "Respectivamente" pede a ordem: tempo primeiro, dados depois; a (E) inverte.

📌 **RTO = Time = tempo máximo para voltar a operar. RPO = Point = perda máxima de dados (distância até o último backup). Com "respectivamente", conferir a ordem.**

---

## Questão 54 · ✅ Acertou (com dúvida)

Em um ambiente de Tecnologia da Informação, o princípio da Segregação de Funções (SoD - *Separation of Duties*) é rigorosamente aplicado. Um Analista de Sistemas é designado para desenvolver e testar novas funcionalidades em um sistema de missão crítica. Conforme a política de segurança, esse mesmo analista não possui permissão para realizar a implementação (*deployment*) do código final no ambiente de produção.

O seguinte risco ou ameaça de segurança e governança o princípio da Segregação de Funções é projetado primariamente para mitigar o problema nesse cenário específico:

(A) Risco de *Phishing* e engenharia social.

(B) Risco de ataques de Negação de Serviço (DoS).

✅ **\(C) Risco de conluio e fraude interna.** ← sua resposta

(D) Risco de indisponibilidade por falha de hardware.

(E) Risco de exploração de vulnerabilidades de *Zero-Day*.

**Confirmação:** você eliminou A, D e E e marcou certo. Segregar funções é impedir que **uma pessoa sozinha** execute todo um processo crítico (desenvolver, testar e publicar): reduz o risco de fraude e de erro interno, porque exige a participação de mais alguém.

📌 **Segregação de funções = ninguém faz o processo crítico inteiro sozinho → combate fraude e erro interno. Quem desenvolve não publica em produção.**

---

## Questão 55 · ✅ Acertou

Na gestão de ativos de informação, o conceito de *Asset Owner*, conforme a ISO/IEC 27002, é fundamental para a governança.

A principal responsabilidade do Proprietário do Ativo é

(A) ser o responsável financeiro pelo ativo.

(B) realizar o *backup* diário do ativo.

✅ **\(C) definir os requisitos de segurança e a classificação do ativo.** ← sua resposta

(D) monitorar e analisar os logs de acesso ao ativo.

(E) desenvolver o código-fonte do sistema que gerencia o ativo.

**Confirmação:** acerto firme. O proprietário **responde** pelo ativo: classifica a informação e define quem pode acessá-la e com que proteção. Backup e logs são tarefas operacionais do **custodiante** (em geral, a TI).

📌 **Proprietário do ativo = classifica e define os requisitos de proteção (responde pelo ativo). Custodiante = opera os controles (backup, logs).**

---

## Questão 56 · ❌ Errou (convicto)

O sistema de inicialização e gerenciamento de serviços padrão no CentOS 7 é o `systemd`. Um administrador de sistemas precisa tornar inativo o serviço HTTPD (Apache) para que ele não inicie automaticamente após a reinicialização do sistema, mas precisa mantê-lo instalado.

O comando *systemctl* correto para realizar essa ação é

(A) *systemctl stop httpd*

✅ **(B) *systemctl disable httpd***

\(C) *systemctl mask httpd*

(D) *systemctl kill httpd*

(E) *systemctl remove httpd* ← sua resposta

**Depende de:** sistemas operacionais (parte comum; Semana 10). **Limítrofe:** administração de Linux em detalhe é do cargo de Infraestrutura; no seu, o edital traz só "Sistemas operacionais".

**Por que errou:** você sublinhou "mantê-lo instalado" e marcou justamente "**remove**", que é a única que contradiz o enunciado (e nem existe no `systemctl`). Você riscou A, C e D e não riscou a (B): a resposta ficou sem análise. É o caso da regra de 09/11: procurar no enunciado a palavra que contradiz a alternativa.

📌 **systemctl: start/stop = liga ou desliga AGORA · enable/disable = inicia ou não NO BOOT · mask = bloqueia qualquer início. "Não iniciar automaticamente após reiniciar" = disable.**

---

## Questão 57 · ✅ Acertou

Um Analista de Sistemas está desenvolvendo um Plano de Testes. Ele utiliza o Diagrama de Casos de Uso para identificar os cenários de teste de nível de sistema e o Diagrama de Objetos para verificar a configuração de dados antes e depois da execução de um caso de uso.

A principal vantagem de se usar o Diagrama de Objetos em conjunto com um Caso de Uso para a validação do sistema reside no fato de que o Diagrama de Objetos

(A) valida a arquitetura física do servidor onde o Caso de Uso será executado.

(B) permite modelar o fluxo de mensagens entre as classes, detalhando a implementação do Caso de Uso.

\(C) fornece uma representação concreta das classes, verificando se a estrutura estática é válida.

✅ **(D) permite visualizar os valores específicos dos atributos das instâncias envolvidas, confirmando o estado do sistema em um ponto de execução do Caso de Uso.** ← sua resposta

(E) serve como base para a criação do banco de dados, sendo irrelevante para testes.

**Confirmação:** acerto firme, com A, B e E riscadas. Diagrama de objetos = "fotografia" das **instâncias** e dos **valores** dos atributos em um momento. (B) é diagrama de sequência; (A) é diagrama de implantação.

📌 **Diagrama de classes = os tipos (estrutura). Diagrama de objetos = instâncias com valores em um instante (foto do sistema).**

---

## Questão 58 · ❌ Errou (convicto) · limítrofe

Um Analista de Arquitetura está avaliando a adoção de um *framework* para estruturar a visão da arquitetura corporativa de uma organização pública. Ele precisa de um modelo que não apenas catalogue os ativos existentes, mas que também forneça um conjunto de *views* e *viewpoints*, permitindo que a arquitetura seja descrita sob perspectivas de diferentes *stakeholders*.

Assinale a opção que apresenta o *framework* de arquitetura corporativa mais adequado para atender esse requisito de múltiplas visões estruturadas e a sua principal característica de organização conceitual.

(A) TOGAF; A principal característica é o *Architecture Development Method*, um método iterativo.

✅ **(B) Zachman Framework; A principal característica é a classificação das perspectivas arquiteturais em uma matriz 6 X 6.**

\(C) DoDAF; A principal característica é o foco na interoperabilidade e nas especificações militares.

(D) ISO/IEC/IEEE 42010; A principal característica é o padrão que define os conceitos de *view* e *viewpoint*, mas não fornece um método ou conteúdo específico. ← sua resposta

(E) Gartner Framework; A principal característica é o foco na medição do valor de negócio da arquitetura.

**Depende de:** frameworks de arquitetura corporativa. **Limítrofe:** o edital do Cargo 5 fala em "padrões de arquitetura corporativa", sem citar Zachman nem TOGAF. Baixa prioridade.

**Por que errou:** a sua escolha tem lógica: a ISO 42010 realmente é a norma que **define** *view* e *viewpoint*. Mas o enunciado pede um **framework** que "catalogue" e "forneça um conjunto" de visões por *stakeholder*, e a própria (D) diz que a norma "não fornece método ou conteúdo específico". Quem entrega as visões prontas, organizadas por perspectiva, é o **Zachman** (uma matriz de 6 perspectivas × 6 perguntas).

📌 **Zachman = matriz 6 × 6 (perspectivas × o quê, como, onde, quem, quando, por quê): classifica, não tem método. TOGAF = método ADM, iterativo. ISO 42010 = norma que define os conceitos de descrição de arquitetura (view, viewpoint).**

---

## Questão 59 · ❌ Não sabia ("?")

Uma aplicação web crítica de um órgão público opera em um *cluster* de servidores. O Balanceador de Carga está configurado para utilizar o algoritmo *Round Robin* ponderado e ativado o recurso de Afinidade de Sessão.

A principal **desvantagem** ou **risco** da utilização da Afinidade de Sessão em termos de escalabilidade e tolerância a falhas, é que ela

(A) impede a distribuição uniforme da carga, resultando em um subaproveitamento de alguns servidores.

(B) elimina a necessidade de *firewalls* de aplicação nos nós do *cluster*.

\(C) aumenta a latência das requisições, pois exige múltiplas consultas ao banco de dados de sessão. ← sua resposta

✅ **(D) causa a perda de dados da sessão do usuário se o servidor específico falhar.**

(E) bloqueia a escalabilidade horizontal, impedindo a adição de novos nós ao *cluster*.

**Depende de:** balanceamento de carga e alta disponibilidade (System Design, Semana 7).

**Por que errou:** assunto ainda não estudado. Afinidade de sessão (*sticky session*) = o balanceador manda o **mesmo usuário sempre para o mesmo servidor**, porque a sessão fica na memória daquele servidor. Se ele cai, a sessão se perde: é o risco para a **tolerância a falhas**. A (C) descreve o contrário: banco de sessão compartilhado é a **alternativa** à afinidade (sessão fora do servidor, por exemplo no Redis). A (A) é um efeito real, mas menor; (E) exagera com "bloqueia" e "impedindo".

📌 **Afinidade de sessão (sticky) = mesmo usuário → mesmo servidor. Risco: o servidor cai e a sessão se perde. Solução: aplicação sem estado (stateless), com a sessão em cache distribuído (Redis). Cuidado com verbos absolutos: "bloqueia", "impede", "elimina".**

---

## Questão 60 · ✅ Acertou (com dúvida)

Em um projeto de alta complexidade e missão crítica como um sistema de tráfego aéreo, a equipe optou pelo Modelo Cascata de desenvolvimento. Após a conclusão das fases de Requisitos e Design, e com a Codificação em andamento, o cliente terá sua primeira oportunidade de Validação significativa apenas na fase de Testes, no final do ciclo

O principal risco arquitetônico e de custo introduzido pela natureza *late-feedback* do Modelo Cascata nesse cenário é

(A) o risco de crescimento descontrolado do escopo (*scope creep*) durante a fase de Manutenção devido ao baixo engajamento do cliente.

(B) a dificuldade em alocar desenvolvedores *sêniores* para a fase de Codificação devido à rigidez do cronograma sequencial.

\(C) a necessidade de produzir documentação excessiva, o que inevitavelmente introduz inconsistências no código.

✅ **(D) o risco de que erros fundamentais nos requisitos ou no design sejam descobertos somente na fase de validação, resultando em um custo de retrabalho exponencialmente maior.** ← sua resposta

(E) o aumento do *vendor lock-in* devido à dependência excessiva de ferramentas de design proprietárias.

**Depende de:** modelos de processo: cascata (**estudado na Semana 1**).

**Confirmação:** as outras quatro foram riscadas e você marcou certo. Cascata = feedback tardio: o erro de requisito só aparece no fim, quando corrigir custa muito mais.

📌 **Cascata: fases em sequência, cliente só valida no fim → erro de requisito descoberto tarde = retrabalho caro. Quanto mais tarde o defeito é achado, maior o custo da correção.**

---

## 4. Discursiva 01 · Estudo de caso (Scrum) · 15/40 (estimativa)

> **Questão autoral, no estilo FGV, não oficial.** Corrigida pelo espelho fechado de 04/11 (escrito antes da sua resposta), com rigor de banca. **A nota é estimativa:** o edital do TJPB não detalha os critérios de correção. Faixa provável: 14 a 17. Mínimo para não ser eliminado: 24.

**Nota por item**

| Item | O que o enunciado pediu | Pontos | Você |
|---|---|---|---|
| A | Três problemas, cada um fundamentado no Guia do Scrum | 12 | **7,0** |
| B | Por que a comparação é inadequada + o que são story points + uso correto da velocidade | 8 | **2,0** |
| C | Forma adequada + **exemplo** de história + critério de aceitação + **INVEST** | 9 | **2,0** |
| D | Encaminhamentos para qualidade e para acabar com as interferências | 8 | **2,5** |
| Geral | Linguagem, fluência, coerência, falar do caso, até 30 linhas | 3 | **1,5** |
| | **Total** | **40** | **15,0** |

**O que funcionou:** texto corrido em 4 parágrafos, 28 linhas, na ordem dos itens, letra legível, falando do caso (e não do Scrum em geral). No Simulado 01 a discursiva não saiu; agora você entregou um texto completo. A estrutura deixou de ser o problema: o que falta é **conteúdo específico**.

### Item A · 7/12

| Problema que você apontou | Avaliação | Pontos |
|---|---|---|
| Itens criados pelos desenvolvedores, sem critérios de aceitação | Citado. Fundamento parcial: disse que quem cria é o "Dono do Produto", mas no plural ("Donos") e com "apenas". No Guia, o Product Owner é **uma pessoa**, responsável por gerenciar o Product Backlog; ele pode delegar a escrita, mas continua responsável. Faltou dizer que a causa é o **PO ausente** | 2,5/4 |
| Daily com tempo estendido | Citado. Fundamento parcial: os 15 minutos estão certos, mas não é "recomendação", é o limite do evento. Faltou o principal do cenário: a Daily virou **prestação de contas ao coordenador**; ela é dos Developers, para inspecionar o progresso rumo à **Meta da Sprint** | 2,5/4 |
| Ausência da Definição de Pronto | Citado certo na linha 3. Na linha 8 virou "**Definition of Ready (DoD)**", e a explicação ("tarefas não planejadas corretamente") é de Definition of **Ready**. Termo técnico trocado anula o fundamento. Pronto = **Done**: compromisso do **Incremento** | 2,0/4 |

> No **rascunho** você escreveu "Definition of Done (DoD)" e explicou certo ("requisitos atendidos, testes executados"). Ao passar a limpo, trocou pelo termo errado. Na dúvida entre a sigla em inglês e o nome em português, use só o português: "Definição de Pronto".

Ficaram de fora dois problemas fortes do cenário: o coordenador **incluindo demandas direto no Sprint Backlog** (você só tratou disso no fim, como solução) e a velocidade usada como **avaliação de desempenho**. O comando pedia fundamento "no Guia do Scrum", e o Guia não foi citado nenhuma vez.

### Item B · 2/8

| Critério do espelho | Avaliação | Pontos |
|---|---|---|
| Story points = medida **relativa** de esforço, complexidade e incerteza, calibrada por equipe | Citou complexidade (certo), mas incluiu **tempo de execução**, impacto no sistema e **quantidade de pessoas**, que não entram. Não disse "relativa" | 0,5/2 |
| Escalas diferentes → números não comparáveis | Presente: "tais variáveis mudam de equipe para equipe" e "nem sempre a maior pontuação indica maior produtividade". Perdeu parte por concluir que indica "maior impacto ao cliente" (ponto não mede valor) | 1,5/2 |
| O que é velocidade e qual o **uso correto** (a própria equipe planejar e prever) | **Ausente.** O comando pedia isso com todas as letras | 0/2 |
| Efeito da cobrança: inflar as estimativas | Ausente | 0/2 |

> É o seu ponto fraco 5 (estimativa ágil), agora por escrito: story point **não é tempo**. A frase "A comparação entre velocidades e Story Points" também mistura as duas coisas: a comparação do caso é entre as **velocidades de duas equipes**.

### Item C · 2/9

| Critério do espelho | Avaliação | Pontos |
|---|---|---|
| História no formato "Como… quero… para…", com papel do contexto | Descreveu o formato, mas **não deu o exemplo** que o comando pediu ("apresentando um exemplo") | 1/3 |
| Critério de aceitação verificável | Explicou para que serve, sem escrever nenhum | 1/3 |
| Relação com o INVEST (pelo menos 2 características) | **Ausente.** A palavra INVEST não aparece no texto | 0/3 |

> Este era o item mais barato da prova: você acertou 13/15 no bloco de user stories e INVEST em 28/10. Uma história de duas linhas, um critério e duas letras do INVEST valiam 9 pontos.

### Item D · 2,5/8

| Encaminhamento | Avaliação | Pontos |
|---|---|---|
| Product Owner disponível, cuidando do backlog | Presente, mas pedindo o PO "nas daily". A Daily é dos Developers; o PO precisa estar disponível para a equipe, na Sprint Planning, na Review e no refinamento | 1,5/2 |
| Fim das interferências externas | Presente, mas genérico ("não interferência de outros setores"). Faltou o **como**: a demanda vai ao PO, entra no Product Backlog e não muda a Sprint em andamento | 1/2 |
| Criar a Definição de Pronto (testes, revisão) | Ausente como proposta | 0/2 |
| Scrum Master atuando (timebox, remover impedimentos, orientar a organização) | Ausente: o Scrum Master não aparece no texto | 0/2 |
| Parar de usar velocidade como métrica de desempenho | Ausente | 0/2 |

### Abordagem geral · 1,5/3

Texto organizado e sobre o caso. Perdeu por desvios de norma e por termos fora do Guia:

| Linha | Como está | Como fica |
|---|---|---|
| 6 | "Dailys detém como recomendação um tempo máximo" | "A Daily Scrum tem duração máxima de quinze minutos" |
| 7 | "manter atualizado apenas a situação" | "manter atualizada apenas a situação" |
| 9–10 | "o processo de sua realização imprecisa, mal executada e com ordem de prioridade afetados" | "o processo de sua realização impreciso, mal executado e com a ordem de prioridade afetada" |
| 14 | "É notório que tais variáveis mudem" | "É notório que tais variáveis mudam" |
| 15 | "onde nem sempre a maior pontuação" | "de modo que nem sempre…" ("onde" só para lugar) |
| 17 | "é necessário a presença do Product Owner" | "é necessária a presença" (com artigo, concorda: regra de 28/10, ponto fraco 1) |
| 21 | "também se destaca os critérios" | "também se destacam os critérios" |
| 16 e 28 | parágrafos sem ponto final | fechar com ponto |
| várias | "task", "feature", "P.O", "Donos do Produto" | "item do Product Backlog", "funcionalidade", "Product Owner" |

### Termos técnicos que faltaram

Guia do Scrum · Meta da Sprint · Sprint Backlog (pertence aos Developers) · Incremento · Definição de Pronto (Done) · Scrum Master · timebox · medida relativa · velocidade para planejamento e previsão · inflação de estimativas · INVEST (Independente, Negociável, Valiosa, Estimável, Pequena, Testável) · Dado/Quando/Então · refinamento do Product Backlog.

### Por que a nota ficou em 15: o método

O conteúdo você tem (os blocos de Scrum e de user stories foram bons). O que faltou foi **responder ao que cada comando pede**. Somando os quatro itens, o enunciado pedia cerca de 15 entregas (problemas, fundamentos, definições, exemplo, critério, INVEST, encaminhamentos); o texto atendeu por inteiro a poucas delas.

📌 **Antes do rascunho, transformar cada item em lista de entregas, com o número ao lado: "A: 3 problemas + 3 fundamentos do Guia", "B: por que não compara + o que é story point + uso certo da velocidade", "C: 1 história + 1 critério + 2 letras do INVEST", "D: 4 encaminhamentos". Cada entrega vira uma frase. Só passar a limpo depois de riscar todas da lista.**

📌 **"Apresente um exemplo" = escrever o exemplo. Descrever o formato não pontua como exemplo.**

### Versão melhorada (cabe em 30 linhas)

> O cenário revela três desvios em relação ao Guia do Scrum. Primeiro, o Product Owner não exerce o papel: segundo o Guia, ele responde por maximizar o valor do produto e por gerenciar o Product Backlog, o que exige disponibilidade; sem ele, os desenvolvedores criam itens vagos, sem critérios de aceitação. Segundo, o coordenador inclui demandas no Sprint Backlog, que pertence apenas aos Developers; novas demandas devem ser levadas ao Product Owner e ordenadas no Product Backlog, sem ameaçar a Meta da Sprint. Terceiro, não há Definição de Pronto, compromisso do Incremento: item que não a atende não pode ser entregue nem apresentado na Sprint Review, o que explica os defeitos recorrentes.
>
> A comparação de velocidades é inadequada porque story points são uma medida relativa de esforço, complexidade e incerteza, calibrada por cada equipe; logo, 25 e 40 pontos não estão na mesma escala. A velocidade, soma dos pontos dos itens concluídos por Sprint, serve para a própria equipe planejar e prever entregas. Usada como meta, induz a inflar estimativas sem gerar valor.
>
> Um item adequado seria: "Como advogado, quero anexar documentos em PDF à petição, para protocolá-la sem ir ao fórum". Critério de aceitação: dado um arquivo PDF de até 10 MB, quando o advogado o anexa, então o sistema o vincula à petição e exibe a confirmação. A história é valiosa, pois entrega benefício ao usuário; pequena, pois cabe em uma Sprint; e testável, pelo critério objetivo, conforme o modelo INVEST.
>
> Como encaminhamentos, propõe-se: designar um Product Owner com disponibilidade e autoridade para refinar o backlog; criar uma Definição de Pronto que exija testes e revisão de código; direcionar as demandas do coordenador ao Product Owner; restaurar a Daily Scrum de quinze minutos, conduzida pelos Developers com apoio do Scrum Master; e abandonar a velocidade como indicador de desempenho.

---

## 5. Para o caderno de erros

Só o que cai no TJPB. Os erros em assunto já estudado (⚠️) vêm primeiro.

| Assunto | Q | Por que errei | Regra certa |
|---|---|---|---|
| ⚠️ RUP: fases | 26 | Circulei "linha de base da arquitetura" e risquei Elaboração | Arquitetura + riscos + casos de uso críticos = Elaboração |
| ⚠️ Validação de requisitos | 25 | Marquei rastreabilidade | Validar = produto certo (completo, consistente, atende ao cliente); rastrear = gerenciamento |
| ⚠️ Lista encadeada × vetor | 30 | Marquei array dinâmico | Vetor desloca (O(n)); lista duplamente encadeada com o ponteiro = O(1) |
| ⚠️ Coesão: cognato | 5 | Não sabia a palavra e risquei a certa | Cognato = mesmo radical (raciocinar/raciocínio) |
| ⚠️ Discursiva: story points | B | Escrevi que story point inclui tempo e número de pessoas | Medida relativa de esforço, complexidade e incerteza; velocidade serve à própria equipe |
| ⚠️ Discursiva: Definição de Pronto | A | Troquei por Definition of Ready | Pronto = Done = compromisso do Incremento |
| Plural de modéstia | 1 | Achei que "nós" incluía o leitor | Testar se o leitor pratica as ações; se não, "nós" = autor |
| Finalidade do segmento | 2 | Fiquei com "rugiam raivosamente" | Ligar à tese/título; sujeito da frase = foco |
| Interpretação (INCORRETA) | 3 | Dei ✓ na alternativa que inventava a causa | Causa que o trecho não dá = falsa; D × E com causas diferentes |
| Parônimos | 7 | Não conhecia espiar × expiar | Expiar = pagar culpa; espiar = espreitar |
| Probabilidade com permutação | 15 | Não sabia montar | Bloco "AB" × 2, menos os casos proibidos; ÷ n! |
| Sistema de equações | 17 | Conferi as rodas e não as crianças | Fechar as duas condições; atalho do "tudo bicicleta" |
| Equações e razão | 19 | Somei as equações em vez de substituir | Substituir para sumir com o x; p = 3b |
| Função piso | 20 | Não sabia | Aplicar a definição; ⌊−2,1⌋ = −3 |
| UML: composição | 28 | Não sabia | Parte não vive sem o todo = composição (losango cheio) |
| Níveis de modelagem | 32 | Marquei lógico + casos de uso | Alto nível, sem tecnologia = conceitual; dados = diagrama de classes |
| SOAP: WSDL | 34 | Marquei XML | WSDL descreve; SOAP transporta; UDDI publica |
| Gargalo de Von Neumann | 36 | Risquei a certa | Instruções e dados na mesma memória e no mesmo barramento |
| Carry × overflow | 38, 39 | Soma binária errada; não conhecia os termos | Sem sinal = carry; complemento de dois = overflow |
| Octal → binário | 40 | Não lembrava | 3 bits por dígito octal; 4 por hexadecimal |
| Compilação × interpretação | 41 | Marquei o contrário | Sem etapa de construção, linha a linha = interpretação |
| Função × procedimento | 42 | Marquei o termo genérico | Não retorna valor = procedimento |
| Integridade referencial | 46 | Marquei entidade | FK aponta para PK existente = referencial |
| ISO 27005: tratamento | 50 | "Evitar" lido como "reduzir" | Reduzir com controles = modificar; evitar = desistir da atividade |
| Risco residual | 51 | Marquei aceitável | O que sobra depois do tratamento = residual |
| RTO × RPO | 53 | Não sabia | RTO = tempo parado; RPO = perda de dados |
| systemctl | 56 | Marquei "remove" com "manter instalado" no enunciado | disable = não inicia no boot |
| Zachman × ISO 42010 | 58 | Marquei a norma | Framework com matriz 6 × 6 = Zachman (baixa prioridade) |
| Afinidade de sessão | 59 | Não sabia | Servidor cai, sessão se perde; solução = sessão fora do servidor |

Fora do edital (só registro): Q45 (IDEF1X) e Q48 (CMMI/MPS.BR).

---

## 6. O que estudar agora

**1. Revisão das 22h40 (hoje ou amanhã): os erros em assunto já estudado.** Reler as regras 📌 das questões **26 (RUP), 25 (validação), 30 (lista × vetor) e 5 (cognato)** e refazer as quatro sem olhar. Na discursiva: story points e Definição de Pronto.

**2. Estratégia: riscar a certa (5 vezes) é o que mais custa.** O protocolo de 12/11 diz: X só com a prova escrita ao lado. Nas questões 1, 5, 26, 36 e 38 o X não tem prova. Onde você riscou **com** a palavra sublinhada (Q21, Q23, Q24), acertou. Proposta para o próximo bloco: **1ª passada sem nenhum X**, só pontinhos; eu confiro isso na correção.

**3. Português (almoço): a fila não muda, e o H ganha prioridade.** De 2/10 para 5/10. Os 3 erros de interpretação (Q1, Q2, Q3) são todos do **Módulo H**, cuja teoria ainda falta; "finalidade do segmento" foi errada pela terceira vez. Depois do H, **D (concordância)**, que apareceu na sua discursiva ("é necessário a presença", "manter atualizado a situação"). Parônimos (Q7) e cognato (Q5) viram cartões do Anki.

**4. RLM (almoço, dias alternados):** o mapa segue com porcentagem (Q11 firme: pode ser rápido) e **razão, proporção e equações** (Q17 e Q19 são sistemas simples: é o ganho mais rápido). Depois, **combinatória e probabilidade** (Q15; já era erro no Simulado 01). Lógica proposicional continua firme (Q13).

**5. Específicas (19h e 20h): a fila não muda.** Primeiro o **bloco de hash** (8 questões, pendente; a Q29 mostra que a teoria ficou). Depois **POO → SOLID → GoF** (Q28 composição e Q33 Singleton são desse bloco). Em seguida, a Semana 4, **modelo relacional e SQL**: Q31 (formas normais), Q32 (níveis de modelagem) e Q46 (integridade referencial) são exatamente o conteúdo dela.

**6. Decisão para você: arquitetura de computadores e fundamentos de programação.** Foram **10 das 40 específicas** desta prova (Q35 a Q44) e você fez 4. No plano, o assunto está como ⚪ na Semana 10. Ressalva: esta prova seguiu o edital da ALE-RO; o edital do TJPB cita "arquitetura de computadores" na parte comum, mas não diz quantas questões saem dela. Sugestão de baixo custo, sem mexer na fila: **um resumo de 1 página + 8 a 10 cartões no Anki** (bases numéricas, carry × overflow, Von Neumann, memórias, compilação × interpretação, função × procedimento). É conteúdo que você viu na faculdade e que volta rápido. Se quiser, eu preparo.

**7. Discursiva (sábado, treino de estrutura):** reescrever **esta mesma discursiva** em 40 minutos, sem olhar a versão melhorada, usando a lista de entregas. A meta é passar de 15 para 28 ou mais com o conteúdo que você já tem. Só depois, uma discursiva nova no próximo simulado.

**8. Assuntos ainda não estudados (não é para correr atrás agora):** SOAP/WSDL (Semana 6), balanceamento de carga (Semana 7), riscos, continuidade e controle de acesso (Semana 11), sistemas operacionais (Semana 10). Os erros deles ficam no caderno para quando o assunto chegar.

**Pendente fora do estudo:** 🔴 **boleto de R$ 120 até quinta, 19/11** (sem agendamento).

**Próximo simulado:** domingo, 22/11, 13h, como no plano. Comparar com este: **30/60 (26 sem os chutes), 17 acertos firmes, 7 erros convictos, 5 certas riscadas** e discursiva 15/40.
