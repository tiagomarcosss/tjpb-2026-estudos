# Contexto de Estudo · TJPB 2026

**Atualizado em:** 27/10/2026 · **Semana do plano:** 1 (Engenharia de Software e Ágil)

> Arquivo substituído toda semana. Regras estudadas ficam em "regras-tjpb". Plano e conteúdo por semana ficam em "plano-tjpb".

---

## Situação atual

- Semana 0 (21–25/10): inscrição, caderno de erros, Anki e diagnóstico.
- **1ª retificação do edital (23/10):** jornada 30h · isenção da taxa só até 27/10, 16h · inscrição segue até 18/11, 16h. Plano atualizado para a versão 3 em 26/10. Inscrição: ainda não confirmada.
- Adiantando a Semana 1 (Engenharia de Software e Ágil) desde 22/10.
- Estudo sem cursinho: fontes oficiais + banco de questões (QConcursos/TEC) + Claude como professor e corretor de discursiva. Pacotes pós-edital ainda não lançados.
- Questões autorais salvas em .md na pasta "QUESTÕES NÃO OFICIAIS" (blocos em `Provas/`: `AAAA-MM-DD_Semana-XX_Bloco-XX_Assunto.md`; correções em `Correções/`: `_CORRECAO.md`). Provas oficiais seguem a mesma divisão.
- Simulados: todo domingo, 13h–17h, + 1 discursiva + 1h de correção. Em janeiro, 13h–18h.
- 1º simulado: domingo 25/10, prova FGV TRT-16 2022 (Analista Judiciário – TI). Pular Legislação e Atualidades.

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
- **25/10 · Simulado TRT-16 2022:** Port __/10 · RLM __/10 · Específicas __/40 · Discursiva __/40
  - Erros: __
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

---

## Pontos fracos (prioridade)

### Português / RLM

1. Sintaxe (base): termos da oração, predicação verbal, AA × CN, orações subordinadas
2. Concordância verbal e nominal pela norma-padrão (≈50% do Português FGV)
3. Lógica da argumentação: silogismos, validade, falácias. Validade acertada em 27/10 (Q12); cadeia de condicionais errada por pressa (Q11)
4. Lógica proposicional (novo, 27/10): bicondicional com F ↔ F, contagem de linhas 2ⁿ, tautologia, condicional dada como falsa, "ou… ou" na dedução. Negações e equivalências: 4/4 em 27/10 (1/2 para sair; foram assistidas)
5. Regência verbal e pronomes relativos (lembrar/lembrar-se, obedecer a, cujo, onde/aonde)
6. Interpretação: opinião × fato, rótulo acrescentado pela alternativa, paradoxo, discurso direto × indireto
7. Porcentagem e divisão proporcional
8. Semântica: conectivos ("de modo que"), vocabulário erudito (irascível, indelével)
9. Raciocínio sequencial (filas, trocas, calendários)

### Técnico

1. RUP · perspectivas dinâmica/estática/prática: em branco 2× (24 e 26/10). Fases: acertou em 26/10 (1/2)
2. Scrum · responsabilidades (dono do Sprint Backlog, quem decide o quê): errou 22 e 26/10. Artefatos × compromissos: acertou em 26/10 por chute (não conta)
3. Scaling up × out: errou 24 e 26/10
4. Modelos de processo (novo): espiral × prototipação, modelo em V (qual teste para qual fase), prototipação na elicitação. Errou 3/3 em 26/10
5. Kanban (novo): lead time × cycle time. Errou em 26/10
6. Leitura de código: 2/2 em 26/10 (1/2 para sair)
7. Subtipos de RNF: acertou em 26/10 (1/2 para sair)
8. XP · práticas: acertou em 26/10 (1/2 para sair)
9. Estratégia de prova: "incorreta" (errou Q3 em 26/10 por conteúdo, mas marcou "?" na certa), nunca deixar em branco e **reler a alternativa antes de marcar** (2 erros de atenção em RLM em 27/10)

---

## Próximos passos

| Dia | O que fazer |
|---|---|
| Seg 26/10 · 22:40 | Reler as 7 regras 📌 dos erros da prova de hoje. Anki: "RUP dinâmica × estática × prática", "Scaling up × out", "Lead × cycle time", "V: qual teste para qual fase?", "Dono do Sprint Backlog" |
| Ter 27/10 | ✅ Almoço/tarde: bloco RLM conectivos (8/15). Bloco 1: RF × RNF × regras de negócio + 10 min de RUP (seção 3.6 do mapa). Bloco 2: questões FGV de requisitos + 5 de Kanban. 22:40: reler as 7 regras 📌 do bloco RLM e refazer Q6, Q7 e Q15 sem olhar |
| Qua 28/10 | Plano: user stories (INVEST) + Gherkin. Revisão: refazer Q1, Q2, Q11 e Q13 da prova de 26/10 sem olhar. Revisão espaçada de 7 dias das regras de 21/10 + refazer Q8 e Q10 do bloco RLM |
| Qui 29/10 | Almoço: RLM, 10 questões FGV de equivalências e negações (QConcursos/TEC), pelo método de Boole. Depois, seção 4.1 do plano |
| Sex 30/10 → Sáb 31/10 | Seguir a seção 4.1 do plano (estimativa, SDD, revisão da semana). Sáb no almoço: RLM argumentação e diagramas (todo/algum/nenhum) |
| Dom 01/11 · 13h | Simulado + discursiva. Meta: zero questões em branco e reler cada alternativa de lógica antes de marcar |
| Pendente | Placar do simulado TRT-16 de 25/10 (Port · RLM · Específicas · Discursiva) |

- **Almoço (Português, 10 questões FGV por dia):**

| Semana | Seg | Qua | Sex |
|---|---|---|---|
| 26–30/10 | Termos da oração + predicação | AA × CN | Orações subordinadas |
| 02–06/11 | Concordância verbal | Concordância nominal | Pontuação |
| 09–13/11 | Semântica, conectivos, reescritura | Verbo: tempos, modos, vozes | Regência e crase |

- **Ter e qui no almoço:** alternar argumentação/falácias e porcentagem/proporção.
- **Anki (criar):** verbos de regência (lembrar, esquecer, simpatizar, obedecer, residir, pagar, perdoar, assistir, visar, aspirar, preferir, implicar) · adjetivos eruditos (irascível, indelével, imiscível, inefável, inócuo, iníquo, profícuo, perene) · figuras de linguagem (paradoxo, antítese, ironia, metáfora).
- **Hábitos de prova:** em "incorreta", escrever V/F ao lado de cada alternativa · em interpretação, sublinhar a palavra que a alternativa acrescenta · só trocar resposta com regra concreta.
- **Leitura de código:** incluir 2 a 3 questões por semana desde já, mesmo antes da Semana 3.
