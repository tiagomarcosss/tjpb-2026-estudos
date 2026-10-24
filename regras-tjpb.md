# Regras Estudadas · TJPB 2026

**Atualizado em:** 24/10/2026

> Arquivo acumulativo: só recebe acréscimos, no fim da seção certa. Uma regra por linha. Usado para revisão espaçada.
> Data entre colchetes = quando a regra entrou.

---

## Português

- [21/10] Opinião × fato: adjetivo avaliativo indica opinião.
- [21/10] Cujo: sem artigo depois, indica posse, concorda com a coisa possuída.
- [23/10] Teste da subordinada: troca por "isso" = substantiva · caracteriza um nome = adjetiva · troca por advérbio = adverbial.
- [23/10] "É preciso / é necessário / é bom + infinitivo" = oração substantiva subjetiva reduzida de infinitivo.
- [23/10] Adjunto adnominal × complemento nominal: sem preposição = AA · completa adjetivo ou advérbio = CN · com substantivo: agente/possuidor = AA, paciente = CN.
- [23/10] Verbo de ligação depende do que vem depois: característica (adjetivo) = estado · lugar ou modo = intransitivo ("ficou à janela").
- [23/10] Regência: lembrar algo / lembrar-se de algo ("lembrar de" é erro) · simpatizar não é pronominal · obedecer a · residir em · pagar a alguém (paguei-lhe).
- [23/10] Concordância: é proibido entrada (sem artigo) × é proibida a entrada (com artigo) · anexo concorda · meio (= um pouco) não varia.
- [23/10] "De modo que" + indicativo = consequência · + subjuntivo = finalidade.
- [23/10] Vírgula separa oração adverbial anteposta. Oração tem verbo; adjunto adverbial ("No dia seguinte") não.
- [23/10] Irascível = que se irrita fácil (de "ira"). Nem todo "i-" inicial é negação.
- [23/10] Paradoxo = ideias opostas que convivem. Alternativa que repete o texto e acrescenta rótulo (irônico, negativo) ou extrapola (impossível, sempre) é suspeita.
- [23/10] Discurso direto = fala preservada e separada (travessão, aspas, verbo de elocução). "Narrador interpreta/absorve a fala" = discurso indireto.
- [23/10] Variação linguística: a FGV nunca aceita tratar a variante como "desprestigiada" ou "pobre".

## Raciocínio Lógico-Matemático

### Lógica proposicional

- [21/10] Se A, então B: válidos → "A, logo B" e "não B, logo não A". Inválidos → "B, logo A" e "não A, logo não B".
- [21/10] Negação de "se A, então B" = "A e não B" (nunca outra condicional).
- [21/10] "Não A ou B" equivale a "se A, então B".
- [21/10] "A ou B" + não B → logo A.
- [21/10] Se e somente se: as duas partes são sempre iguais (ambas V ou ambas F).
- [21/10] Encadeamento: começar pela premissa solta; sem premissa solta, supor uma afirmação e buscar contradição.

### Quantificadores e argumentação

- [21/10] "Nenhum A é B" equivale a "se A, então não B".
- [21/10] Todo/algum/nenhum: desenhar círculos (diagramas), não usar tabela de conectivos.
- [21/10] "Todo A é B" equivale a "todo não B é não A" (não equivale a "todo B é A").
- [21/10] Generalização: poucos casos → todos. Falsa causa: causa errada para um fato.

### Matemática

- [21/10] Porcentagem com mudança no grupo: montar "parte = % × total" com os valores depois da mudança.
- [21/10] Divisão proporcional: somar as proporções → dividir o total → multiplicar pela parte pedida.

### Raciocínio sequencial

- [21/10] Filas com trocas: letras no papel, reescrevendo a fila a cada troca.

---

## Engenharia de Software e Ágil

### Modelos de processo (SDLC)

- [22/10] Cascata: sequencial, requisitos estáveis, feedback tardio, forte documentação entre fases.
- [22/10] Incremental = adiciona partes prontas · Iterativo = refina o mesmo produto · Espiral = guiado por risco · Prototipação = valida requisitos.
- [22/10] Ágil = iterativo + incremental.
- [22/10] RUP: Concepção → Elaboração (arquitetura) → Construção → Transição.
- [24/10] 4 atividades fundamentais de todo processo (Sommerville): especificação · projeto e implementação · validação · evolução.
- [24/10] Incremental: processo pouco visível (não compensa documentar cada versão), estrutura degrada sem refatoração; menos indicado para sistemas grandes, de vida longa e com várias equipes.
- [24/10] Integração e configuração (reuso): menos custo e risco, entrega rápida; mas exige concessão nos requisitos e perde o controle sobre a evolução dos componentes.
- [24/10] RUP · Elaboração = maioria dos casos de uso + descrição da arquitetura + plano de desenvolvimento, riscos principais tratados. Concepção = caso de negócio.
- [24/10] RUP · 3 perspectivas: dinâmica = fases no tempo · estática = workflows (atividades) · prática = boas práticas. Todo workflow pode ocorrer em qualquer fase; cada fase tem iterações.
- [24/10] RUP não é ágil: é iterativo e incremental, mas dirigido a planos (pesado). Definição: dirigido a casos de uso, centrado na arquitetura, iterativo e incremental. AUP/OpenUP são as variações ágeis.
- [24/10] Manifesto Ágil: "mais que", não "em vez de". Processos, documentação, contratos e planos têm valor.
- [24/10] Dirigido a planos quando: sistema crítico, regulação externa, especificação aprovada antes de codificar, equipe grande ou distribuída.

### XP e escalamento ágil

- [24/10] Test-first: teste que falha → código mínimo → refatorar. Refatorar = mudar a estrutura sem mudar o comportamento.
- [24/10] Propriedade coletiva (XP): qualquer desenvolvedor altera qualquer parte do código; não existe dono de módulo.
- [24/10] Ritmo sustentável (XP): evitar horas extras em excesso, pois reduzem a qualidade do código e a produtividade.
- [24/10] Histórias de usuário e cliente no local são práticas da XP (não exclusivas do Scrum).
- [24/10] Scaling up = ágil em sistema grande (várias equipes) · Scaling out = ágil espalhado por toda a organização.

### Scrum

- [22/10] Scrum Team: PO + SM + Developers, até 10 pessoas, sem sub-times. Developers são autogerenciáveis (Guia 2020).
- [22/10] Autogestão dos Developers = como fazer o trabalho (Sprint Backlog), não decisões de produto.
- [22/10] Só o Product Owner cancela a Sprint, e somente se a Sprint Goal ficar obsoleta.
- [22/10] Scrum Master: líder que serve; não distribui tarefas, não é gerente de projeto.
- [22/10] Timeboxes (Sprint de 1 mês): Planning 8h · Daily 15 min · Review 4h · Retro 3h.
- [22/10] Review = inspeciona o produto (com stakeholders) · Retro = inspeciona o processo (pessoas, interações, processos, ferramentas).
- [22/10] Artefatos e compromissos: Product Backlog → Product Goal · Sprint Backlog → Sprint Goal · Incremento → DoD. DoD não é artefato.
- [22/10] Refinamento do backlog não é evento.

### Kanban e Lean

### Requisitos e user stories

- [24/10] Requisito de usuário = alto nível, linguagem natural · requisito de sistema = detalhado, preciso, pode ser base do contrato.
- [24/10] RNF de produto = comportamento do software (disponibilidade, desempenho) · organizacional = norma interna (linguagem, processo) · externo = lei/regulação (LGPD). Teste: "quem exige isso?".
- [24/10] RNF deve ser mensurável e verificável; "fácil de usar" é só meta.

### Estimativa

---

## APF, SAFe e Testes

## Algoritmos, POO, SOLID e GoF

## Banco de Dados e SQL

## Arquitetura e System Design

## Linguagens e Frameworks

## Mobile e UI/UX

## DevOps e Nuvem

## Segurança

## IA

## Judiciário, LGPD e Governança

---

## Estratégia de prova

- [22/10] V/F com itens I, II, III: se a combinação que achei não existe nas alternativas, reavaliar os itens antes de escolher a mais próxima.
- [23/10] Questão que pede a "incorreta": julgar cada alternativa como V ou F; a resposta é a única F.
- [24/10] Item V/F que define uma prática pelo oposto do nome ("propriedade coletiva" = "um único dono") é falso. Um item não fica falso só porque a prática também existe em outro método.
