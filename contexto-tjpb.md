# Contexto de Estudo · TJPB 2026

**Atualizado em:** 06/11/2026 · **Semana do plano:** 2 (APF, SAFe e Testes)

> Arquivo substituído toda semana. Regras estudadas ficam em "regras-tjpb". Plano e conteúdo por semana ficam em "plano-tjpb".

---

## Situação atual

- Semana 0 (21–25/10): inscrição, caderno de erros, Anki e diagnóstico.
- **1ª retificação do edital (23/10):** jornada 30h · isenção da taxa só até 27/10, 16h · inscrição segue até 18/11, 16h. Plano atualizado para a versão 3 em 26/10. Inscrição: ainda não confirmada.
- **2ª retificação do edital (29/10, lida em 02/11):** discursiva vira **estudo de caso** sobre Conhecimentos Específicos (análise do contexto → problemas → teoria e norma → solução), **mínimo 24/40** e 8 hipóteses de nota zero · "remuneração" → "vencimento" (valor igual) · demais itens não afetam o Dev. Anexo I não mudou. Discursivas autorais passam a ser estudos de caso.
- Adiantando a Semana 1 (Engenharia de Software e Ágil) desde 22/10.
- Estudo sem cursinho: fontes oficiais + banco de questões (QConcursos/TEC) + Claude como professor e corretor de discursiva. Pacotes pós-edital ainda não lançados.
- Questões autorais salvas em .md na pasta "QUESTÕES NÃO OFICIAIS" (blocos em `Provas/`: `AAAA-MM-DD_Semana-XX_Bloco-XX_Assunto.md`; correções em `Correções/`: `_CORRECAO.md`). Provas oficiais seguem a mesma divisão.
- Simulados: todo domingo, 13h–17h, + 1 discursiva + 1h de correção. Em janeiro, 13h–18h.
- **1º simulado oficial: domingo 01/11, 13h**, cronometrado e sem consulta. Prova FGV inédita: TJ-MS 2024 ou TJ-AP 2024 (recomendadas) ou outro caderno da DATAPREV (não o ATI Desenvolvimento de Software · tarde, cujo Português já foi resolvido em 23/10). Marcar "?" nos chutes. É o ponto de partida da evolução. O TRT-16 de 25/10 foi desconsiderado.

---

## Histórico semanal

### Semana 0 (21–25/10) · Diagnóstico

- **Antes do plano · Prova FGV TJ-RR (TI):** placar não registrado. O que mais derrubou: leitura de código (rastrear saída).
- **21/10 · Português/RLM (10 autorais):** 3/10
  - Erros: silogismo "se... então" (negar o antecedente), opinião × fato, pronome "cujo", falácias (generalização × falsa causa), fila com trocas.
  - Não soube: porcentagem com mudança no grupo, divisão proporcional.
- **22/10 · Bloco 1 SDLC e Scrum (5 autorais):** 3/5
  - Acertos: cascata, Daily Scrum, incremental.
  - Erros: quem cancela a Sprint (marquei Developers), DoD como artefato, duvidei da definição da Retrospectiva.
- **23/10 · Prova oficial FGV DATAPREV (Português, Q1–12):** 2/12 (17%) · 8 erros · 2 em branco
  - Acertos: pontuação (oração adverbial anteposta), variação linguística.
  - Em branco: oração subordinada substantiva, adjunto adnominal × complemento nominal.
  - Erros: interpretação (rótulo "irônica"; risquei o paradoxo certo), regência ("lembra do"), vocabulário (irascível), discurso direto × indireto, "de modo que" (consequência × finalidade), verbo de ligação ("ficou à janela"), concordância ("é proibido a entrada").
  - Padrões: lacuna de base em sintaxe; julgar pelo uso comum e não pela norma; errar "assinale a incorreta" marcando alternativa verdadeira (Q6, Q8); trocar a resposta certa sem regra (Q4, Q5).
  - Arquivos: `PROVAS OFICIAIS (estudo)/Provas/2026-10-23_Semana-00_FGV-DATAPREV_Portugues_*` (prova e PDF original) e `Correções/` (correção v3).
  - Meta para a próxima prova de Português: ≥ 5/12, nenhuma em branco por desconhecimento.
- **24/10 · Bloco Eng. Software UNIVESP Aulas 01–05 (14 autorais, PDF anotado à mão):** 9/14 (64%) · 3 erros · 2 em branco
  - Acertos: atividades do processo, cascata, incremental ("incorreta"), reuso (I/II/III), Manifesto Ágil, ágil × planos, test-first, requisito de usuário × sistema, RNF ("incorreta").
  - Em branco (não estudado): RUP · fases (Elaboração) e 3 perspectivas.
  - Erros: XP (aceitei "propriedade coletiva = um dono"; descartei histórias de usuário achando que era só Scrum), scaling up × out, RNF de produto × organizacional (invertidos).
  - Evolução: "assinale a incorreta" 2/2 usando V/F ao lado (era erro na DATAPREV); modelos de processo acertados de novo.
  - Arquivo: `QUESTÕES NÃO OFICIAIS/Correções/2026-10-23_Semana-01_Bloco-01_EngSoftware-UNIVESP-Aulas01a05_CORRECAO_v2.md` (+ .pdf)
- **25/10 · Simulado TRT-16 2022:** desconsiderado (feito sem condições de prova e sem placar). Não entra na evolução.
- **Evolução:** — (ponto de partida)
- **Observação:** no TRT-16, Português de Analista cobrou mais argumentação, inferência e organização textual do que gramática pura.

### Semana 1 (26/10–01/11) · Engenharia de Software e Ágil

- **26/10 · Prova Eng. Software (15 autorais, Okular):** 8/15 (53%) · 6 erros · 1 em branco
  - Acertos: RUP fases (era branco), RUP × ágil, verificação × validação, artefatos/compromissos (chute, segundo anotação), XP práticas (era erro), subtipos de RNF (era erro), leitura de código 2/2 (TDD Python, refatoração Java).
  - Em branco: perspectivas do RUP (2ª vez).
  - Erros: espiral × prototipação (palavra "protótipo" puxou), modelo em V (lado do requisito × teste; unitário ≠ req. sistema), prototipação "incorreta" (achei que não ajuda na elicitação), Scrum (achei que o PO altera o Sprint Backlog, 2ª vez em responsabilidades), scaling up × out (2ª vez), Kanban lead × cycle (tomei a fila como lead time).
  - Evolução: Eng. Software 9/14 (64%) → 8/15 (53%), com 8 das 15 sobre pontos fracos. Estratégia V/F funcionou (marcou "?" na resposta certa da Q3, mas não confiou).
  - Arquivo: `QUESTÕES NÃO OFICIAIS/Correções/2026-10-26_Semana-01_Bloco-01_Prova-EngSoftware-15q_CORRECAO.pdf` (+ .md)
- **26/10 · Organização do estudo:**
  - Resumo `mapa-engenharia-de-software` v2 (pra que serve · onde é usado · por que é assim · conceitos técnicos).
  - Obsidian configurado: `00-HOME` (seção Hoje), 14 notas em `disciplinas/`, painéis Bases em `paineis/`, modelos em `modelos/`.
  - Pastas de questões e provas divididas em `Provas/` e `Correções/`. Correções passam a sair sempre em PDF.
  - 1ª retificação do edital lida e aplicada ao plano (v3): jornada 30h, isenção só até 27/10, item 10.12 corrigido.
  - Anki com AnkiConnect: 30 cartões em formato FGV simplificado, baralhos `TJPB 2026::03 Engenharia de Software e Ágil::<assunto>` + `00 Estratégia de prova`. Primeira revisão: hoje às 22:40.
- **27/10 · Bloco RLM Conectivos e proposições (15 autorais, PDF anotado):** 8/15 (53%) · 7 erros · 0 em branco
  - Acertos: condicional falsa, negação do "e" e do "se… então" e contrapositiva (3, 4 e 5 assistidas, explicadas antes da resposta), bicondicional na dedução, validade (Q12: não caiu em negar o antecedente, erro de 21/10), negação de "todo", leitura de código Python (XOR com `!=`).
  - Erros de conteúdo: paradoxo tomado como proposição, tabela 2⁴ em vez de 2⁵ (contou 4 variáveis), F ↔ F avaliado como F, tautologia por eliminação sem simplificar, condicional falsa (copiou o consequente).
  - Erros de atenção: Q10 (deduziu Ana V e Bruno F, mas marcou a D) e Q11 (pressa: aceitou "fato negativo não conclui").
  - Método que funcionou: lógica como Álgebra de Boole/circuitos do IFPB (A → B = A' + B, ↔ = XNOR, ou… ou = XOR) e a analogia do segurança da festa. Usar esse formato nas explicações de RLM.
  - Arquivo: `QUESTÕES NÃO OFICIAIS/Correções/2026-10-27_Semana-01_Bloco-01_RLM-Conectivos-e-Proposicoes_CORRECAO.pdf` (+ .md)
  - Anki: 31 cartões FGV (10 em cada sub-baralho `02 RLM::01 Conectivos e tabela-verdade`, `02 Negações e equivalências`, `03 Dedução e argumentos` + 1 em `00 Estratégia de prova`). Cópia em `anki/2026-10-27_RLM-Conectivos-Proposicoes_formato-FGV.tsv`.
  - Edital completo lido (`edital/edital.pdf`) → **plano v4**: parte "Comum a todos os cargos de TI" incluída (SO, redes, BI, ISO 27005, gestão de TI, PJe, MoReq-Jus, Res. 522/2023), níveis 🔴 🟡 ⚪ por assunto, normas do CNJ aos sábados e RLM com 12 itens de matemática (seção 4.2). Conversa franca sobre o volume: meta realista é passar dos 60% e ter a discursiva corrigida; as vagas dependem de constância.
- **28/10 · Bloco Português Classes de palavras A1 (15 autorais, PDF anotado):** 9/15 (60%) · 5 erros · 1 em branco
  - Acertos: substantivo 3/3 (substantivação, abstrato × concreto, gênero), adjetivo 2/2 (posição; opinião × fato, que era erro em 21/10), artigo definido × indefinido, numeral (classificação, "um" numeral), classificação mista. "Incorreta" 2/2 entre as respondidas.
  - Em branco: locução → adjetivo (de rio = fluvial, não lacustre).
  - Erros: locução adjetiva × adverbial ("às pressas"; contou "com rapidez" como adjetiva), artigos de lei (art. 10 = dez), **concordância repetida de 23/10** ("é proibido a entrada" e "seguem anexo": de novo pelo uso comum).
  - Pontinho = candidata sem certeza: Q4 ✅, Q10 ❌, Q11 ✅. Acertos sem dúvida: 7 de 9.
  - Arquivo: `QUESTÕES NÃO OFICIAIS/Correções/2026-10-28_Semana-01_Bloco-01_Portugues-Classes-de-Palavras-A1_CORRECAO.pdf` (+ .md)
- **28/10 · Bloco Eng. Software User stories, INVEST e BDD (15 autorais, PDF anotado):** **13/15 (87%)**, melhor placar até agora · 1 erro · 1 em branco
  - Assunto do dia (Q1–10): 9/10. 3 Cs, INVEST (I e N), épico, critério × DoD, Gherkin, BDD × Cucumber, história bem escrita e leitura de código Python (rastreou na margem) certos. Q4 e Q5 com marca de dúvida.
  - Em branco: TDD × ATDD × BDD (Q8, só "?"). Dava para eliminar: I = V e III = F deixavam só A ou E.
  - Revisão (Q11–15): 4/5. Acertou Sprint Backlog dos Developers (era erro 22 e 26/10), lead × cycle (era erro 26/10), modelo em V (era erro 26/10) e negação da condicional por Boole.
  - Erro: concordância **pela 3ª vez** ("em anexos"; descartou "é necessário paciência"). Eliminou certo "anexo", "é proibido a" e "meias".
  - **Regra nova (pedido do Tiago):** bloco de assunto novo cobra só o assunto; revisão e pontos fracos só quando ele pedir (registrado no `CLAUDE.md`).
  - Novo PC (Windows, `C:\Users\Pichau`, conta `tiagomarcosss`): Git, GitHub CLI e Node instalados nesta sessão.
  - Arquivo: `QUESTÕES NÃO OFICIAIS/Correções/2026-10-28_Semana-01_Bloco-02_User-Stories-INVEST-e-BDD_CORRECAO.pdf` (+ .md)
- **29/10 · Bloco RLM Argumentação lógica e diagramas lógicos (15 autorais, PDF anotado):** 9/15 (60%) · 4 erros · 2 em branco
  - Começou como diagnóstico ("não sei o assunto"); virou treino depois da teoria e de 11 exemplos resolvidos no chat. Assistidas: Q2 e Q11 (montei o caminho de setas) e Q6 (desempatei B × D). Sem as assistidas: 7/12.
  - Acertos: todo + algum, afirmar o consequente, modus tollens, falácias 2/2 (era erro em 21/10), equivalência de "todo" (recíproca, com dúvida), negação de "nenhum".
  - Em branco ("?"): conjuntos/Venn (Q9) e conjuntos em Python (Q15). Assunto não estudado.
  - Erros: letras parecidas P_F × P_e trocadas (Q2), "conclusão V → válido" (Q4), "S' = V" lido como servidor V (Q10), contrapositiva D' → L sem negar o L + aceitou a recíproca (Q14).
  - Método que funcionou: setas para todo/nenhum, ficha do x para algum, "V empurra para frente, F puxa para trás", teste pela 1ª palavra da alternativa. O Tiago prefere raciocinar com V/F e setas a expandir Boole (achou "massivo").
  - Arquivo: `QUESTÕES NÃO OFICIAIS/Correções/2026-10-29_Semana-01_Bloco-01_RLM-Argumentacao-e-Diagramas-Logicos_CORRECAO.pdf` (+ .md)
- **30/10 · Bloco Português Verbo, advérbio e locuções A2 (15 autorais, PDF anotado):** 8/15 (53%) · 6 erros · 1 "não sabia" (Q4 voz passiva, letra certa com "?")
  - Acertos: verbo de ligação, locução verbal, tempos (-sse → -ria), advérbio × adjetivo (setas certas), concessão × tempo, "bastante" (com dúvida entre A e D), modalização e "vai + infinitivo" (com dúvida). Verbo: 4/5.
  - Erros: "muito" ligado ao verbo vizinho (é "muito bem"), "-mente" no primeiro advérbio, contagem de locuções adverbiais (classificou certo as do meio, mas esqueceu "Na segunda-feira," do início), **"em anexo" pela 4ª vez** (fez "anexo" concordar em todas), "reaveu" (é reouve), particípio de "tinha terminado" aceito como adjetivo.
  - Comparação: A1 (28/10) 9/15 → A2 8/15.
  - Arquivo: `QUESTÕES NÃO OFICIAIS/Correções/2026-10-30_Semana-01_Bloco-01_Portugues-Verbo-Adverbio-e-Locucoes-A2_CORRECAO.pdf` (+ .md)
- **30/10 · Bloco Eng. Software Estimativa ágil (15 autorais, PDF anotado):** 10/15 (67%) · 4 erros (1 chute) · 1 em branco
  - Estudou por videoaula no mesmo dia. Conceito firme: story points, Fibonacci, Planning Poker (procedimento, divergência, cartas "?"/"∞"), T-shirt, Guia do Scrum (Developers dimensionam), dias ideais, capacidade, triangulação (com dúvida em B = APF). 
  - Em branco ("?"): Cone da Incerteza (não conhecia o termo).
  - Erros: tudo em **velocidade**. Q5: método certo, mas dividiu 63 ÷ 3 = 32. Q6 (código): ignorou o `[-3:]`, fez a média das 5 e chutou. Q8: **riscou a falsa numa "INCORRETA"** e circulou uma verdadeira. Q15: achou que "estimativas independentes" no Delphi era falso e que item parcial conta na velocidade.
  - Comparação: user stories (28/10) 13/15 → estimativa 10/15.
  - Arquivo: `QUESTÕES NÃO OFICIAIS/Correções/2026-10-30_Semana-01_Bloco-02_Estimativa-Agil_CORRECAO.pdf` (+ .md)

### Semana 2 (02–08/11) · APF, SAFe e Testes

- **31/10 a 02/11:** pausa por esgotamento (burnout), sem estudo. A3, B1 e o 1º simulado ficaram para depois. **1º simulado remarcado para dom 08/11, 13h.**
- **03/11 (tarde) · RLM Conjuntos e Venn (bloco 15 autorais, respostas pendentes):** feito com ajuda no chat.
  - Q3 assistida ("exatamente dois"): lançou os pares (20, 15, 18) direto nas faixas, sem descontar o centro. Entendeu: faixa = par − centro; exatamente dois = soma dos pares − 3 × centro.
  - Q4 e Q5 assistidas (mínimo/máximo): **não entendeu** pelas explicações de "arrumação" nem pela tabela. Entendeu pela imagem dele do **"sugar"**: o círculo maior engole o menor, e quem estava só no menor vai para fora (fora máx = 5 + 45 = 120 − 70). Simulador de Venn criado como artefato. Q15 (mínimo dos três) não feita.
  - Ainda falta enviar as respostas do bloco para a correção em PDF.
- **03/11 (tarde) · Silogismos com todo/algum (4 questões de videoaula, resolvidas no chat):** Pedro biólogo ✅, pedreiros/carpinteiros ✅ (a E também decorre), militares ❌ (juntou fichas de "alguns" diferentes, C × D), cariocas ✅ por eliminação. Travou porque o enunciado não dizia "considere verdadeiro" (o "se… então" já diz).
  - Método que funcionou: setas + ficha da pessoa (criar um carioca e empurrar o V pelas setas). Explicar com a **listinha dele** (`C → F`, `C · B`), não com notação nova. "Ajustar" uma anotação equivalente à certa confunde: só corrigir quando estiver errada.
- **03/11 (tarde) · 7 questões FGV oficiais (diagramas lógicos 2023–2024 + TJ-MT 2024):** 4/6 respondidas
  - ✅ Niterói 2023 (algum é simétrico; assistida), Abreu e Lima 2024 Q3 (V-F-F pela lógica; a fonte dá B = V-V-F, gabarito divergente, não conta como erro), Macaé 2024 (contrapositiva com "ou"), TJ-MT Q24 (p ∨ q → r falsa).
  - ❌ PM-SP 2023 (marcou "quem é ciclista joga basquete": leu "alguns" como "todos"; a anotação `C · B · F` estava certa, faltou traduzir a alternativa) e Abreu e Lima Q4 (achou que "todo B é C" garante "nem todo C é B"; B pode ser igual a C).
  - Pendente: TJ-MT Q29 (B − A).
  - Padrão dos erros: **ler a premissa mais forte do que ela é**. Contrapositivas 2/2.
- **03/11 (noite) · Bloco APF/IFPUG padrão FGV (8 autorais, PDF anotado):** 3/8 (38%) · 4 erros · 1 em branco ("?")
  - Antes do bloco: pesquisa em 10 provas FGV de TI. APF aparece em ~1 questão por prova (TJ-RJ 2026, MPU 2025, TJ-PI 2015), sempre **classificação em cenário, telas e VAF**, nunca tabela DER/RLR. Decisão: estudar conceito, não decorar tabelas.
  - Acertos: transações SE × CE 2/2 (definição de SE; "dias calculados" = SE e "como armazenado" = CE) e propriedades da APF (I/II/III).
  - Em branco ("?"): VAF (não sabia a fórmula: 0,65 + 0,01 × soma).
  - Erros, todos em **funções de dados**: "armazenados na base" virou ALI em vez de EE (Q1) · aba dependente contada como 2º ALI e EE dobradas (Q2) · cadastro só lido virou ALI por estar no "mesmo banco corporativo", riscando a certa (Q6) · índice e backup contados como ALI (Q8).
  - Analogias que funcionaram: SE = GET com service/cálculo, CE = GET puro, EE = POST/PUT/DELETE, ALI = tabelas do próprio banco, AIE = API de outro sistema, RLR = classe dentro do agregado, DER = atributos.
  - Arquivo: `QUESTÕES NÃO OFICIAIS/Correções/2026-11-03_Semana-02_Bloco-03_APF_CORRECAO.pdf` (+ .md)
  - Depois da correção: desânimo forte ("não vou passar", "acho que vou desistir"), no fim de um dia pesado e um dia após a pausa por esgotamento. Decidiu continuar. Combinado: não decidir nada cansado à noite. Se o cansaço voltar, reduzir a carga (1 bloco por noite, cortar assuntos ⚪) em vez de parar. Retoma em 04/11.
- **04/11 · Decisão: mínimo/máximo de Venn fora do estudo** (aposta do Tiago: não está escrito no edital; no máximo 1 questão). Fica só a fórmula de emergência (meio mín = A + B − total · meio máx = o menor). Bloco 02 de 03/11 (15 questões, metade de mín/máx) **apagado a pedido dele** e trocado por um bloco curto. No bloco 01 de 03/11, pular Q4, Q5 e Q15.
- **04/11 (manhã) · Bloco RLM Conjuntos e Venn sem mín/máx (8 autorais, PDF anotado):** 4/8 (50%) · 2 erros · 2 "não sabia" ("?")
  - Acertos: nenhum com 2 conjuntos, (A ∩ B) − C (com pontinho; anotação certa), **3 conjuntos "exatamente uma" sozinho** (em 03/11 foi assistido) e **conjuntos em Python** (em branco em 29/10).
  - Erros de execução, com o método certo (explicados por ele): Q2: achou o meio (25%) e **tirou do círculo errado** (50 − 25 = só aplicativo; pedia só site = 45 − 25 = 20%). Q3: montou as regiões, mas **subtraiu uma** (`x − 1 + 10 − 2(2x − 10) = 62`); certo: (x − 10) + 10 + (2x − 10) = 62 → x = 24 → somente X = 38.
  - "?": pertinência × inclusão (∈ × ⊂ com elemento {1}) e "exatamente um/dois/três" (fatias separadas: total = nenhum + exat. 1 + exat. 2 + exat. 3).
  - Arquivo: `QUESTÕES NÃO OFICIAIS/Correções/2026-11-04_Semana-02_Bloco-01_RLM-Conjuntos-e-Venn-8q_CORRECAO.pdf` (+ .md)
- **04/11 (noite) · Requisitos adiado a pedido** (diz lembrar RF × RNF, TDD/ATDD e user stories; bloco no sábado). Pesquisa de incidência do T2: tipos de teste e TDD estão no edital e caem em quase toda prova FGV de desenvolvimento (117 questões FGV no QConcursos; AL-GO 2026 com ≥ 4; NAV Brasil 2026 com 4; TJ-SC 2026). SAST/DAST, Pact e mutação: nenhuma questão FGV achada → 🟡/⚪.
- **04/11 (noite) · Bloco Tipos de teste (15 autorais, PDF anotado), após videoaula ISTQB:** 8/15 (53%) · 3 erros · 4 "não sabia" ("?")
  - Acertos: níveis (com dúvida na B), alfa × beta, carga × estresse, erro → defeito → falha, stub × driver, pirâmide/automação, **complexidade ciclomática** (desenhou o grafo) e TDD com stub (código).
  - "?": **valor-limite**, **partição de equivalência**, **caixa-branca × preta** e **estático × dinâmico**. Técnicas de projeto de casos: 0/4.
  - Erros: cobertura (achou que 1 caso com `if` True dá 100% de decisões) · confirmação × regressão invertidos ("executou novamente" puxou regressão) · em "incorreta", marcou o princípio verdadeiro "presença, não ausência" (a falsa era a falácia da ausência de erros, com "certamente").
  - Arquivo: `QUESTÕES NÃO OFICIAIS/Correções/2026-11-04_Semana-02_Bloco-02_Tipos-de-Teste_CORRECAO.pdf` (+ .md)
- **05/11 (manhã) · Anki de silogismos + 1 autoral no chat (Central de Mandados × teletrabalho):** acertou a autoral (C), com dúvida.
  - **As setas estão sempre certas** (inclusive as contrapositivas). Trava na **tradução das alternativas**: "documento" tomado como letra (substantivo comum a todos não ganha letra), emendar setas que não encaixam (fim de uma ≠ começo da outra), "algum" na alternativa.
  - Método que destravou: setas soltas com "/" → emendar onde a letra se repete igual → **"Sl → Pp · Ti'" = tudo o que o Sl carrega** (forma dele) → "algum" = ficha (um "Carlos") empurrada pelas setas. Prefere V/F com as setas originais a virar contrapositiva. A seta só obriga quando o começo é V (F → V é verdadeiro). Premissa vale como V mesmo sem "considere verdadeiro" (dúvida repetida de 03/11).
- **05/11 (tarde) · Anki zerado no AnkiWeb** (revisão geral, muita Eng. Software e RLM). Sub-baralho `04 APF, SAFe e Testes::02 Testes` **não aparece no AnkiWeb**: lote de 04/11 (`anki/2026-11-04_Tipos-de-Teste_formato-FGV.tsv`) não sincronizado/importado. Resolver no PC de casa (sincronizar ou importar o .tsv).
- **05/11 · Decisão: conta do VAF fora do treino.** Pesquisa: APF FGV 2026 (MPE-ES, TCE-SC, TJ-SC, TCE-PE) cobrou classificação e conceito, não a conta. Conta do VAF achada em FCC (TRE-PI 2009, TJ-CE 2022); uma FGV TCE-SC 2026 com conta foi citada, mas não confirmada. SISP e contratos usam PF não ajustado. Fica só a regra de emergência: **soma 35 = neutro, ±1% por ponto**. Tempo de APF vai para ALI × AIE e EE × SE × CE.
- **05/11 · Guia de estilo FGV criado** (`resumos/guia-estilo-fgv.md`, regra no `CLAUDE.md`): levantamento em cadernos FGV 2022–2026 (TI: TJ-RJ 2026 e MPU 2025; Português: 67 questões; RLM: 40 oficiais + 56 do PDF). Achados que podem mexer no plano (**conversar antes de mudar**): RLM recente ≈ 70% matemática e só ≈ 12% lógica formal (porcentagem é o assunto nº 1) · Português de tribunal quase sem texto longo, forte em coesão, argumentação e linguística textual; gramática pura rara · TI no modelo Tribunal sem INCORRETA nem I/II/III, SQL é o código mais cobrado, contar RF/RNF num depoimento caiu no TJ-RJ e no MPU. Simulados: TRT-24 2025, TJ-MS 2024 e TJ-AP 2024 seguem inéditos.
- **05/11 · Pact e mutation testing (⚪) cortados da fila** a pedido (cansado de testes; nenhuma questão FGV achada em 04/11). Único assunto de teste restante: SAST × DAST (sexta).
- **05/11 (tarde) · Bloco Português B1 + B2 · sujeito e complementos (15 autorais, PDF anotado):** 7/15 (47%) · 7 erros · 1 em branco
  - Acertos: sujeito posposto, sujeito na passiva, oculto ("nós"), haver sem sujeito (com dúvida), VTI, verbo de ligação × lugar, núcleo do sujeito (**riscou os adjuntos: técnica certa**).
  - Erros: composto × adjuntos com "e" ("servidores da vara e do cartório") · "expedem-se certidões" (passiva) tomado como indeterminado · "parecia tranquila" (ligação) como intransitivo, com a certa no pontinho · OD × OI invertidos ("aos advogados") · predicativo do sujeito como adjunto de modo (sublinhou a ligação com o sujeito) · predicativo do objeto como objeto direto.
  - **"INCORRETA" 0/2 de novo** (Q7 em branco com pontinho numa verdadeira; Q14 circulou a verdadeira), sem V/F escrito. 3ª sessão seguida com esse erro.
  - Por tipo: sujeito 5/8 · complementos 2/7 · predicativo 0/2. Comparação: A1 9/15 → A2 8/15 → B1 + B2 7/15. **B1 + B2 sai da fila** (teoria + bloco corrigido).
  - Arquivo: `QUESTÕES NÃO OFICIAIS/Correções/2026-11-05_Semana-02_Bloco-01_Portugues-Sujeito-e-Complementos-B1B2_CORRECAO.pdf` (+ .md). Bloco feito no formato antigo (antes do guia FGV); os próximos seguem o guia.
- **05/11 (noite) → corrigido em 06/11 · Bloco SAFe (12 autorais, 1º no modelo do guia FGV, PDF anotado):** **9/12 (75%)**, melhor placar da Semana 2 · 3 erros · 0 em branco
  - Acertos firmes (sem pontinho): feature × story × épico × capability e ART (I/II/III com V/F escrito). **Acertos com dúvida (pontinho): 7 de 9** → ROAM (B × C), WSJF conta e código (contas certas na margem), IP Iteration, objetivo não comprometido (C × D), eventos do ART ("?" em Solution Demo) e Large Solution (B × D).
  - Erros: **RTE × Product Management** (Q1: ignorou "não define nem prioriza o backlog") · **voto de confiança baixo** (Q3: entre B e E, aceitou Business Owners refazendo o plano sem os times) · **CD Pipeline** (Q11: Continuous Exploration tomada como "levar à produção"; o cenário era deploy × release com feature toggle).
  - Leitura de código (Q6, Python com `sorted(..., reverse=True)`): rastreou certo na margem, mas com pontinho (não conta para tirar dos pontos fracos).
  - **SAFe sai da fila** (teoria + bloco corrigido).
  - Arquivo: `QUESTÕES NÃO OFICIAIS/Correções/2026-11-05_Semana-02_Bloco-02_SAFe_CORRECAO.pdf` (+ .md)
- **06/11 (tarde) · Bloco Português A3 · pronome, preposição e conjunção + locuções (15 autorais, modelo do guia FGV, PDF anotado):** 8/15 (53%) · 7 erros · 0 em branco
  - Antes do bloco: teoria das locuções (pronominal, prepositiva, conjuntiva) no chat. Fez a prova à tarde para liberar a noite.
  - Acertos: relativo × outros "que" (eliminação certa), valor da preposição (teste "por quê?" anotado), concessiva, prepositiva × conjuntiva ("INCORRETA"), este × aquele (setas certas), **"de modo que" = consequência** (era erro em 23/10), "como" causa × conformidade (com pontinho), "toda" × "toda a".
  - Erros, quase todos pelo **uso comum**: "Vossa Excelência… vosso" · "viu-lhe" aceito e "os recebeu" rejeitado (OD × OI de novo) · "e" adversativo tomado como aditivo · "o sistema que eu te falei" (faltou "de que") · **"para mim assinar" aceito e "para eu revisar" riscado** · ambiguidade do "seu" não vista (uma seta só) · "pois" posposto tomado como "porque" (**com certeza**).
  - **"Cujo" parece errado para ele** (Q10 e Q14), mas estava certo nas duas.
  - **V/F escrito nas negativas (Q4, Q8, Q11)**: primeira vez desde 28/10. Negativas 2/4, e os dois erros foram de conteúdo.
  - Por tipo: preposição e locuções 2/2 · conjunções 3/5 · **pronomes 3/8**. Comparação: A1 9/15 → A2 8/15 → B1 + B2 7/15 → A3 8/15. **A3 sai da fila** (teoria + bloco corrigido; a correção cobre a teoria dos pronomes).
  - Arquivo: `QUESTÕES NÃO OFICIAIS/Correções/2026-11-06_Semana-02_Bloco-01_Portugues-Pronome-Preposicao-Conjuncao-A3_CORRECAO.pdf` (+ .md)

---

## Pontos fracos (prioridade)

### Português / RLM

1. Concordância nominal pela norma-padrão (≈50% do Português FGV): errada **4×** (23/10, 28/10 manhã, 28/10 noite e 30/10), sempre pelo uso comum. "Em anexo" errado 3 vezes seguidas: em 30/10 fez "anexo" concordar até com o "em". Regra-gatilho: **tem EM = advérbio = não varia**. Olhar primeiro se há "em" e se há artigo. "Bastante" acertou em 30/10 (com dúvida)
2. **Pronomes pela norma (novo, 06/11): 3/8 no A3, sempre pelo uso comum.** "Para mim + infinitivo" aceito (é "para eu revisar") · o × lhe ("viu-lhe" aceito; ligado ao OD × OI do B1 + B2) · Vossa Excelência + "vosso" (é "seu") · relativo sem a preposição do verbo ("que eu te falei" → "de que") · ambiguidade do "seu" (desenhar duas setas) · "cujo" parece errado e não é (Q10 e Q14). Firmes: relativo × outros "que", este × aquele, "toda" × "toda a"
3. Sintaxe (base), atualizado 05/11: B1 + B2 7/15, complementos 2/7. **Predicativo** (do sujeito × adjunto de modo; do objeto × objeto direto) 0/2 · OD × OI com "aos" · intransitivo × ligação · composto × adjuntos com "e" · "se" passiva × indeterminado · existir × haver. Ainda pendentes: AA × CN (B3) e orações subordinadas (C)
4. Locução adjetiva × adverbial (28/10): errou 2/2 (Q7, Q8) e deixou em branco locução → adjetivo erudito. Em 30/10: classificou certo pelas setas, mas na contagem esqueceu a locução do início da frase (Q9). Valor semântico acertado com dúvida (Q8)
5. Morfologia A2 (novo, 30/10): o que o advérbio de intensidade modifica ("muito bem"), "-mente" coordenado (rápida e justamente), voz passiva (não sabia: SER + particípio), conjugação de derivados (reouve, intervier, mantiver), particípio de tempo composto não é adjetivo
6. Lógica da argumentação (atualizado 05/11): **setas certas, trava ao traduzir a alternativa** (palavra comum a todos virando letra, emenda sem fim = começo, "algum" = ficha). Silogismos com todo/algum/nenhum. Em 03/11, FGV oficiais: errou "quem é X faz Y" (= todo, seta) lido a partir de um "alguns", e "todo B é C" tomado como "C maior que B" (podem ser iguais); juntou fichas de "alguns" diferentes (militares). Contrapositiva 2/2. Antes (29/10): letras parecidas, "S' = V", recíproca aceita · validade × verdade. Falácias 2/2 em 29/10 (1/2 para sair)
7. Conjuntos e Venn (atualizado 04/11): bloco de 04/11 4/8. "Somente": meio tirado do círculo errado (escrever o nome do conjunto na conta) · equação do "dobro" com região subtraída (regiões sempre se somam) · ∈ × ⊂ ("?") · "exatamente um/dois/três" como fatias ("?"). 3 conjuntos "exatamente uma" e conjuntos em Python: acertos (1/2 para sair). Mínimo/máximo **fora do estudo** (decisão de 04/11)
8. Lógica proposicional (novo, 27/10): bicondicional com F ↔ F, contagem de linhas 2ⁿ, tautologia, condicional dada como falsa, "ou… ou" na dedução. Negações e equivalências: 4/4 em 27/10 (1/2 para sair; foram assistidas)
9. Regência verbal (lembrar/lembrar-se, obedecer a). Relativos (cujo, onde/aonde) passaram para o item 2 em 06/11
10. Conjunções pelo sentido (novo, 06/11): "e" adversativo (= mas) tomado como aditivo · "pois" posposto = conclusivo, errado **com certeza**. "De modo que" = consequência: acertou em 06/11 (era erro em 23/10; 1/2 para sair)
11. Interpretação: rótulo acrescentado pela alternativa, paradoxo, discurso direto × indireto. Opinião × fato: acertou em 28/10 (1/2 para sair)
12. Numeração de artigos de lei (novo, 28/10): ordinal até o 9º, cardinal do 10 em diante
13. Porcentagem e divisão proporcional
14. Semântica: vocabulário erudito (irascível, indelével). Conectivos passaram para o item 10
15. Raciocínio sequencial (filas, trocas, calendários)

### Técnico

0. **Estratégia "INCORRETA" (vale para todas as disciplinas; subiu em 05/11):** errada em 3 sessões seguidas (30/10 estimativa, 04/11 testes, 05/11 Português Q7 e Q14). Sempre marca ou deixa candidata uma alternativa **verdadeira**, sem V/F escrito. Pela pesquisa de 05/11, ~25% do Português FGV é negativo. Regra: V/F ao lado das 5 e circular a F. **06/11 (A3): voltou a escrever V/F (✓) em 3 das 4 negativas; 2/4, e os erros foram de conteúdo.** Manter no simulado de 08/11
1. Testes · técnicas de projeto de casos (novo, 04/11): 0/4. Valor-limite, partição de equivalência, caixa-branca × preta e estático × dinâmico com "?"; cobertura de decisões errada (1 caso True ≠ 100% de decisões). Também: confirmação × regressão invertidos e princípio "presença, não ausência" julgado falso. Níveis, alfa/beta, carga/estresse, stub/driver, ciclomática e pirâmide: ok
2. SAFe (novo, 06/11): 9/12, mas 7 acertos com dúvida. **Papéis RTE × Product Management** (facilita × prioriza) · **voto de confiança baixo** = os times retrabalham o plano no evento · **CD Pipeline** (Exploration = o quê; Deployment = produção) e deploy × release · System × Solution Demo ("?"). Firmes: hierarquia do backlog e ART
3. APF · funções de dados (novo, 03/11): 0/3. Confunde "o sistema usa ou grava" com "é um ALI separado": ação de gravar ≠ ALI, dado lido de outro sistema = AIE (mesmo banco não importa), entidade dependente = RLR, índice/backup não contam. Transações SE × CE: 2/2. VAF: conta fora do treino (05/11), só a regra dos 35
4. (Ver item 0.) Histórico da estratégia "INCORRETA" (voltou em 30/10 e em 04/11: na Q12 de testes deu ✓ em B e C, mas circulou a A, que era verdadeira; "certamente" na D era a pista): na Q8 de estimativa riscou a afirmação falsa (que era a resposta) e circulou uma verdadeira. Antes: 3/3 em 28/10. Escrever V/F e circular a F; nunca riscar a F
5. Estimativa ágil · velocidade (novo, 30/10): conta da média (63 ÷ 3 = 32), velocidade não compara equipes, item parcial não conta, Delphi = estimativas independentes, Cone da Incerteza (em branco). Conceitos de story points e Planning Poker: 7/7
6. Leitura de código (voltou em 30/10): ignorou `[-3:]` (fatiamento) e chutou. Rastrear linha a linha numa tabela, como em 28/10
7. RUP · perspectivas dinâmica/estática/prática: em branco 2× (24 e 26/10). Fases: acertou em 26/10 (1/2)
8. Scaling up × out: errou 24 e 26/10
9. TDD × ATDD × BDD (novo, 28/10): em branco. Inseguro no ATDD
10. Modelos de processo: espiral × prototipação e prototipação na elicitação (erros de 26/10, ainda não recobrados). Modelo em V: acertou em 28/10 (1/2 para sair)
11. Scrum · responsabilidades: errou 22 e 26/10; acertou o dono do Sprint Backlog em 28/10 (1/2 para sair). Artefatos × compromissos: acertou em 26/10 por chute (não conta)
12. Kanban · lead × cycle time: acertou em 28/10 (1/2 para sair)
13. Subtipos de RNF: acertou em 26/10 (1/2 para sair)
14. XP · práticas: acertou em 26/10 (1/2 para sair)
15. Estratégia de prova: nunca deixar em branco (Q6 em 28/10 manhã e Q8 em 28/10 noite: em I/II/III, julgar os itens que sabe e eliminar) e **reler a alternativa antes de marcar** (2 erros de atenção em RLM em 27/10). "Incorreta" com V/F: 3/3 em 28/10
- Leitura de código saiu da lista em 28/10 e **voltou em 30/10** (Q6 de estimativa).

---

## Fila de pendências (regra de 04/11)

> A fila manda, não o calendário (ver "Fila de estudo" no `CLAUDE.md`). Dia perdido = a fila não anda. Um item só sai com **teoria + bloco corrigido**. Atraso se paga cortando ⚪ (e depois 🟡), nunca dobrando a carga.

**Português · almoço (Módulo 0, base: não pular)**

| # | Item | Nível | Situação |
|---|---|---|---|
| 3 | **B3:** termos acessórios (adjuntos, aposto, vocativo, complemento nominal) + revisão do Módulo 0 | 🔴 base | **Próximo** (seg 09/11, almoço). Na revisão do Módulo 0, incluir pronomes (para eu × para mim, o × lhe, relativo + preposição) |
| → | Depois: **D. Concordância** (previsão: a partir de 10/11) | 🔴 | Ordem em discussão (05/11): a pesquisa FGV sugere coesão (G) e texto/argumentação (H) antes de concordância. Decidir com o Tiago |

- ✅ **B1 + B2 saiu da fila em 05/11** (bloco 7/15; predicativo e OD × OI ficam como ponto fraco).
- ✅ **A3 saiu da fila em 06/11** (bloco 8/15; pronomes e conjunções pelo sentido ficam como ponto fraco).

**Específicas · noite**

| # | Item | Nível | Situação |
|---|---|---|---|
| 7 | **SAST × DAST × IAST, SonarQube** | 🟡 | **06/11: sem bloco, a pedido** (diz já conhecer o assunto). Fica pendente como leitura para revisar (mapa curto ou 5 FGV reais quando sobrar tempo). Primeiro a ir para o fim da fila se apertar |
| 8 | **APF:** 5 a 10 questões reais só de funções de dados (ALI, AIE, RLR) | 🔴 reforço | Sábado 07/11 |
| 9 | ⚪ SDD · agilidade organizacional | ⚪ | Leitura de 1 página cada, ou corta. **Pact e mutation testing cortados em 05/11** (a pedido; nenhuma questão FGV achada) |

- ✅ **Requisitos saiu da fila em 06/11, a pedido** (teoria na Semana 1 e questões nos blocos corrigidos de 24/10 e 26/10: RF × RNF, usuário × sistema, subtipos de RNF, prototipação na elicitação, V&V). Treinado pouco: técnicas de elicitação, regras de negócio e **contagem de RF/RNF num depoimento** (caiu no TJ-RJ 2026 e no MPU 2025). Cobrar nos blocos de revisão e nos simulados.
- ✅ **SAFe saiu da fila em 06/11** (bloco 9/12; papéis, voto de confiança e CD Pipeline ficam como ponto fraco).
- **Revisão da Semana 1** (era 31/10): absorvida pelo simulado de 08/11. Não dobrar.
- **RLM:** conjuntos e Venn fechados em 04/11 (sem mín/máx). Próximo pelo mapa: porcentagem, razão e proporção (ter/qui no almoço, depois do Módulo 0).

## Próximos passos

| Dia | O que fazer |
|---|---|
| Seg 26/10 · 22:40 | Reler as 7 regras 📌 dos erros da prova de hoje. Anki: "RUP dinâmica × estática × prática", "Scaling up × out", "Lead × cycle time", "V: qual teste para qual fase?", "Dono do Sprint Backlog" |
| Ter 27/10 | ✅ Almoço/tarde: bloco RLM conectivos (8/15). Bloco 1: RF × RNF × regras de negócio + 10 min de RUP (seção 3.6 do mapa). Bloco 2: questões FGV de requisitos + 5 de Kanban. 22:40: reler as 7 regras 📌 do bloco RLM e refazer Q6, Q7 e Q15 sem olhar |
| Qua 28/10 | ✅ Almoço/tarde: Módulo 0 A1 + bloco Português classes de palavras (9/15). ✅ Noite: user stories, INVEST e BDD (13/15). Revisão 22:40: regras 📌 da Q8 (TDD × ATDD × BDD) e da Q15 ("em anexo", "é necessário paciência"); regras 📌 do bloco de hoje + refazer Q7, Q8, Q10 e Q14 sem olhar; escrever 3 frases com "é proibido/proibida" e 3 com "anexo/anexas/em anexo". Revisão espaçada de 7 dias das regras de 21/10 + refazer Q8 e Q10 do bloco RLM |
| Qui 29/10 | ✅ Almoço/tarde: em vez de negações (já feitas em 27/10), RLM argumentação e diagramas (item 2 do mapa de RLM): teoria + 11 exemplos + bloco (9/15). Noite: cansado, só Anki ✅ (41 cartões de 28/10 e 29/10 criados). Estimativa ágil adiada para sexta |
| Sex 30/10 | ✅ Videoaulas + bloco Português A2 (8/15) e bloco estimativa ágil (10/15). Revisão 22:40: regras 📌 de hoje (Q5, Q6, Q9, Q10 e Q14 do A2; Q5, Q6, Q8, Q11 e Q15 de estimativa), 5 frases com "em anexo" e 5 com "anexo(s)/anexa(s)", refazer as contas da Q5 e da Q6 sem olhar |
| Sáb 31/10 | Almoço: Módulo 0 A3 (pronome, preposição, conjunção); abrir o bloco A3 com 1 questão de "em anexo" e 1 de voz passiva. Bloco 1: SDD (leitura leve). Bloco 2: **RLM conjuntos e Venn** (2 e 3 conjuntos, "no mínimo/no máximo"; ficou em branco em 29/10). Noite: Anki de estimativa ágil + Português A2 |
| Dom 01/11 · 13h | ⏸️ Não feito (pausa por burnout, 31/10–02/11). Remarcado para dom 08/11. **1º simulado oficial** (cronometrado, sem consulta, prova FGV inédita) + discursiva **autoral do Claude** sobre assunto já estudado (Eng. Software/Ágil), entregue fechada e corrigida com rigor de banca (combinado em 28/10; não usar a discursiva da prova). Objetiva 13h–16h, discursiva 16h–17h. Meta: zero questões em branco, "?" nos chutes e reler cada alternativa de lógica antes de marcar. Enviar respostas e gabarito para correção |
| Ter 03/11 | ✅ Tarde: RLM conjuntos e Venn (bloco 15 autorais, respostas pendentes) + silogismos (4 de videoaula) + 7 FGV oficiais (4/6). Criado o bloco 02 de Venn (15 autorais, foco em mínimo/máximo) para outro dia. ✅ Noite: APF/IFPUG (teoria no chat + bloco 3/8). 22:40: regras 📌 de APF de 03/11 (refazer Q4 do VAF e Q2 das telas sem olhar) + regras de Venn e Q4/Q5 do bloco 01 com o "sugar" |
| Qua 04/11 | ✅ Manhã: bloco curto de Venn sem mín/máx (4/8). ✅ Regra da fila criada (`CLAUDE.md`) e mapas ajustados. Almoço: B1 + B2 (teoria dada; falta tipos de sujeito + bloco). ✅ Noite: Requisitos adiado para sábado (a pedido) → **Tipos de teste**: videoaula + bloco (8/15); saiu da fila. 22:40: regras 📌 de testes (Q3, Q4, Q5, Q6, Q9, Q12, Q13) + refazer Q3/Q4 com a faixa [18, 70] e o 2º caso da Q6 sem olhar + Anki de testes; regras de conjuntos de 04/11. Bloco 01 de Venn (03/11): opcional, pulando Q4, Q5 e Q15. APF volta no sábado: 5 a 10 questões reais FGV/Cebraspe só de funções de dados (ALI, AIE, RLR) |
| Qui 05/11 | ✅ Manhã: Anki de silogismos + autoral no chat. ✅ Tarde: Anki zerado (AnkiWeb), guia de estilo FGV, **bloco Português B1 + B2 (7/15)**; saiu da fila. Noite: **SAFe** (item 6). Antes, 10 min: refazer Q9 e Q13 de testes de cabeça. 22:40: regras 📌 do B1 + B2 (Q3, Q5, Q7, Q8, Q10, Q12, Q13, Q14) + refazer Q12 (teste da concordância), Q13 (teste do pronome) e Q14 com V/F |
| Sex 06/11 | ✅ Bloco SAFe corrigido (9/12). ✅ Tarde: **A3** (8/15); saiu da fila. Ainda à tarde (para liberar a noite): **SAST × DAST × IAST, SonarQube** (item 7): liga com estático × dinâmico (Q13 de testes); antes, 5 min no mapa SAFe (papéis e CD Pipeline). 22:40: regras 📌 de SAFe e do A3 (06/11) + refazer Q1, Q3 e Q11 de SAFe e Q8, Q13 e Q15 do A3 sem olhar |
| Sáb 07/11 | Dia de recuperação: zerar o que sobrou da fila → **bloco de Requisitos** (item 4, adiado) → APF real (item 8) → se sobrar, 5 FGV reais de técnicas de teste (valor-limite, partição, cobertura) → leitura ⚪ (item 9). Sem passar do horário normal |
| Dom 08/11 · 13h | **1º simulado oficial** (remarcado de 01/11): prova FGV inédita (TJ-MS 2024 ou TJ-AP 2024), cronometrada e sem consulta, + discursiva autoral (estudo de caso) entregue fechada. "?" nos chutes, nada em branco |

- **Almoço (Português · Módulo 0 de base, combinado em 28/10; virou fila em 04/11):** A1 ✅ 28/10 · A2 ✅ 30/10 · B1 + B2 ✅ 05/11 · A3 ✅ 06/11 · falta B3 + revisão. Depois: D concordância (previsão 10–13/11) → F pontuação (16–20/11) → C período (23–27/11) → E regência, crase e colocação (30/11–04/12). Questões FGV só depois do Módulo 0; até lá, autorais básicas.

- **Ter e qui no almoço:** alternar argumentação/falácias e porcentagem/proporção.
- **Anki (29/10, noite):** ✅ 41 cartões criados no PC de casa (25 de 28/10 + 16 de 29/10; cópias em `anki/`). Total no Anki: 102. Faltam os cartões de 30/10 (Português A2 e estimativa ágil): criar no sábado. Ao criar a conta AnkiWeb: **enviar (upload) do PC de casa; nos aparelhos novos, baixar (download)**, para não apagar o histórico.
- **Anki (criar):** verbos de regência (lembrar, esquecer, simpatizar, obedecer, residir, pagar, perdoar, assistir, visar, aspirar, preferir, implicar) · adjetivos eruditos (irascível, indelével, imiscível, inefável, inócuo, iníquo, profícuo, perene) · figuras de linguagem (paradoxo, antítese, ironia, metáfora).
- **Hábitos de prova:** em "incorreta", escrever V/F ao lado de cada alternativa · em interpretação, sublinhar a palavra que a alternativa acrescenta · só trocar resposta com regra concreta · pontinho ao lado = candidata sem certeza (eliminação, para não reler o que já descartei) · **silogismo (29/10):** legenda com letras de inícios diferentes, ficha com a letra positiva (S = F), seta virada já com os dois apóstrofos, apontar letra da alternativa ↔ ficha antes de marcar. Os erros de 29/10 foram de anotação, não de raciocínio. O Tiago não vai pedir atendimento especial (decisão dele em 29/10).
- **Leitura de código:** incluir 2 a 3 questões por semana desde já, mesmo antes da Semana 3.
