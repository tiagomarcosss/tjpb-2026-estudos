---
tipo: correcao
fonte: autoral
disciplina: ["Engenharia de Software e Ágil", "RLM", "Português"]
assunto: "User stories, INVEST, critérios de aceitação e BDD/Gherkin (+ revisão: Scrum, Kanban, modelo em V, negação da condicional, concordância) (15 questões)"
semana: 1
data: 2026-10-28
acertos: 13
total: 15
---

# Correção · Engenharia de Software · User stories, INVEST e BDD · 15 questões

**Data:** 28/10/2026 · **Semana 1** · **Placar: 13/15 (87%)** · 1 erro · 1 em branco

**Respostas lidas das anotações do PDF:** 1-C · 2-A · 3-D · 4-B · 5-A · 6-D · 7-B · 8-em branco · 9-D · 10-C · 11-A · 12-E · 13-B · 14-C · 15-D

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

> **Marcas no PDF:** a Q8 ficou só com um "?" e sem letra marcada (contada como em branco). Nas Q4 e Q5 há uma marquinha ao lado da alternativa escolhida, além do círculo; pelo seu método, isso é **acerto com dúvida**. Riscos de eliminação bem usados nas Q3, Q4, Q6, Q10, Q13 e Q15. Na Q9 você rastreou o código na margem (capacidade 10 → 2, H1 e H4), e na Q14 resolveu por Boole: (A' + B)' = A·B'.

| Questão | Assunto | Sua | Gabarito | Resultado |
|---|---|---|---|---|
| 1 | 3 Cs (Cartão, Conversa, Confirmação) | C | C | ✅ |
| 2 | INVEST · Independente | A | A | ✅ |
| 3 | INVEST · Negociável ("incorreta") | D | D | ✅ |
| 4 | Épico e fatiamento de histórias | B | B | ✅ (com dúvida) |
| 5 | Critério de aceitação × DoD | A | A | ✅ (com dúvida) |
| 6 | Gherkin · Dado / Quando / Então / E | D | D | ✅ |
| 7 | BDD × Gherkin × Cucumber | B | B | ✅ |
| 8 | TDD × ATDD × BDD (I, II, III) | — | E | ⬜ em branco |
| 9 | Leitura de código Python (Sprint) | D | D | ✅ |
| 10 | História bem escrita (formato + INVEST) | C | C | ✅ |
| 11 | Scrum · dono do Sprint Backlog (revisão) | A | A | ✅ |
| 12 | Kanban · lead × cycle time (revisão) | E | E | ✅ |
| 13 | Modelo em V (revisão) | B | B | ✅ |
| 14 | Negação da condicional (revisão RLM) | C | C | ✅ |
| 15 | Concordância: "em anexo", "é necessário" (revisão Português) | D | E | ❌ (repetido) |

**Placar separado (regra nova de 28/10):**
- **Assunto do dia (Q1–Q10): 9/10 (90%)**, com a Q8 em branco.
- **Revisão de pontos fracos (Q11–Q15): 4/5.** Este bloco ainda misturou a revisão; a partir de agora, bloco de assunto novo cobra só o assunto.

**Comparação:** é o seu **melhor placar até agora**. Eng. Software foi de 9/14 (64%, 24/10) para 8/15 (53%, 26/10) e agora 13/15 (87%). E três pontos fracos antigos caíram certos:

1. **Sprint Backlog dos Developers (Q11):** errou em 22/10 e 26/10; agora acertou.
2. **Lead × cycle time (Q12):** errou em 26/10; agora acertou com as datas marcadas.
3. **Modelo em V (Q13):** errou em 26/10; agora acertou eliminando três alternativas.

**O que ainda pesa:** concordância nominal, **3ª vez** (23/10, 28/10 de manhã e agora). Desta vez você eliminou certo "anexo", "é proibido a" e "meias", o que é progresso. Mas caiu em "em anexos" (a locução não varia) e descartou "é necessário paciência" (certa, porque não há artigo).

---

## Questão 1 · ✅ Acertou

A equipe de desenvolvimento do Tribunal de Justiça passou a registrar requisitos como histórias de usuário. Na capacitação, o analista apresentou os "3 Cs" propostos por Ron Jeffries.

Assinale a opção que descreve corretamente os três elementos.

(A) Cartão é a especificação completa e definitiva da funcionalidade; Conversa é a reunião em que o PO apresenta o cartão; Confirmação é a assinatura do PO no cartão.

(B) Cartão é o registro breve da necessidade; Conversa ocorre apenas na Sprint Planning; Confirmação é a aprovação formal da história na Sprint Review.

✅ **(C) Cartão é o registro breve que lembra a necessidade; Conversa é o diálogo em que os detalhes são esclarecidos entre equipe, PO e usuários; Confirmação são os critérios de aceitação que permitem verificar se a história foi atendida.** ← sua resposta

(D) Cartão é o documento de requisitos do sistema; Conversa é a negociação contratual com o fornecedor; Confirmação é o teste unitário escrito pelo desenvolvedor.

(E) Cartão é o item do Sprint Backlog; Conversa é a Daily Scrum; Confirmação é a Definição de Pronto (DoD) do time.

(A) e (D) transformam o cartão em especificação completa, o oposto da ideia. (B) limita a conversa a um evento. (E) troca a Confirmação pela DoD.

📌 **3 Cs:** Cartão = lembrete curto · Conversa = onde nasce o detalhe (contínua, não um evento) · Confirmação = critérios de aceitação.

---

## Questão 2 · ✅ Acertou

O Product Owner do sistema de custas judiciais organizou as histórias abaixo.

- H1: Como servidor da contadoria, quero cadastrar as tabelas de custas, para manter os valores atualizados.
- H2: Como advogado, quero simular o valor das custas, para saber quanto pagar antes do protocolo. Só pode ser desenvolvida depois de H1.
- H3: Como advogado, quero emitir a guia de pagamento, para quitar as custas. Só pode ser desenvolvida depois de H2.

O PO reclamou que não consegue reordenar essas histórias livremente no backlog.

Considerando o modelo INVEST, o critério mais diretamente comprometido é

✅ **(A) Independente.** ← sua resposta

(B) Negociável.

\(C) Valiosa.

(D) Estimável.

(E) Testável.

Você sublinhou as pistas certas ("depois de H1", "depois de H2"). Dependência em cadeia impede reordenar o backlog: é a falha do **I**. As histórias têm valor, são estimáveis e testáveis.

📌 **Independente = pode ser priorizada e entregue em qualquer ordem.** Pista na FGV: "só depois de", "depende de", "não consegue reordenar".

---

## Questão 3 · ✅ Acertou

Sobre o modelo INVEST para histórias de usuário, assinale a afirmativa **incorreta**.

(A) Uma história valiosa entrega um resultado perceptível para o usuário ou para o cliente.

(B) Uma história estimável tem informação suficiente para que o time avalie o seu tamanho.

\(C) Uma história pequena (*small*) cabe dentro de uma iteração.

✅ **(D) Uma história negociável, depois de escrita e aprovada pelo PO, torna-se um contrato fechado de escopo, cujos detalhes não devem mais ser rediscutidos pela equipe.** ← sua resposta

(E) Uma história testável permite definir critérios objetivos para verificar se foi atendida.

Você sublinhou "incorreta" e riscou as verdadeiras: a estratégia funcionou de novo. "Negociável" significa o contrário de "contrato fechado".

📌 **Negociável = os detalhes são combinados na conversa, não é contrato fechado.** Alternativa que define o critério pelo oposto do nome é falsa (mesma regra da "propriedade coletiva" de 24/10).

---

## Questão 4 · ✅ Acertou (com dúvida)

No backlog do novo sistema de gabinete consta a seguinte história:

"Como magistrado, quero um módulo completo de gestão do gabinete, com minutas, agenda de audiências, estatísticas de produtividade e assinatura em lote, para organizar o trabalho da unidade."

O time estimou que a entrega levaria cerca de quatro Sprints de duas semanas.

A conduta mais adequada é

(A) manter a história como está e aumentar a duração da Sprint para dois meses.

✅ **(B) tratá-la como épico e dividi-la em histórias menores, cada uma entregando valor ao usuário e cabendo em uma Sprint.** ← sua resposta

\(C) dividi-la por camadas técnicas (banco de dados, back-end e telas), uma camada por Sprint.

(D) reescrevê-la como requisito não funcional, por envolver vários módulos.

(E) rejeitá-la, pois histórias de usuário só servem para funcionalidades simples.

(A) viola o Scrum (Sprint de no máximo um mês). \(C) é o **fatiamento horizontal**: nenhuma camada sozinha entrega valor ao usuário. (D) e (E) não têm base.

📌 **Épico = história grande demais para uma Sprint → dividir em fatias verticais** (cada fatia atravessa banco, back-end e tela e entrega algo usável). Fatiar por camada técnica é errado.

---

## Questão 5 · ✅ Acertou (com dúvida)

Um time Scrum do Tribunal registrou as duas definições abaixo.

1. "Todo item entregue deve ter o código revisado por um par, testes unitários com cobertura mínima de 80% e implantação no ambiente de homologação."
2. "Para a história 'emitir certidão negativa', o sistema deve gerar o PDF com QR code de validação e recusar CPF inválido."

Assinale a opção que classifica corretamente as definições 1 e 2.

✅ **(A) 1 é a Definição de Pronto (DoD), que vale para todos os itens do Incremento; 2 são critérios de aceitação, específicos daquela história.** ← sua resposta

(B) 1 são critérios de aceitação; 2 é a Definição de Pronto (DoD).

\(C) Ambas são critérios de aceitação, pois as duas verificam a conclusão de itens.

(D) Ambas compõem a Definição de Pronto (DoD), pois as duas são condições de qualidade.

(E) 1 é a Definição de Pronto (DoD); 2 é a Definição de Preparado (DoR), pois descreve as condições para iniciar a história.

A pista estava no que você sublinhou: "**Todo** item" (vale para tudo = DoD) × "Para **a história** 'emitir certidão'" (vale para uma = critério). (E) erra porque a DoR trata de quando a história está pronta para **entrar** na Sprint, não do que ela deve fazer.

📌 **DoD = vale para todo item, qualidade interna (revisão, testes, deploy) · Critério de aceitação = vale para uma história, comportamento esperado pelo usuário.** Para estar pronta, a história precisa cumprir os dois.

---

## Questão 6 · ✅ Acertou

Observe o cenário abaixo, escrito em Gherkin, com as palavras-chave substituídas por números.

```gherkin
Cenário: Recurso protocolado fora do prazo
  [1] que o prazo recursal do processo terminou em 20/10
  [2] o advogado tentar protocolar o recurso em 22/10
  [3] o sistema deve exibir o alerta de intempestividade
  [4] registrar a tentativa no histórico do processo
```

As palavras-chave que substituem corretamente [1], [2], [3] e [4] são, respectivamente,

(A) Quando, Dado, Então, Mas.

(B) Dado, Então, Quando, E.

\(C) Então, Quando, Dado, E.

✅ **(D) Dado, Quando, Então, E.** ← sua resposta

(E) Dado, Quando, E, Então.

Você eliminou pelo primeiro item: "que o prazo terminou" só pode ser **Dado** (contexto). Isso derruba A e C. Depois, "tentar protocolar" é a ação (**Quando**), o que derruba B.

📌 **Gherkin: Dado = contexto anterior · Quando = ação ou evento · Então = resultado esperado · E/Mas = continuam o passo anterior.** Pista gramatical: "Dado **que**…", "Quando **o usuário** + verbo", "Então **o sistema deve**…".

---

## Questão 7 · ✅ Acertou

A equipe de qualidade do Tribunal pretende adotar BDD. Sobre BDD, Gherkin e Cucumber, assinale a afirmativa correta.

(A) Gherkin é uma metodologia ágil que substitui o TDD no ciclo de desenvolvimento.

✅ **(B) Cucumber é uma ferramenta que interpreta cenários escritos em Gherkin e os executa como testes automatizados, ligando cada passo a um trecho de código.** ← sua resposta

\(C) Só se pratica BDD com o uso do Cucumber, que é parte obrigatória da abordagem.

(D) Cenários em Gherkin só podem ser escritos em inglês, com as palavras Given, When e Then.

(E) No BDD, os cenários são escritos exclusivamente pelos desenvolvedores, em linguagem técnica, sem participação da área de negócio.

(A) Gherkin é linguagem, não metodologia. \(C) Cucumber é uma ferramenta entre várias (SpecFlow, Behave, Behat). (D) Gherkin aceita vários idiomas, inclusive o português (`# language: pt`). (E) BDD é colaborativo e usa linguagem de negócio.

📌 **BDD = prática · Gherkin = linguagem · Cucumber = ferramenta que executa o Gherkin.** Os passos do cenário viram código pelas *step definitions*.

---

## Questão 8 · ⬜ Em branco

Analise as afirmativas a seguir sobre abordagens de desenvolvimento guiadas por testes.

I\. No TDD, o desenvolvedor escreve um teste de unidade que falha antes de escrever o código de produção.

II\. No ATDD, os critérios de aceitação são definidos em colaboração entre negócio, desenvolvimento e teste antes da implementação, e passam a guiar o desenvolvimento.

III\. O BDD substitui o TDD; por isso, ao adotar BDD, a equipe deixa de escrever testes de unidade.

Está correto o que se afirma em

(A) I, apenas.

(B) II, apenas.

\(C) I e III, apenas.

(D) II e III, apenas.

✅ **(E) I e II, apenas.**

**Onde travou:** você marcou "?" e não escolheu. Provavelmente faltou segurança no item II (ATDD), que vimos só de passagem. Mas dava para resolver por eliminação, sem saber o II:

- **I é V**: é o ciclo do TDD que você já domina (vermelho → verde → refatorar, regra de 26/10).
- **III é F**: "substitui" e "deixa de escrever testes de unidade" são exageros; BDD e TDD se complementam.
- Com I = V e III = F, só sobram **(A)** e **(E)**. Entre as duas, o II descreve exatamente o que o nome ATDD diz (*Acceptance Test-Driven*: os testes de **aceitação** guiam o desenvolvimento). Logo, (E).

📌 **TDD = teste de unidade, pelo desenvolvedor · ATDD = critérios de aceitação definidos juntos (negócio + dev + teste) antes de codificar · BDD = comportamento em linguagem de negócio.** Os três se complementam; nenhum substitui o outro.

📌 **Nunca deixar em branco:** julgue os itens que você sabe e veja quantas alternativas sobram. Aqui, dois itens resolviam 80% da questão.

---

## Questão 9 · ✅ Acertou

Considere o código Python a seguir, usado para montar uma Sprint a partir do backlog.

```python
historias = [
    {"id": "H1", "pontos": 5,  "criterios": 3},
    {"id": "H2", "pontos": 13, "criterios": 2},
    {"id": "H3", "pontos": 3,  "criterios": 0},
    {"id": "H4", "pontos": 8,  "criterios": 1},
    {"id": "H5", "pontos": 2,  "criterios": 4},
]
capacidade = 15
sprint = []
for h in historias:
    if h["criterios"] == 0:
        continue
    if h["pontos"] > 8:
        print(f"{h['id']}: dividir")
        continue
    if capacidade - h["pontos"] >= 0:
        sprint.append(h["id"])
        capacidade -= h["pontos"]
print(sprint, capacidade)
```

A saída produzida é

(A)
```
H2: dividir
['H1', 'H4'] 2
```

(B)
```
['H1', 'H4', 'H5'] 0
```

\(C)
```
H2: dividir
['H1', 'H3', 'H5'] 5
```

✅ **(D)**
```
H2: dividir
['H1', 'H4', 'H5'] 0
```
← sua resposta

(E)
```
H2: dividir
H3: dividir
['H1', 'H4', 'H5'] 0
```

Rastreio: H1 entra (15 → 10) · H2 tem 13 > 8 → imprime "dividir" · H3 tem 0 critérios → `continue`, pulada em silêncio · H4 entra (10 → 2) · H5 entra (2 → 0, porque `>=` aceita o zero). Sua anotação na margem (10, 2, H1, H4) bate exatamente.

Pegadinhas: (A) quem lê `>=` como `>` perde a H5 · (B) esquece o `print` · \(C) ignora o `continue` da H3 · (E) acha que o `continue` também imprime.

📌 **Leitura de código: anotar a variável a cada volta do laço** (como você fez). `continue` pula o resto da volta sem imprimir nada; `>=` inclui o zero.

---

## Questão 10 · ✅ Acertou

Assinale a opção que apresenta a história de usuário mais bem escrita, considerando o formato "Como / quero / para" e o modelo INVEST.

(A) Como sistema, quero migrar o banco de dados para PostgreSQL.

(B) Como usuário, quero que o sistema seja rápido.

✅ **(C) Como servidor do cartório, quero consultar processos pelo número CNJ, para localizar os autos sem depender da secretaria.** ← sua resposta

(D) Como advogado, quero todo o módulo de peticionamento, intimações e pagamento de custas, para usar o PJe.

(E) Como desenvolvedor, quero criar a tabela TB_PROCESSO com índice na coluna NUM_CNJ.

(A) "sistema" não é usuário e não há benefício · (B) "rápido" não é testável · (D) é épico, não é pequena · (E) é tarefa técnica, sem valor para o usuário. Só a \(C) tem papel real, ação clara e benefício.

📌 **História boa = papel real + ação + benefício ("para…").** "Como sistema" ou "como desenvolvedor" + detalhe técnico = tarefa, não história.

---

## Questão 11 · ✅ Acertou (revisão: ponto fraco de 22 e 26/10)

No meio de uma Sprint do sistema de mandados, os Developers descobriram que uma das histórias só atenderá aos critérios de aceitação se for criada uma tarefa extra de ajuste no banco de dados. No mesmo dia, o Product Owner quis incluir uma história nova, não prevista na Sprint Planning. A Sprint Goal continua válida.

De acordo com o Guia do Scrum (2020), é correto afirmar que

✅ **(A) os Developers podem incluir a tarefa extra no Sprint Backlog, que pertence a eles; já a inclusão da nova história altera o escopo e deve ser negociada com o Product Owner, sem comprometer a Sprint Goal.** ← sua resposta

(B) somente o Scrum Master pode alterar o Sprint Backlog durante a Sprint.

\(C) o Product Owner pode alterar o Sprint Backlog diretamente, pois é o responsável por todos os backlogs do produto.

(D) nenhuma alteração no Sprint Backlog é permitida depois da Sprint Planning.

(E) os Developers devem cancelar a Sprint e fazer uma nova Sprint Planning.

Era exatamente o erro de 26/10 (achar que o PO altera o Sprint Backlog). Desta vez você não caiu na \(C). (E) erra duas vezes: quem cancela é só o PO, e só se a Sprint Goal ficar obsoleta.

📌 **Sprint Backlog é dos Developers:** eles ajustam o plano durante a Sprint. Mudança de escopo é negociada com o PO, sem mexer na Sprint Goal.

---

## Questão 12 · ✅ Acertou (revisão: ponto fraco de 26/10)

O quadro Kanban da equipe de sistemas registrou o seguinte para um pedido da Corregedoria:

- 01/10: pedido registrado na coluna "Backlog";
- 08/10: o time puxou o item para "Em desenvolvimento";
- 15/10: o item foi entregue em produção.

O lead time e o cycle time desse item foram, respectivamente,

(A) 7 dias e 14 dias.

(B) 14 dias e 14 dias.

\(C) 7 dias e 7 dias.

(D) 21 dias e 7 dias.

✅ **(E) 14 dias e 7 dias.** ← sua resposta

Lead = 01/10 → 15/10 = 14 dias (inclui a fila). Cycle = 08/10 → 15/10 = 7 dias. (A) inverte os dois, que foi o seu erro de 26/10.

📌 **Lead time = pedido → entrega (visão do cliente) · Cycle time = início do trabalho → entrega (visão do time). Lead ≥ cycle.**

---

## Questão 13 · ✅ Acertou (revisão: ponto fraco de 26/10)

Um projeto do Tribunal com requisitos estáveis segue o modelo em V. Os critérios de aceitação definidos com os usuários na fase de requisitos serão usados para validar o sistema ao final.

Assinale a opção que associa corretamente as fases de especificação aos níveis de teste nesse modelo.

(A) Requisitos do usuário ↔ teste unitário · requisitos do sistema ↔ teste de integração · código ↔ teste de aceitação.

✅ **(B) Requisitos do usuário ↔ teste de aceitação · requisitos do sistema e arquitetura ↔ teste de sistema · projeto dos módulos ↔ teste de integração · código ↔ teste unitário.** ← sua resposta

\(C) Requisitos do sistema ↔ teste de aceitação · requisitos do usuário ↔ teste de sistema · código ↔ teste de integração.

(D) Projeto dos módulos ↔ teste de sistema · arquitetura ↔ teste de integração · requisitos do usuário ↔ teste unitário.

(E) Todas as fases de especificação são validadas apenas pelo teste de regressão, executado ao final do projeto.

O V "espelha" cada fase do lado esquerdo no teste da mesma altura do lado direito: o topo (usuário) com o topo (aceitação), o fundo (código) com o fundo (unitário).

📌 **Modelo em V:** req. do usuário ↔ aceitação · req. do sistema/arquitetura ↔ sistema · projeto de módulos ↔ integração · código ↔ unitário.

---

## Questão 14 · ✅ Acertou (revisão: RLM de 21 e 27/10)

Considere a proposição:

"Se a história é testável, então ela possui critérios de aceitação."

A negação lógica dessa proposição é

(A) Se a história não é testável, então ela não possui critérios de aceitação.

(B) Se a história possui critérios de aceitação, então ela é testável.

✅ **(C) A história é testável e não possui critérios de aceitação.** ← sua resposta

(D) A história não é testável ou possui critérios de aceitação.

(E) A história não é testável e não possui critérios de aceitação.

Você resolveu pelo método de Boole: A → B = A' + B, então a negação é (A' + B)' = A · B'. (A) é a inversa, (B) é a recíproca e (D) é **equivalente** à original (não é a negação).

📌 **Negação de "se A, então B" = "A e não B".** Nunca outra condicional.

---

## Questão 15 · ❌ Errou (erro repetido: 23/10 e 28/10)

Assinale a frase que está de acordo com a norma-padrão quanto à concordância.

(A) Seguem anexo os critérios de aceitação da história.

(B) É proibido a alteração do Sprint Backlog pelo Product Owner.

\(C) As histórias foram entregues meias prontas na Sprint Review.

❌ (D) Seguem, em anexos, os cenários escritos em Gherkin. ← sua resposta

✅ **(E) É necessário paciência no refinamento do backlog.**

**Onde se confundiu:** você riscou certo o "anexo" (A), o "proibido" (B) e o "meias" \(C), que é um avanço. Sobraram (D) e (E). Provavelmente estranhou "necessário" (masculino) com "paciência" (feminino) e achou que "em anexos" estaria concordando com "cenários". Os dois raciocínios vão pelo ouvido, não pela regra:

- **"Em anexo" é locução e nunca varia.** Quem varia é só o adjetivo "anexo" sem preposição (seguem **anexos** os cenários).
- **"É necessário paciência" está certo porque não há artigo.** Sem artigo, a expressão fica no masculino singular. Com artigo, concorda: "É necessári**a a** paciência".

📌 **É necessário / é proibido / é bom + substantivo SEM artigo = invariável** (é necessário paciência) · **COM artigo = concorda** (é necessária a paciência). **"Em anexo" nunca vai para o plural.**

---

## Para o caderno de erros

| Assunto | Por que errei | Regra certa |
|---|---|---|
| TDD × ATDD × BDD (Q8, em branco) | Inseguro no ATDD; não usei a eliminação pelos itens que sabia | I (TDD) = V e III (BDD substitui TDD) = F já deixavam só A ou E. ATDD = critérios de aceitação definidos juntos antes de codificar |
| Concordância: "em anexo" e "é necessário" (Q15, 3ª vez) | Julguei pelo ouvido: "em anexos" parecia concordar e "necessário paciência" parecia errado | "Em anexo" nunca varia. Sem artigo, "é necessário/proibido + substantivo" fica invariável; com artigo, concorda |

---

## O que estudar agora

| Quando | O que fazer |
|---|---|
| Hoje · 22:40 (revisão) | Reler as regras 📌 da Q8 e da Q15. Escrever 3 frases com "em anexo / anexo / anexas" e 3 com "é necessário / é necessária a". Revisão espaçada: regras de 21/10 (7 dias) e de 27/10 (1 dia) |
| Qui 29/10 · almoço | RLM: 10 questões FGV de equivalências e negações (QConcursos/TEC), pelo método de Boole |
| Qui 29/10 · 19h–20h50 | Estimativa ágil: Planning Poker, story points e T-shirt (seção 5.3 do mapa) + bloco só desse assunto |
| Sex 30/10 · almoço | Português Módulo 0 A2 (verbo, advérbio, locuções adverbiais) |
| Sáb 31/10 | Revisão da semana (aqui entra o bloco misto, se você pedir) |
| Dom 01/11 · 13h | 1º simulado oficial (TJ-MS 2024 ou TJ-AP 2024), cronometrado e sem consulta. Meta: zero em branco |
