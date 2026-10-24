# Correção · Bloco 1 · SDLC e Scrum

**Data:** 22/10/2026 · **Placar: 3/5 (60%)**
**Respostas lidas das anotações do Okular:** 1-C · 2-B · 3-A · 4-D · 5-B

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

| Questão | Sua | Gabarito | Resultado |
|---|---|---|---|
| 1 | C | C | ✅ |
| 2 | B | D | ❌ |
| 3 | A | C | ❌ |
| 4 | D | D | ✅ |
| 5 | B | B | ✅ |

---

## Questão 1 · ✅ Acertou

Um tribunal contratou o desenvolvimento de um sistema de controle de custas processuais. Os requisitos foram definidos por resolução, são estáveis e não devem mudar durante o projeto. A equipe optou por um modelo em que cada fase só começa após a conclusão e aprovação da anterior.

Sobre o modelo adotado, é correto afirmar que

(A) permite entregar partes funcionais do sistema ao usuário a cada ciclo curto de desenvolvimento.

(B) tem como principal característica a análise de riscos ao início de cada volta do ciclo.

✅ **(C) é adequado ao cenário descrito, mas tem como desvantagem o feedback tardio do usuário sobre o produto.**

(D) é classificado como iterativo, pois cada fase refina o resultado da fase anterior.

(E) dispensa a documentação formal entre as fases, já que os requisitos são estáveis.

Você identificou o cascata ("cada fase só começa após a anterior") e eliminou as distratoras certas: (A) é incremental, (B) é espiral, (D) é iterativo e (E) está errada porque o cascata é fortemente documentado.

📌 **Cascata:** sequencial, adequado para requisitos estáveis, com feedback tardio e forte documentação entre as fases.

---

## Questão 2 · ❌ Errou

Durante uma Sprint, o Product Owner percebe que a Sprint Goal se tornou obsoleta em razão de uma mudança na legislação. O Scrum Master sugere aguardar o fim da Sprint, e os Developers propõem cancelá-la imediatamente.

De acordo com o Guia do Scrum, a Sprint

(A) pode ser cancelada apenas pelo Scrum Master, que é responsável pela aplicação do framework.

❌ **(B) pode ser cancelada por decisão consensual entre os Developers.** ← sua resposta

(C) não pode ser cancelada, devendo ser concluída e a mudança tratada na Retrospectiva.

✅ **(D) pode ser cancelada apenas pelo Product Owner, se a Sprint Goal se tornar obsoleta.**

(E) pode ser cancelada por qualquer membro do Scrum Team, desde que comunicado aos stakeholders.

**Onde você se confundiu:** como os Developers são autogerenciáveis, parece natural que eles decidam. Mas a autogestão vale para **como** fazer o trabalho (o Sprint Backlog), não para decisões sobre o produto. Cancelar a Sprint é uma decisão de valor e de produto, que é responsabilidade do PO. O enunciado colocou de propósito a proposta dos Developers como isca.

📌 **Só o Product Owner pode cancelar a Sprint**, e somente se a Sprint Goal se tornar obsoleta. O SM não cancela, os Developers não cancelam e não existe cancelamento "por consenso".

---

## Questão 3 · ❌ Errou

Considere as seguintes afirmativas sobre o Scrum:

I. A Sprint Review tem como objetivo inspecionar o resultado da Sprint e determinar adaptações futuras, com a participação dos stakeholders. → **Verdadeira**

II. A Sprint Retrospective tem como objetivo planejar formas de aumentar a qualidade e a efetividade, inspecionando pessoas, interações, processos e ferramentas. → **Verdadeira**

III. A Definition of Done é um dos três artefatos do Scrum, ao lado do Product Backlog e do Sprint Backlog. → **Falsa**

Está correto o que se afirma em

❌ **(A) I, apenas.** ← sua resposta

(B) II, apenas.

✅ **(C) I e II, apenas.**

(D) II e III, apenas.

(E) I, II e III.

**Onde você se confundiu:** pelas suas marcações, você avaliou I ✓, II ✗ e III ✓. Como "I e III" não existia entre as alternativas, ficou com (A). Foram dois erros:

- **II é verdadeira:** é praticamente a definição do Guia do Scrum para a Retrospectiva. Ela olha para o **processo** (pessoas, interações, processos, ferramentas).
- **III é falsa:** os três artefatos são **Product Backlog, Sprint Backlog e Incremento**. A DoD é o **compromisso** do Incremento, não um artefato.

**Dica de prova:** quando a sua combinação de V/F não aparece em nenhuma alternativa, é sinal de que você errou algum item. Volte e reavalie, em vez de escolher a mais próxima.

📌 **Artefatos:** Product Backlog → Product Goal · Sprint Backlog → Sprint Goal · Incremento → DoD. **Review = produto · Retro = processo.**

---

## Questão 4 · ✅ Acertou

Sabe-se que, em uma equipe Scrum, a Daily Scrum vem durando cerca de 40 minutos, conduzida pelo Scrum Master, que pergunta a cada Developer o que fez e distribui as tarefas do dia.

Considerando o Guia do Scrum, essa prática está

(A) correta, pois cabe ao Scrum Master distribuir as tarefas para garantir a Sprint Goal.

(B) incorreta apenas quanto à duração, já que o timebox da Daily é de 30 minutos.

(C) correta, desde que a duração não ultrapasse o timebox da Sprint Planning.

✅ **(D) incorreta, pois a Daily tem timebox de 15 minutos, é um evento dos Developers, e estes são autogerenciáveis.**

(E) incorreta, pois a Daily deve ser conduzida pelo Product Owner, responsável pelo Sprint Backlog.

Você acertou e evitou as duas pegadinhas: (B) erra o timebox ("apenas" e "30 minutos") e (E) atribui o Sprint Backlog ao PO, quando ele pertence aos Developers.

📌 **Daily:** 15 minutos, dos Developers e para os Developers. O SM não conduz nem distribui tarefas.

---

## Questão 5 · ✅ Acertou

Uma equipe desenvolve um portal de serviços. Na primeira entrega, disponibilizou o módulo de consulta processual já em produção. Na segunda, acrescentou o peticionamento eletrônico. Na terceira, incluiu a emissão de certidões. Em cada entrega, os módulos anteriores permaneceram inalterados.

O cenário descrito caracteriza, essencialmente, um desenvolvimento

(A) em cascata, pois as funcionalidades foram entregues em sequência.

✅ **(B) incremental, pois o sistema foi entregue em partes funcionais adicionadas a cada ciclo.**

(C) iterativo, pois o mesmo produto foi refinado a cada ciclo.

(D) em espiral, pois cada entrega foi precedida de análise de risco.

(E) em V, pois cada módulo foi verificado por um nível de teste correspondente.

Você acertou. A pista decisiva é "os módulos anteriores permaneceram inalterados": foram partes adicionadas, sem refinamento do que já existia.

**Atenção à sua anotação "protótipo":** prototipação é diferente de incremental. O protótipo é um modelo descartável ou evolutivo, usado para **validar requisitos**. Aqui, cada entrega já estava **em produção**.

📌 **Incremental = adiciona partes prontas · Iterativo = refina o mesmo produto · Prototipação = valida requisitos antes do produto final.**

---

## Para o caderno de erros

| Assunto | Por que errei | Regra certa |
|---|---|---|
| Cancelamento da Sprint | Achei que a autogestão dos Developers incluía cancelar | Só o PO cancela, se a Sprint Goal ficar obsoleta |
| Artefatos do Scrum | Coloquei a DoD como artefato | Artefatos: PB, SB e Incremento. DoD = compromisso do Incremento |
| Retrospectiva | Duvidei da definição correta | Retro inspeciona pessoas, interações, processos e ferramentas |
| Estratégia de V/F | Escolhi a alternativa "mais próxima" | Se a combinação não existe, reavalie os itens |

## O que estudar agora

- **Sex 23/10 · Bloco 1 (19h):** leia o **Guia do Scrum 2020** inteiro (13 páginas), com foco nas seções "Scrum Team" e "Artefatos".
- **Sex 23/10 · Bloco 2 (20h):** 10 questões FGV de Scrum no QConcursos/TEC, filtrando por papéis e eventos.
- **Revisão das 22:40:** crie 3 cards no Anki: "Quem cancela a Sprint?", "Quais são os 3 artefatos e seus compromissos?" e "Review × Retro".
- **Sáb 24/10:** Kanban + Lean, conforme a ordem da semana.
