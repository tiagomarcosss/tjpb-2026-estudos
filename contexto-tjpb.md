# Contexto de Estudo · TJPB 2026

**Atualizado em:** 29/10/2026 · **Semana do plano:** 1 (Engenharia de Software e Ágil)

> Arquivo substituído toda semana. Regras estudadas ficam em "regras-tjpb". Plano e conteúdo por semana ficam em "plano-tjpb".

---

## Situação atual

- Semana 0 (21–25/10): inscrição, caderno de erros, Anki e diagnóstico.
- **1ª retificação do edital (23/10):** jornada 30h · isenção da taxa só até 27/10, 16h · inscrição segue até 18/11, 16h. Plano atualizado para a versão 3 em 26/10. Inscrição: ainda não confirmada.
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

---

## Pontos fracos (prioridade)

### Português / RLM

1. Concordância nominal pela norma-padrão (≈50% do Português FGV): errada **3×** (23/10, 28/10 manhã e 28/10 noite), sempre pelo uso comum. Na 3ª já eliminou "anexo", "é proibido a" e "meias", mas errou "em anexo" (invariável) e "é necessário paciência" (certo, sem artigo). Olhar primeiro se há artigo
2. Sintaxe (base): termos da oração, predicação verbal, AA × CN, orações subordinadas
3. Locução adjetiva × adverbial (novo, 28/10): errou 2/2 (Q7, Q8) e deixou em branco locução → adjetivo erudito
4. Lógica da argumentação (atualizado 29/10): silogismos com todo/algum/nenhum 2/5 (erros de anotação: letras parecidas, "S' = V", contrapositiva sem negar os dois lados, recíproca aceita) · validade × verdade (achou que conclusão V torna válido) · formas da condicional ok (tollens, afirmar consequente). Falácias 2/2 em 29/10 (1/2 para sair)
5. Conjuntos e Venn (novo, 29/10): em branco 2/2 (contagem com "nenhum" e operações de conjunto em Python). Não estudado
6. Lógica proposicional (novo, 27/10): bicondicional com F ↔ F, contagem de linhas 2ⁿ, tautologia, condicional dada como falsa, "ou… ou" na dedução. Negações e equivalências: 4/4 em 27/10 (1/2 para sair; foram assistidas)
7. Regência verbal e pronomes relativos (lembrar/lembrar-se, obedecer a, cujo, onde/aonde)
8. Interpretação: rótulo acrescentado pela alternativa, paradoxo, discurso direto × indireto. Opinião × fato: acertou em 28/10 (1/2 para sair)
9. Numeração de artigos de lei (novo, 28/10): ordinal até o 9º, cardinal do 10 em diante
10. Porcentagem e divisão proporcional
11. Semântica: conectivos ("de modo que"), vocabulário erudito (irascível, indelével)
12. Raciocínio sequencial (filas, trocas, calendários)

### Técnico

1. RUP · perspectivas dinâmica/estática/prática: em branco 2× (24 e 26/10). Fases: acertou em 26/10 (1/2)
2. Scaling up × out: errou 24 e 26/10
3. TDD × ATDD × BDD (novo, 28/10): em branco. Inseguro no ATDD
4. Modelos de processo: espiral × prototipação e prototipação na elicitação (erros de 26/10, ainda não recobrados). Modelo em V: acertou em 28/10 (1/2 para sair)
5. Scrum · responsabilidades: errou 22 e 26/10; acertou o dono do Sprint Backlog em 28/10 (1/2 para sair). Artefatos × compromissos: acertou em 26/10 por chute (não conta)
6. Kanban · lead × cycle time: acertou em 28/10 (1/2 para sair)
7. Subtipos de RNF: acertou em 26/10 (1/2 para sair)
8. XP · práticas: acertou em 26/10 (1/2 para sair)
9. Estratégia de prova: nunca deixar em branco (Q6 em 28/10 manhã e Q8 em 28/10 noite: em I/II/III, julgar os itens que sabe e eliminar) e **reler a alternativa antes de marcar** (2 erros de atenção em RLM em 27/10). "Incorreta" com V/F: 3/3 em 28/10
- Saiu da lista em 28/10: **leitura de código** (acertou em 26/10 e 28/10, duas sessões seguidas). Continua sendo treinada quando couber no assunto ou na revisão

---

## Próximos passos

| Dia | O que fazer |
|---|---|
| Seg 26/10 · 22:40 | Reler as 7 regras 📌 dos erros da prova de hoje. Anki: "RUP dinâmica × estática × prática", "Scaling up × out", "Lead × cycle time", "V: qual teste para qual fase?", "Dono do Sprint Backlog" |
| Ter 27/10 | ✅ Almoço/tarde: bloco RLM conectivos (8/15). Bloco 1: RF × RNF × regras de negócio + 10 min de RUP (seção 3.6 do mapa). Bloco 2: questões FGV de requisitos + 5 de Kanban. 22:40: reler as 7 regras 📌 do bloco RLM e refazer Q6, Q7 e Q15 sem olhar |
| Qua 28/10 | ✅ Almoço/tarde: Módulo 0 A1 + bloco Português classes de palavras (9/15). ✅ Noite: user stories, INVEST e BDD (13/15). Revisão 22:40: regras 📌 da Q8 (TDD × ATDD × BDD) e da Q15 ("em anexo", "é necessário paciência"); regras 📌 do bloco de hoje + refazer Q7, Q8, Q10 e Q14 sem olhar; escrever 3 frases com "é proibido/proibida" e 3 com "anexo/anexas/em anexo". Revisão espaçada de 7 dias das regras de 21/10 + refazer Q8 e Q10 do bloco RLM |
| Qui 29/10 | ✅ Almoço/tarde: em vez de negações (já feitas em 27/10), RLM argumentação e diagramas (item 2 do mapa de RLM): teoria + 11 exemplos + bloco (9/15). Noite: estimativa ágil (Planning Poker, story points, T-shirt) + bloco só desse assunto. 22:40: Anki (cartões de 28/10 + os de hoje) e refazer Q10 e Q14 do bloco RLM sem olhar |
| Sex 30/10 → Sáb 31/10 | Almoço: Módulo 0. Sex A2 (verbo, advérbio, **locuções adverbiais**: fecha os erros de Q7 e Q8 de 28/10) · Sáb A3 (pronome, preposição, conjunção). Resto: seção 4.1 do plano (estimativa, SDD, revisão da semana). Sábado, Bloco 2: **RLM conjuntos e Venn** (2 e 3 conjuntos, "no mínimo/no máximo"; ficou em branco em 29/10) no lugar da argumentação, que já foi feita |
| Dom 01/11 · 13h | **1º simulado oficial** (cronometrado, sem consulta, prova FGV inédita) + discursiva **autoral do Claude** sobre assunto já estudado (Eng. Software/Ágil), entregue fechada e corrigida com rigor de banca (combinado em 28/10; não usar a discursiva da prova). Objetiva 13h–16h, discursiva 16h–17h. Meta: zero questões em branco, "?" nos chutes e reler cada alternativa de lógica antes de marcar. Enviar respostas e gabarito para correção |

- **Almoço (Português · Módulo 0 de base, combinado em 28/10):** qua 28/10 A1 ✅ · sex 30/10 A2 (verbo, advérbio, locuções) · sáb 31/10 A3 (pronome, preposição, conjunção) · seg 02/11 B1 (sujeito e predicado) · qua 04/11 B2 (verbo e complementos) · sex 06/11 B3 (termos acessórios) + revisão. Depois: D concordância (09–13/11) → F pontuação (16–20/11) → C período (23–27/11) → E regência, crase e colocação (30/11–04/12). Questões FGV só a partir de 09/11; até lá, autorais básicas.

- **Ter e qui no almoço:** alternar argumentação/falácias e porcentagem/proporção.
- **⏰ LEMBRAR NA REVISÃO DAS 22:40 DE 29/10 (adiado pelo Tiago no almoço):** criar no Anki os cartões de 28/10 (user stories, INVEST, critério × DoD, Gherkin, BDD × TDD × ATDD, concordância "em anexo" / "é necessário") e os de 29/10 (RLM argumentação: conversão todo/nenhum/algum, ficha do x × setas, contrapositiva × recíproca, validade × verdade, formas válidas, falácias, Venn e conjuntos em Python; e estimativa ágil, se o bloco da noite sair). O Tiago vai criar a conta AnkiWeb e sincronizar: **primeiro sincronizar e enviar (upload) do PC que já tem os 61 cartões; nos aparelhos novos, escolher baixar (download)**, para não apagar o histórico.
- **Anki (criar):** verbos de regência (lembrar, esquecer, simpatizar, obedecer, residir, pagar, perdoar, assistir, visar, aspirar, preferir, implicar) · adjetivos eruditos (irascível, indelével, imiscível, inefável, inócuo, iníquo, profícuo, perene) · figuras de linguagem (paradoxo, antítese, ironia, metáfora).
- **Hábitos de prova:** em "incorreta", escrever V/F ao lado de cada alternativa · em interpretação, sublinhar a palavra que a alternativa acrescenta · só trocar resposta com regra concreta · pontinho ao lado = candidata sem certeza (eliminação, para não reler o que já descartei) · **silogismo (29/10):** legenda com letras de inícios diferentes, ficha com a letra positiva (S = F), seta virada já com os dois apóstrofos, apontar letra da alternativa ↔ ficha antes de marcar. Os erros de 29/10 foram de anotação, não de raciocínio. O Tiago não vai pedir atendimento especial (decisão dele em 29/10).
- **Leitura de código:** incluir 2 a 3 questões por semana desde já, mesmo antes da Semana 3.
