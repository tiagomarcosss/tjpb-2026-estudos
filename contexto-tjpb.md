# Contexto de Estudo · TJPB 2026

**Atualizado em:** 24/10/2026 · **Semana do plano:** 0 (adiantando a Semana 1)

> Arquivo substituído toda semana. Regras estudadas ficam em "regras-tjpb". Plano e conteúdo por semana ficam em "plano-tjpb".

---

## Situação atual

- Semana 0 (21–25/10): inscrição, caderno de erros, Anki e diagnóstico.
- Adiantando a Semana 1 (Engenharia de Software e Ágil) desde 22/10.
- Estudo sem cursinho: fontes oficiais + banco de questões (QConcursos/TEC) + Claude como professor e corretor de discursiva. Pacotes pós-edital ainda não lançados.
- Questões autorais salvas em .md na pasta "QUESTÕES NÃO OFICIAIS" (padrão: `AAAA-MM-DD_Semana-XX_Bloco-XX_Assunto.md` + `_CORRECAO.md`).
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
  - Arquivos: `PROVAS OFICIAIS (estudo)/2026-10-23_Semana-00_FGV-DATAPREV_Portugues_*` (prova, PDF original, correção v3).
  - Meta para a próxima prova de Português: ≥ 5/12, nenhuma em branco por desconhecimento.
- **24/10 · Bloco Eng. Software UNIVESP Aulas 01–05 (14 autorais, PDF anotado à mão):** 9/14 (64%) · 3 erros · 2 em branco
  - Acertos: atividades do processo, cascata, incremental ("incorreta"), reuso (I/II/III), Manifesto Ágil, ágil × planos, test-first, requisito de usuário × sistema, RNF ("incorreta").
  - Em branco (não estudado): RUP · fases (Elaboração) e 3 perspectivas.
  - Erros: XP (aceitei "propriedade coletiva = um dono"; descartei histórias de usuário achando que era só Scrum), scaling up × out, RNF de produto × organizacional (invertidos).
  - Evolução: "assinale a incorreta" 2/2 usando V/F ao lado (era erro na DATAPREV); modelos de processo acertados de novo.
  - Arquivo: `QUESTÕES NÃO OFICIAIS/2026-10-23_Semana-01_Bloco-01_EngSoftware-UNIVESP-Aulas01a05_CORRECAO_v2.md` (+ .pdf)
- **25/10 · Simulado TRT-16 2022:** Port __/10 · RLM __/10 · Específicas __/40 · Discursiva __/40
  - Erros: __
- **Evolução:** — (ponto de partida)
- **Observação:** no TRT-16, Português de Analista cobrou mais argumentação, inferência e organização textual do que gramática pura.

---

## Pontos fracos (prioridade)

### Português / RLM

1. Sintaxe (base): termos da oração, predicação verbal, AA × CN, orações subordinadas
2. Concordância verbal e nominal pela norma-padrão (≈50% do Português FGV)
3. Lógica da argumentação: silogismos, validade, falácias
4. Regência verbal e pronomes relativos (lembrar/lembrar-se, obedecer a, cujo, onde/aonde)
5. Interpretação: opinião × fato, rótulo acrescentado pela alternativa, paradoxo, discurso direto × indireto
6. Porcentagem e divisão proporcional
7. Semântica: conectivos ("de modo que"), vocabulário erudito (irascível, indelével)
8. Raciocínio sequencial (filas, trocas, calendários)

### Técnico

1. Leitura de código: rastrear a saída de trechos (Java, Python, JS)
2. RUP: fases × produtos (Elaboração = arquitetura) e perspectivas dinâmica/estática/prática (não estudado)
3. Subtipos de RNF: produto × organizacional × externo
4. XP: práticas (propriedade coletiva, ritmo sustentável, histórias + cliente no local) e scaling up × out
5. Scrum: responsabilidades dos papéis (quem decide o quê) e artefatos × compromissos
6. Estratégia de prova: V/F com itens I, II, III e "assinale a incorreta" (julgar cada alternativa V/F; não trocar resposta sem regra). Melhorou em 24/10 (2/2 "incorreta")

---

## Próximos passos

| Dia | O que fazer |
|---|---|
| Sex 23/10 | Ler o Guia do Scrum 2020 inteiro + 10 questões FGV de Scrum (papéis e eventos). Anki: "Quem cancela a Sprint?", "3 artefatos e compromissos", "Review × Retro" |
| Sáb 24/10 | 30 min de RUP (Sommerville cap. 2: fases × produtos, 3 perspectivas) + 5 questões FGV de RUP. Depois Kanban (WIP, lead time, cycle time) + Lean (7 desperdícios) + questões. Videoaula de 20 min: termos da oração. Anki: "Produto da Elaboração", "RUP dinâmica × estática × prática", "Scaling up × out", "RNF produto × organizacional × externo" |
| Dom 25/10 · 13h | Simulado TRT-16 2022 + 1 discursiva + 1h de correção. Trazer placar por disciplina e erros |
| Seg 26/10 → Dom 01/11 | Seguir a ordem da Semana 1 na seção 4.1 do plano. Ter 27/10 (RF × RNF): reforçar subtipos de RNF ("quem exige isso?") |

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
