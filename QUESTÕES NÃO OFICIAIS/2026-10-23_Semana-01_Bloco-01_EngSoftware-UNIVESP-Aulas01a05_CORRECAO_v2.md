# Correção · Simulado Semana 1 · Engenharia de Software (UNIVESP, Aulas 01 a 05)

**Versão 2** (questões completas, inclusive nos acertos) · **Data da correção:** 24/10/2026
**Placar: 9/14 (64%)** · 3 erros · 2 em branco
**Respostas lidas das marcações à mão no PDF:** 1-B · 2-D · 3-E · 4-C · 5-(branco) · 6-(branco) · 7-E · 8-A · 9-B · 10-C · 11-B · 12-C · 13-B · 14-E

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais. Base teórica: Sommerville, *Engenharia de Software* (material da UNIVESP).

| Questão | Assunto | Sua | Gabarito | Resultado |
|---|---|---|---|---|
| 1 | Atividades do processo | B | B | ✅ |
| 2 | Escolha do modelo | D | D | ✅ |
| 3 | Incremental (incorreta) | E | E | ✅ |
| 4 | Integração e configuração | C | C | ✅ |
| 5 | Fases do RUP | — | C | ⬜ em branco |
| 6 | Perspectivas do RUP | — | D | ⬜ em branco |
| 7 | Manifesto Ágil | E | E | ✅ |
| 8 | Ágil × dirigido a planos | A | A | ✅ |
| 9 | Ciclo test-first da XP | B | B | ✅ |
| 10 | Princípios e práticas da XP | C | B | ❌ |
| 11 | Scaling up × scaling out | B | D | ❌ |
| 12 | Requisito de usuário × de sistema | C | C | ✅ |
| 13 | Tipos de RNF | B | A | ❌ |
| 14 | RNF (incorreta) | E | E | ✅ |

**Por aula:** Aula 01 4/4 · Aula 02 (RUP) 0/2 em branco · Aula 03 2/2 · Aula 04 1/3 · Aula 05 2/3

---

## Aula 01 · Modelos de processo e atividades de software

## Questão 1 · ✅ Acertou

**Atividades fundamentais do processo de software**

Sabe-se que, independentemente do modelo de processo adotado, todo processo de software reúne um conjunto de atividades fundamentais.

Assinale a opção que apresenta corretamente essas atividades.

(A) Elicitação, prototipação, homologação e implantação.

✅ **(B) Especificação, projeto e implementação, validação e evolução.** ← sua resposta

(C) Concepção, elaboração, construção e transição.

(D) Planejamento, análise de riscos, engenharia e avaliação do cliente.

(E) Requisitos, arquitetura, codificação e manutenção corretiva.

Você riscou as distratoras certas: (C) são as fases do RUP, (D) são os quadrantes do espiral e (A)/(E) misturam termos soltos.

📌 **4 atividades fundamentais (Sommerville):** especificação · projeto e implementação · validação · evolução.

---

## Questão 2 · ✅ Acertou

**Escolha do modelo de processo**

A equipe de TI de um tribunal vai desenvolver um módulo de integração com o sistema de outro órgão público. Sabe-se que:

- os requisitos estão estáveis e bem compreendidos, pois seguem um protocolo já definido;
- o contrato exige que a documentação de cada fase seja formalmente aprovada antes do início da fase seguinte;
- parte da equipe trabalha em outra cidade.

Considerando esse cenário, o modelo de processo mais adequado é:

(A) o desenvolvimento incremental, com entregas parciais a cada iteração.

(B) a prototipação descartável, para validar os requisitos com os usuários.

(C) a Programação Extrema (XP), com cliente no local.

✅ **(D) o modelo em cascata.** ← sua resposta

(E) a integração e configuração de componentes reusáveis.

Pelas suas marcações, a leitura foi a certa: você grifou "estáveis", "compreendidos" e "formalmente aprovada antes do início" e riscou a prototipação (B) e o "cliente no local" da XP (C). O incremental (A) não se justifica com requisitos estáveis e aprovação formal por fase. A integração e configuração (E) não combina com um protocolo novo entre órgãos.

📌 **Cascata:** requisitos estáveis + aprovação formal por fase + equipe distribuída/contrato rígido.

---

## Questão 3 · ✅ Acertou

**Desenvolvimento incremental**

Com relação ao desenvolvimento incremental, assinale a afirmativa **incorreta**.

(A) Reduz o custo de acomodar mudanças nos requisitos, pois menos análise e documentação precisam ser refeitas.

(B) Facilita a obtenção de feedback do cliente sobre o que já foi desenvolvido.

(C) Permite entregar e implantar software útil mais cedo, mesmo sem toda a funcionalidade prevista.

(D) Tende a degradar a estrutura do sistema à medida que novos incrementos são adicionados, caso não haja tempo e recursos para refatoração.

✅ **(E) Torna o processo mais visível para os gerentes, pois cada versão gera documentação completa, o que o torna preferível para sistemas grandes, de vida longa e com equipes distribuídas.** ← sua resposta

Ótimo hábito: você escreveu "NÃO É" ao lado de "incorreta" e circulou "sistemas grandes". (A), (B) e (C) são as vantagens do livro, e (D) é um problema real. A (E) inverte o livro: no incremental o processo é **pouco visível**, porque não compensa documentar cada versão, e ele é **menos indicado** para sistemas grandes, de vida longa e com várias equipes.

📌 **Problemas do incremental:** processo pouco visível e estrutura que se degrada sem refatoração.

---

## Questão 4 · ✅ Acertou

**Integração e configuração (reuso)**

Um tribunal decidiu adotar um sistema de gestão de documentos já existente no mercado, configurável, em vez de desenvolver uma solução do zero.

Sobre a abordagem de integração e configuração, analise as afirmativas a seguir.

I. Os requisitos podem precisar ser ajustados ao que os componentes disponíveis oferecem. → **V**

II. A abordagem tende a reduzir custos e riscos, além de acelerar a entrega do software. → **V**

III. A organização mantém controle total sobre a evolução dos componentes reutilizados, já que é ela quem os configura. → **F**

Está correto o que se afirma em:

(A) I, apenas.

(B) II, apenas.

✅ **(C) I e II, apenas.** ← sua resposta

(D) II e III, apenas.

(E) I, II e III.

Você grifou "controle total" e "evolução dos componentes", e é exatamente aí que o item III erra. Quem controla a evolução é o **fornecedor**, não a organização que reusa.

📌 **Reuso:** menos custo e risco, entrega rápida · mas há concessão nos requisitos e **perda de controle sobre a evolução**.

---

## Aula 02 · Processo Unificado (RUP)

## Questão 5 · ⬜ Em branco ("não vi esse assunto")

**Fases do RUP**

Ao final de determinada fase de um projeto conduzido pelo Processo Unificado (RUP), a equipe havia produzido:

- um modelo de requisitos com a maior parte dos casos de uso especificados;
- a descrição da arquitetura do sistema;
- um plano de desenvolvimento para o restante do projeto, com os principais riscos tratados.

A fase concluída foi a de:

(A) Concepção.

(B) Construção.

✅ **(C) Elaboração.**

(D) Transição.

(E) Validação.

**Como resolver:** a palavra-chave é **arquitetura**. Cada fase do RUP tem um produto típico:

| Fase | Pergunta que responde | Produto típico |
|---|---|---|
| Concepção | Vale a pena fazer? | Caso de negócio, atores e escopo |
| **Elaboração** | Como vamos fazer? | **Maior parte dos casos de uso, arquitetura, plano de desenvolvimento, riscos principais tratados** |
| Construção | Fazer | Software funcionando e documentação |
| Transição | Entregar | Sistema implantado no ambiente do usuário |

"Validação" (E) não é fase do RUP; está lá só como distratora.

📌 **Elaboração = arquitetura + maioria dos casos de uso + plano do projeto.** Concepção = caso de negócio.

---

## Questão 6 · ⬜ Em branco

**Perspectivas do RUP**

O RUP costuma ser descrito a partir de três perspectivas: dinâmica, estática e prática.

Assinale a afirmativa correta.

(A) A perspectiva estática mostra as fases do modelo ao longo do tempo.

(B) A perspectiva dinâmica mostra as atividades (workflows) realizadas, sem relação com o tempo.

(C) Fases e workflows estão rigidamente associados: o workflow de requisitos ocorre somente na Concepção e o de implementação somente na Construção.

✅ **(D) A perspectiva prática descreve boas práticas, como desenvolver iterativamente, gerenciar requisitos e usar arquiteturas baseadas em componentes.**

(E) O RUP é sequencial: cada fase é executada uma única vez, sem iterações internas.

**A pegadinha:** (A) e (B) trocam as definições. A perspectiva **dinâmica mostra o tempo (as fases)** e a **estática mostra as atividades (os workflows)**. (C) e (E) estão erradas porque, no RUP, todos os workflows podem ocorrer em todas as fases, e cada fase tem iterações.

📌 **RUP · 3 perspectivas:** dinâmica = fases no tempo · estática = workflows (atividades) · prática = boas práticas. Fases e workflows **não** são rigidamente ligados.

📌 **6 boas práticas do RUP:** desenvolver iterativamente · gerenciar requisitos · usar arquitetura baseada em componentes · modelar visualmente (UML) · verificar a qualidade · controlar mudanças.

---

## Aula 03 · Métodos ágeis × dirigido a planos

## Questão 7 · ✅ Acertou

**Manifesto Ágil**

Considere verdadeira a afirmação de que uma equipe de desenvolvimento segue os valores do Manifesto Ágil.

Com base nisso, é correto concluir que a equipe:

(A) não produz documentação, pois o software em funcionamento substitui a documentação abrangente.

(B) não utiliza ferramentas de apoio ao processo, pois indivíduos e interações as substituem.

(C) dispensa contratos formais com o cliente, pois a colaboração substitui a negociação.

(D) não realiza planejamento, pois prioriza responder a mudanças.

✅ **(E) reconhece valor em processos, documentação, contratos e planos, mas valoriza mais indivíduos e interações, software em funcionamento, colaboração com o cliente e resposta a mudanças.** ← sua resposta

Você riscou as quatro alternativas que trocam "valoriza mais" por "elimina" ou "substitui", a pegadinha clássica da FGV.

📌 **Manifesto Ágil:** "mais que", não "em vez de". Os itens da direita **têm valor**.

---

## Questão 8 · ✅ Acertou

**Ágil × dirigido a planos**

Uma gerente de TI precisa decidir entre uma abordagem ágil e uma abordagem dirigida a planos para diferentes projetos.

Assinale a situação em que a abordagem **dirigida a planos** é a mais indicada.

✅ **(A) Sistema crítico de segurança, sujeito a regulação externa que exige documentação detalhada e aprovação prévia da especificação, desenvolvido por uma equipe grande e distribuída.** ← sua resposta

(B) Sistema interno pequeno, com equipe de cinco pessoas no mesmo local e cliente disponível diariamente.

(C) Projeto com requisitos que mudam com frequência e necessidade de entregar valor rapidamente.

(D) Produto novo em fase de teste de hipóteses, validado por meio de protótipos com usuários.

(E) Equipe experiente que prefere comunicação informal e conhecimento compartilhado entre os membros.

Você grifou "dirigida a planos" e acertou. As demais alternativas descrevem cenários ágeis: equipe pequena no mesmo local (B), requisitos instáveis (C), protótipos (D) e comunicação informal (E).

📌 **Dirigido a planos quando:** sistema crítico · regulação externa · especificação antes de codificar · equipe grande ou distribuída · vida longa.

---

## Aula 04 · Programação Extrema (XP) e escalamento

## Questão 9 · ✅ Acertou ("achei boa, só difícil")

**Práticas da XP**

Em um projeto que adota a Programação Extrema (XP), a dupla de programadores segue este ciclo ao implementar cada funcionalidade:

1. escreve um teste automatizado, que inicialmente falha;
2. escreve o código mínimo para o teste passar;
3. melhora a estrutura interna do código, sem alterar seu comportamento.

As práticas da XP descritas nesse ciclo são:

(A) programação em pares e propriedade coletiva.

✅ **(B) desenvolvimento test-first (teste primeiro) e refatoração.** ← sua resposta

(C) integração contínua e pequenos releases.

(D) design simples e ritmo sustentável.

(E) planejamento incremental e cliente no local.

Os passos 1 e 2 são o test-first. O passo 3, "melhora a estrutura sem alterar o comportamento", é a definição de refatoração. A dupla citada no enunciado é só contexto e não faz de (A) a resposta, porque o ciclo descrito não fala de propriedade do código.

📌 **TDD/test-first:** vermelho → verde → refatorar. **Refatorar = mudar a estrutura sem mudar o comportamento.**

---

## Questão 10 · ❌ Errou

**XP: princípios e práticas**

Sobre a Programação Extrema (XP), analise as afirmativas a seguir.

I. Os requisitos são expressos como histórias de usuário, e um representante do cliente participa da equipe para priorizá-las e esclarecê-las. → **Verdadeira**

II. A propriedade coletiva determina que cada módulo tenha um único desenvolvedor responsável por alterá-lo. → **Falsa**

III. O ritmo sustentável recomenda evitar grandes quantidades de horas extras, pois elas reduzem a qualidade do código e a produtividade. → **Verdadeira**

IV. Na integração contínua, o código é integrado ao sistema assim que a tarefa é concluída, e todos os testes devem passar após a integração. → **Verdadeira**

Está correto o que se afirma em:

(A) I e II, apenas.

✅ **(B) I, III e IV, apenas.**

❌ **(C) II e IV, apenas.** ← sua resposta

(D) III e IV, apenas.

(E) I, II, III e IV.

**Onde você se confundiu (pelas suas anotações):**

- **Item I: você escreveu "SCRUM" e riscou.** Histórias de usuário e cliente no local são práticas **da XP**; no livro, estão na lista de práticas da XP. O Scrum também usa histórias, mas isso não torna o item falso. Um item não fica errado só porque a prática também aparece em outro método.
- **Item II: você aceitou como verdadeiro.** O item diz o oposto da prática. Na **propriedade coletiva**, os pares trabalham em todas as áreas do sistema e **qualquer um pode alterar qualquer parte**, sem "ilhas de conhecimento". "Um único dono por módulo" é a negação disso.
- **Item III: você riscou perto de "pois elas reduzem".** A justificativa está certa. É exatamente o argumento do livro: hora extra reduz a qualidade do código e a produtividade no médio prazo.

**Dica de prova:** a palavra "coletiva" já desmente "único desenvolvedor". Quando o nome da prática contradiz a definição dada, desconfie.

📌 **XP · propriedade coletiva:** qualquer desenvolvedor pode alterar qualquer parte do código; não há dono de módulo.
📌 **XP · ritmo sustentável:** evitar horas extras em excesso, porque reduzem qualidade e produtividade.
📌 **XP · histórias de usuário e cliente no local** são práticas da XP (não exclusivas do Scrum).

---

## Questão 11 · ❌ Errou

**Escalamento de métodos ágeis**

A Secretaria de TI de um tribunal tomou duas decisões:

(1) usar métodos ágeis no desenvolvimento de um sistema de grande porte, que exige várias equipes trabalhando em paralelo;

(2) introduzir métodos ágeis em todas as diretorias de TI da organização, e não apenas em um projeto-piloto.

As decisões (1) e (2) correspondem, respectivamente, a:

(A) scaling out e scaling up.

❌ **(B) scaling up nos dois casos.** ← sua resposta

(C) scaling out nos dois casos.

✅ **(D) scaling up e scaling out.**

(E) desenvolvimento dirigido a planos e integração e configuração.

**Onde você se confundiu:** você grifou corretamente "sistema de grande porte" e "projeto-piloto", ou seja, percebeu que são situações diferentes. Mesmo assim, tratou as duas como "aumentar". A distinção do Sommerville é:

| Termo | Escala de quê | Exemplo |
|---|---|---|
| **Scaling up** ("para cima") | do **sistema** | Sistema grande, que uma equipe pequena não dá conta → várias equipes |
| **Scaling out** ("para fora") | da **organização** | Levar o ágil de um piloto para a empresa inteira |

**Macete:** em *up*, o projeto cresce **para cima** (fica maior); em *out*, o ágil se espalha **para fora** (para outras áreas).

📌 **Scaling up = ágil em sistema grande (várias equipes) · Scaling out = ágil em toda a organização.**

---

## Aula 05 · Tipos de requisitos

## Questão 12 · ✅ Acertou

**Requisitos de usuário × de sistema**

Considere as duas declarações a seguir, extraídas da documentação de um sistema judicial.

I. "O sistema deve gerar um relatório mensal dos processos distribuídos por vara."

II. "No último dia útil de cada mês, o sistema deve gerar um relatório em PDF com número do processo, classe, vara e data de distribuição, ordenado por vara e acessível somente a usuários com perfil Gestor."

Assinale a afirmativa correta.

(A) I é requisito de sistema e II é requisito de usuário, pois II se destina aos gestores.

(B) I e II são requisitos não funcionais, pois tratam de relatórios.

✅ **(C) I é requisito de usuário e II é requisito de sistema; II detalha o que o sistema deve fazer e pode servir de base para o contrato de desenvolvimento.** ← sua resposta

(D) I é requisito funcional e II é não funcional, pois II menciona perfil de acesso.

(E) I e II são requisitos de domínio, pois tratam de processos judiciais.

Você riscou as distratoras que trocam o critério da questão: (B) e (D) olham para funcional × não funcional e (E) para domínio. O critério aqui é o **nível de detalhe**. A (A) inverte os dois requisitos.

📌 **Requisito de usuário** = linguagem natural, alto nível, para o cliente · **requisito de sistema** = detalhado, preciso, pode ser base do contrato.

---

## Questão 13 · ❌ Errou

**Funcionais × não funcionais**

Considere os seguintes requisitos de um sistema de um tribunal:

1. O sistema deve permitir ao magistrado assinar digitalmente seus despachos.
2. O sistema deve estar disponível em 99,5% do horário de expediente.
3. O sistema deve ser desenvolvido em Java, conforme o padrão adotado pela Secretaria de TI.
4. O sistema deve tratar os dados pessoais das partes conforme a LGPD.

A classificação correta, na ordem apresentada, é:

✅ **(A) funcional; não funcional de produto; não funcional organizacional; não funcional externo.**

❌ **(B) funcional; não funcional organizacional; não funcional de produto; não funcional externo.** ← sua resposta

(C) funcional; não funcional de produto; não funcional externo; não funcional organizacional.

(D) não funcional de produto; funcional; não funcional organizacional; não funcional externo.

(E) funcional; funcional; não funcional organizacional; não funcional de produto.

**Onde você se confundiu:** a primeira camada você acertou (escreveu F, NF, NF ao lado). O erro foi no subtipo do RNF: você inverteu **produto** e **organizacional** nos itens 2 e 3.

| Subtipo de RNF | Origem | Exemplos | Na questão |
|---|---|---|---|
| **De produto** | Comportamento do próprio software | Desempenho, disponibilidade, confiabilidade, usabilidade, segurança | **2 · 99,5% de disponibilidade** |
| **Organizacional** | Políticas e padrões da organização (cliente ou desenvolvedora) | Linguagem/padrão obrigatório, processo, ambiente operacional | **3 · Java por padrão da Secretaria** |
| **Externo** | Fora do sistema e da organização | Leis (LGPD), regulação, ética, interoperabilidade | **4 · LGPD** |

**Pergunta-teste:** "quem exige isso?" Se é o **usuário**, sobre como o software se comporta, o RNF é de produto. Se é a **própria organização**, por norma interna, é organizacional. Se é uma **lei ou um terceiro**, é externo.

📌 **RNF: produto = como o software se comporta (disponibilidade, desempenho) · organizacional = norma interna (linguagem, processo) · externo = lei/regulação (LGPD).**

---

## Questão 14 · ✅ Acertou

**Requisitos não funcionais**

Sobre requisitos não funcionais, assinale a afirmativa **incorreta**.

(A) Podem afetar a arquitetura do sistema como um todo, e não apenas componentes isolados.

(B) Um único requisito não funcional, como um de segurança, pode gerar vários requisitos funcionais, como autenticação e controle de acesso.

(C) Deixar de atender um requisito não funcional pode tornar o sistema inteiro inutilizável.

(D) Sempre que possível, devem ser escritos de forma quantitativa e verificável, como "tempo de resposta inferior a 2 segundos em 95% das requisições".

✅ **(E) Por serem genéricos, não precisam ser verificáveis; metas como "o sistema deve ser fácil de usar" bastam como especificação final.** ← sua resposta

A estratégia funcionou: você marcou ✓ em (A), (B) e (C) e circulou a única falsa. A (D) é a regra do livro, e a (E) a contradiz. Um RNF precisa ser **mensurável e verificável**; "fácil de usar" é só uma **meta** e tem de virar algo testável.

📌 **RNF verificável:** transformar metas vagas em medidas ("usuário treinado comete no máximo 2 erros/hora").

---

## Para o caderno de erros

| Assunto | Por que errei | Regra certa |
|---|---|---|
| Fases do RUP | Não tinha estudado | Elaboração = arquitetura + maioria dos casos de uso + plano |
| Perspectivas do RUP | Não tinha estudado | Dinâmica = fases/tempo · estática = workflows · prática = boas práticas |
| XP · propriedade coletiva | Aceitei "um dono por módulo" | Qualquer um altera qualquer parte; "coletiva" já desmente "único" |
| XP · histórias de usuário | Descartei por achar que era "do Scrum" | Histórias + cliente no local são práticas da XP |
| Scaling up × out | Tratei as duas decisões como "up" | Up = sistema grande · Out = organização inteira |
| RNF produto × organizacional | Inverti os subtipos | Disponibilidade = produto · linguagem por norma interna = organizacional · LGPD = externo |

## Comparação com o bloco anterior (22/10 · SDLC e Scrum, 3/5)

- **Modelos de processo:** você acertou de novo (cascata, incremental e o "incorreta" sobre incremental). Assunto consolidado.
- **"Assinale a incorreta":** você acertou as duas (Q3 e Q14), usando V/F ao lado das alternativas. Na prova DATAPREV (23/10), esse foi um erro recorrente, então o hábito novo está funcionando.
- **V/F com itens:** você acertou a Q4 e errou a Q10. O erro da Q10 foi de conteúdo (XP), não de estratégia.

## O que estudar agora

- **Sáb 24/10 (hoje):** antes de Kanban e Lean, 30 min de **RUP** (Sommerville, cap. 2, seção "O Rational Unified Process"): fases × produtos e as 3 perspectivas. Depois, 5 questões FGV de RUP no QConcursos/TEC.
- **Revisão das 22:40:** criar 4 cards no Anki: "Produto da fase de Elaboração", "RUP: dinâmica × estática × prática", "Scaling up × scaling out", "RNF de produto × organizacional × externo (exemplos)".
- **Dom 25/10 · simulado TRT-16:** nas questões V/F, aplicar o teste "o nome da prática contradiz a definição?".
- **Ter 27/10 (RF × RNF × regras de negócio):** focar nos subtipos de RNF; nas questões "classifique o requisito", perguntar sempre "quem exige isso?".
- **Revisão espaçada:** XP (propriedade coletiva, ritmo sustentável) e scaling devem voltar nos blocos de 25/10, 31/10 e 23/11.
