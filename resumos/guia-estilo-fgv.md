---
tipo: resumo
disciplina: ["Português", "RLM", "Engenharia de Software e Ágil"]
assunto: "Guia de estilo FGV para elaborar questões autorais (Específicas de TI, Português e RLM)"
data: 2026-11-05
atualizado: 2026-11-05
---

# Guia de estilo FGV · como elaborar questões autorais fiéis à banca

**Criado em:** 05/11/2026 · **Para quem:** o Claude, ao gerar blocos, simulados e cartões Anki (ver `CLAUDE.md`, "Padrão das questões").

> **Base:** levantamento em cadernos oficiais FGV 2022–2026, com contagem real de questões e gabaritos. **Ficaram de fora de propósito** TRT-24 2025, TJ-MS 2024 e TJ-AP 2024, reservados para simulados inéditos.
>
> - **Específicas de TI:** TJ-RJ 2026 (Analista de Sistemas, 32 questões) e MPU 2025 (Desenvolvimento, 40) com gabarito definitivo; TCE-RR 2025, AL-GO 2026, DPE-RO 2025 e AL-AM 2025 (formatos).
> - **Português:** TJ-RJ 2026 (20), TJ-MT 2024 (10), TRF-1 2024 (15), Senado 2022 (10) e DATAPREV (12) · 67 questões.
> - **RLM:** TRT-16 2022, MPE-RJ 2025, TCE-SC 2026 (10 cada) e MPE-ES 2026 (5), mais o PDF local com 56 questões FGV de problemas.
>
> **Limites:** são tendências de provas recentes, não garantia de como será o TJPB. O que é contagem real e o que é interpretação está indicado em cada seção.

---

## 1. Regras gerais (todas as disciplinas)

| Regra | Como fazer |
|---|---|
| **Resposta única defensável** | Revisar cada distrator: nenhum pode também estar certo. A FGV anula questões com duas respostas possíveis (TJ-RJ Q41, TJ-MT Q9) |
| **Comando como frase incompleta** | O enunciado termina em **":"** ("…o analista deve:", "…é correto afirmar que:", "A frase abaixo que… é:") |
| **Alternativas paralelas** | Todas concordam com o ":" do enunciado (sem pista gramatical), têm tamanho parecido e a certa **não** é sempre a mais longa (na amostra de TI, foi a mais longa em 30% das vezes) |
| **Pontuação das alternativas** | Nos tribunais 2024–2026: começam com **minúscula**, terminam em **";"** e a última em **"."**. Exceção: alternativas que são frases completas citadas (Português) ou números (RLM) |
| **Gabarito** | Distribuído de forma **quase uniforme** entre A e E (TI: 15/12/14/15/15 em 71). **Não evitar sequências**: a FGV repete a mesma letra 2 a 3 vezes seguidas (MPU teve 5 C seguidas) |
| **Distrator = erro previsível** | Cada alternativa errada corresponde a um raciocínio errado real (termo vizinho, ordem trocada, conta intermediária), nunca a algo aleatório |
| **Aviso** | Manter no topo do bloco: questões autorais no estilo FGV, não oficiais |

---

## 2. Específicas de TI (40 questões)

### 2.1 A FGV tem duas "caras" (contagem real)

| Característica | **Cara Tribunal/MPU** (TJ-RJ + MPU, 72 questões) | Cara Legislativo/TC/DPE (TCE-RR, AL-GO, DPE-RO) |
|---|---|---|
| Resposta única com cenário | **72/72** | Minoria |
| Afirmativas I/II/III | **0** | 3 a 11 por prova |
| V/F em sequência | **0** | 1 a 3 por prova |
| Associação de colunas | **0** | 2 a 3 por prova |
| INCORRETA/EXCETO | **0** | 0 a 1 por prova |
| "…respectivamente" (par de conceitos) | 3 a 4 por prova | Raro |
| Alternativas | Minúscula + ";" | Maiúscula + "." |

**Decisão para os nossos blocos:** o TJ-RJ, tribunal estadual e o mais parecido com o TJPB, segue 100% a cara Tribunal. Usar **~80% no modelo Tribunal** e **~20% de seguro** (I/II/III, "respectivamente" ou V/F). Na prática, **quase não usar INCORRETA em TI**. Para treinar "assinale a incorreta", o lugar é o Português.

### 2.2 Enunciado (modelo Tribunal)

- **Cenário de 4 a 10 linhas + comando de 1 a 2 linhas.** Questões de contagem ou de requisitos podem passar de 15 linhas.
- **Personagem com nome** (~2/3 das questões no TJ-RJ): "O analista Douglas…", "Joana, analista do TJ…".
- **Cenário do próprio órgão** (~40% no TJ-RJ): PJe, processos, audiências, varas.
- **Sistema fictício em caixa alta:** e-SUPRIMENTS, SISDOC, SisGEPRO. Para nós: **e-PROTOCOLO**, **SIGEP-PB**, **JUSTIÇAPB+** etc. Variar e não repetir entre blocos.
- **Aberturas:** "O analista X está…", "Uma equipe de analistas do TJPB…", "Observe o script SQL a seguir.", "Considere o código Java a seguir."
- **Inglês técnico sem tradução** quando for o termo de mercado (taints/tolerations, drill-through, publisher confirms, JOIN FETCH).
- **Versão ou norma citada quando couber:** Scrum Guide 2020, COBIT 2019, ISO/IEC 27001:2022, UML 2.5.1, DMBOK 2.
- **Uma restrição decisiva no cenário:** "melhor custo-benefício", "sem depender de nuvem", "exatamente uma vez", "com baixo overhead", "em sua totalidade". **Cada distrator viola só essa restrição.**

### 2.3 Como montar os distratores (exemplos reais)

| Técnica | Exemplo real |
|---|---|
| **Ordem invertida no "respectivamente"** | TJ-RJ Q54: certa "taints e tolerations"; a errada traz "tolerations e taints" |
| **Rótulo certo + ação errada, ou número trocado** | TJ-RJ Q31: certa "horizontal, adicionando três novas instâncias"; erradas: "vertical, adicionando três instâncias", "horizontal, adicionando recursos à instância atual", "quatro instâncias" |
| **Definição de um conceito vizinho** | TJ-RJ Q37 (cliente-servidor): as erradas descrevem MVC e repositório. TJ-RJ Q40 (REST): uma descreve SOAP e outra, sessão stateful |
| **Cada errada falha em uma condição do cenário** | MPU Q73 (Rancher): EKS depende de nuvem e RKE1 depende de Docker; o cenário proibia os dois |
| **Nível de abstração trocado** | MPU Q45 ("relação" = table/collection): as erradas são column/field e row/document |
| **Vizinhos do mesmo grupo** (nomes que existem de verdade) | Claims OIDC (iss, iat, exp, sub, aud, jti) com descrições trocadas; LIMIT/OFFSET × TOP × FETCH × START de outros SGBDs |
| **Recíproca** | TJ-RJ Q58: duas alternativas com a mesma frase e os termos trocados |

- **Palavra absoluta** (sempre, nunca, exclusivamente) é pista da cara Legislativo. **No modelo Tribunal o erro fica num detalhe técnico plausível.** Usar pouco.
- **"Todas existem, só uma descrição está certa":** 5 funções, comandos ou atributos reais, e só uma descrição correta.

### 2.4 Leitura de código e figuras

| Item | Padrão |
|---|---|
| Frequência | 10% a 25% das questões (TJ-RJ: ~4 de 32; MPU: ~10 de 40) |
| Linguagens, por ordem | **SQL (PostgreSQL)** > Java/Spring > Python > HTML/CSS > YAML de CI (GitLab) > Mongo shell |
| Tamanho do trecho | 5 a 25 linhas |
| O que pergunta | Saída ou valor final ("o valor da variável será:") · erro ("o código possui um erro, pois a classe:") · qual consulta atende · qual padrão foi aplicado · o que é renderizado |
| Alternativas | Às vezes são blocos de código |
| Figuras (MPU: 6 de 40) | BPMN, DER, UML, telas para contar APF. No bloco autoral, descrever em texto ou tabela |

### 2.5 Temas que se repetem nas provas de tribunal

- **Contagem a partir de um depoimento:** quantos RF e RNF (TJ-RJ Q38: 5 RF + 3 RNF; MPU Q66: 4 RF + 1 RNF de usabilidade + 1 de desenvolvimento). Alternativas com números vizinhos.
- **APF:** classificar em cenário e contar EE/SE/CE/ALI/AIE em telas; SNAP no MPU.
- SQL/PostgreSQL, BI/OLAP (fato semiaditivo, dimensão degenerada, surrogate key, dice, drill-through), DDD, OIDC, GitLab CI, Kubernetes, COBIT 2019, JPA/Hibernate, Java moderno (virtual threads, sealed).
- **Profundidade:** "decoreba aplicada", com nome exato de parâmetro, anotação ou variável dentro de um cenário. O gabarito costuma ser o **termo técnico exato em inglês**.

---

## 3. Português (10 questões)

### 3.1 Estímulo: quase nunca há texto longo

- **TJ-RJ 2026, TRF-1 2024 e TJ-MT 2024:** nenhum texto longo comum. **Cada questão tem o próprio estímulo**: frase solta, trecho de 2 a 9 linhas ou 5 frases diferentes nas alternativas.
- **Senado 2022:** um texto de ~30 linhas usado em só 2 questões.
- **Citações de autores** (TJ-RJ: 12 de 20): Machado, Herculano, Aluísio Azevedo, Quintana, Nelson Rodrigues, Voltaire, Epicuro. Crédito no fim: "(Machado de Assis)". Usar só obras em domínio público ou aforismos genéricos.
- **Gêneros:** aforismo, trecho de romance do séc. XIX, frase publicitária, requerimento, discurso, micro-narrativa. **Nada de tirinha nem crônica longa.**
- A FGV julga **até texto literário pela norma-padrão** (TJ-RJ Q5: "aonde" para lugar fixo está errado).

### 3.2 Distribuição por assunto (67 questões; classificação aproximada)

| Assunto | % | Em 10 questões |
|---|---|---|
| **Coesão, referenciação, retomada, conectores, progressão** | 22% | 2 |
| Tipologia, gênero, narrador, funções da linguagem | 16% | 1 |
| Gramática normativa em contexto (sintaxe, classes, regência, concordância, pontuação) | 16% | 1–2 |
| Interpretação, inferência, sentido de frase | 13% | 2 |
| Semântica, vocabulário, figuras (parônimo, paradoxo, redundância) | 12% | 1 |
| **Argumentação** (falácia, tipo de argumento, contra-argumento, modalização) | 10% | 1–2 |
| Reescrita, equivalência, objetividade | 7% | 1 |

- Crase, colocação pronominal e redação oficial: **nenhuma questão própria** na amostra.
- Concordância e regência só caíram na DATAPREV. Nos tribunais 2024–2026, gramática "pura" foi 1 em 15 (TRF-1) e 1 em 20 (TJ-RJ).

### 3.3 Comandos típicos (literais)

- "A frase abaixo que apresenta um exemplo de má argumentação, apoiado numa generalização excessiva, é:"
- "Em relação à estruturação ou significação da frase acima, é correto afirmar que:"
- "Todas as frases abaixo mostram [...]. A única explicação incorreta é:"
- "Nas opções abaixo, há termos destacados que são omitidos na continuidade da frase. A exceção é:"
- "A frase em que a substituição [...] acarreta alteração significativa do sentido original é:"
- "Na frase [...] há a presença de um paradoxo, o que também ocorre na seguinte frase:"
- "Assinale a opção em que a vírgula se justifica pelo mesmo motivo do que em [...]"
- "Assinale a opção em que a segunda estruturação da frase é mais objetiva que a primeira."
- "O argumento utilizado está corretamente identificado em:"

**Proporções (contagem real):**
- **~25% com comando negativo** (NÃO, incorreta, exceção, "a única"), com a palavra-chave em caixa alta. Mais ~1 de "ache o defeito".
- **~1/4 dos enunciados começa com a definição do conceito** antes da pergunta ("As inferências são fruto do conhecimento de mundo do leitor [...]").
- **Formato "frase / rótulo"** em 1–2 questões por bloco: cada alternativa traz frase + barra + classificação a julgar ("... / argumento de autoridade").
- **"Mesmo processo / mesmo motivo de X"**: comparar um modelo com 5 opções (vírgula, figura, elipse, conector).

### 3.4 Distratores

| Na interpretação | Exemplo |
|---|---|
| **Radicalização** | Certa: "relação paradoxal entre felicidade e vida"; errada: "É impossível ser feliz e viver" |
| **Leitura literal de uma palavra** | "visão negativa do fazer poético, já que o poeta é descrito como 'fingidor'" |
| **Rótulo certo com justificativa falsa, ou o contrário** | "texto injuntivo, pois [...] motiva os leitores" |
| **Inversão** | "visão otimista de um aniversário"; "'não é nada' equivale a 'é tudo'" |
| **Termo técnico trocado** | "'ainda' e 'já' indicam tempo passado e futuro"; definições de narrador trocadas |
| **"Correção" falsa misturada** | A alternativa propõe corrigir o que já está certo ("toda espécie" → "toda a espécie", "onde" → "quando") |

- **Na gramática:** 5 frases do cotidiano, parecidas, com **desvios do uso popular** (simpatizei-me, residem à rua, paguei-o, lembra do, meia confusa, é proibido a entrada, 15hs). Só uma correta.
- **Terminologia de linguística textual com precisão:** hiperônimo, nominalização, elipse, anáfora, função fática, modalização, ponto de vista do narrador. É onde a banca já anulou questão.
- **Alternativas de interpretação** com 2 a 4 linhas; **de gramática**, curtas.

---

## 4. RLM (10 questões)

### 4.1 Distribuição (40 questões oficiais, contagem real)

| Assunto | Nº | Em 10 questões (sugestão) |
|---|---|---|
| **Porcentagem** (média ponderada, mistura, aumento × desconto) | 6 | 2 |
| Equações, sistemas, inteiros | 5 | 1 |
| **Lógica proposicional** (negação, condicional falsa, "Todo") | 5 | 2 |
| Combinatória | 4 | 1 |
| Razão e divisão proporcional | 3 | 1 (junto com porcentagem) |
| Ordenação, trocas, movimentos · associação, verdades/mentiras · calendário · casa dos pombos · criptoaritmética | 10 | 2–3 |
| Regra de três composta, juros, probabilidade | 4 | 0–1 |
| Geometria (**fora do edital do TJPB**) | 3 | 0 |

- **~70% é matemática; só ~12% é lógica formal** (5/40; com verdades/mentiras e associação, 7/40).
- Estatística, matrizes, funções, conjuntos e sequências não apareceram nessa amostra, mas **estão no edital**: incluir de vez em quando.
- **No PDF de problemas (56):** casa dos pombos / "no mínimo" (8), sequências periódicas ("a 2026ª letra", 7), calendário (6), horas (6), filas (6), verdades e mentiras (5).

### 4.2 Enunciado

- **Curto:** 2 a 5 linhas. Comando final curto: "É correto concluir que:", "O valor de X é:", "O menor valor possível de n é:".
- **Nomes de pessoas e cotidiano** (supermercado, cinema, torneio, notícia de jornal). **Zero caso jurídico** (0/40).
- **O órgão entra só como material:** a sigla ("TJPBTJPBTJPB…", anagramas de "PARAIBA"), o ano ("2027"), datas.
- **Fórmulas de lógica:** "Considere verdadeira a afirmação…" · "Sabe-se que a sentença '…' é FALSA. É correto concluir que:" · "Assinale a opção que contém a negação de P" · negação em fala de personagem ("Eu sei que isso não é verdade").
- **Regra inventada no enunciado:** "inversão", "movimento = pular o vizinho da direita", "dia central do ano". O desafio é ler a regra, não aplicar fórmula.

### 4.3 Lógica: formatos preferidos

- **Condicional dada como FALSA** ("Se A e B, então C ou D"). As **alternativas são novas condicionais** a testar com os valores forçados.
- **"Todo A é B" → condicionais:** julgar 3 frases. Só a contrapositiva é V; **recíproca e inversa são as armadilhas**.
- **Negação com quantificador + conectivo juntos** ("Pelo menos um… e nenhum…" → "Nenhum… ou algum…"). O distrator nega só uma parte.
- **Verdades e mentiras:** 3 pessoas, 3 itens, "apenas uma é verdadeira".

### 4.4 Números e distratores

- **Contas com números pequenos e inteiros.** Fração só quando o resultado exige. "Aproximadamente" em juros e desconto.
- **Alternativas em progressão ou bem próximas** (11–12–13–14–15; 59,4–59,6–59,8–60,2–60,4), **em ordem crescente ou decrescente**. Ordem de grandeza também é testada (15% / 1,5% / 0,15%…).
- **Cada distrator vem de um erro clássico:**

| Erro explorado | Exemplo real |
|---|---|
| Linear em vez de circular | Dias não seguidos na semana: 14 (certo) × 15 |
| Simetria de porcentagem | Desconto de 17% → aumento de 20,5% (certo) × 17% |
| Subtrair pontos percentuais | 80% → igualar: 75 (certo) × 60 |
| Ignorar a média ponderada | 25% (certo) × 15% (= 10 + 5) |
| Juros sobre o valor cheio | 22% (certo) × 10% |
| Contar ou não as pontas | "Depois de D37 e antes de F23" |

- **Combinar dois assuntos** numa questão (torneio = combinação + sistema; urna = razão + equação).

---

## 5. Como aplicar nos nossos blocos

| Situação | Regra |
|---|---|
| **Vale para tudo** | Blocos, provas, questões avulsas no chat, simulados autorais e cartões Anki. Só muda se o Tiago pedir **explicitamente** outro formato (regra de 05/11) |
| **Módulo 0 de Português** (A1–B3, base) | Conteúdo básico, **formato FGV**: comando com ":", distratores do uso popular, estímulo curto próprio (frase ou citação) |
| **Bloco de assunto novo** | Só o assunto (regra de 28/10), no formato FGV da disciplina |
| **Específicas** | ~80% modelo Tribunal (cenário + nome + sistema fictício + ":"; alternativas minúsculas com ";") · ~20% I/II/III, "respectivamente" ou V/F · INCORRETA só excepcionalmente |
| **Português** | Estímulo próprio por questão · ~25% negativas · 1 "frase / rótulo" · 1 "mesmo processo" |
| **RLM** | Cotidiano com nomes, sem caso jurídico · alternativas numéricas em progressão e ordenadas · distrator = erro clássico |
| **Okular** | Continua valendo: `\(C)` e `I\.` no `.md` |
| **Anki** | Mesmo padrão em versão curta: comando com ":" e distratores do mesmo grupo |

### Checklist antes de entregar um bloco

1. O comando termina em ":" e todas as alternativas concordam com ele?
2. Só uma resposta é defensável? Cada distrator é um erro previsível e diferente?
3. A certa não é sempre a mais longa? O gabarito está espalhado (com algumas sequências)?
4. TI: tem cenário com nome e restrição decisiva? Tem código (SQL primeiro) quando o assunto permite?
5. Português: estímulo curto e próprio? Proporção de negativas perto de 25%?
6. RLM: números pequenos, alternativas ordenadas e em progressão?
7. Aviso de "autorais, não oficiais" no topo e gabarito fora do arquivo?
