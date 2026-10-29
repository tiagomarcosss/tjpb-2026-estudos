---
tipo: bloco
fonte: autoral
status: corrigido
disciplina: ["Engenharia de Software e Ágil", "RLM", "Português"]
assunto: "User stories, INVEST, critérios de aceitação e BDD/Gherkin (+ revisão: Scrum, Kanban, modelo em V, negação da condicional, concordância)"
semana: 1
data: 2026-10-28
---

# Bloco · Engenharia de Software · User stories, INVEST e BDD (15 questões)

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

## Questão 1

A equipe de desenvolvimento do Tribunal de Justiça passou a registrar requisitos como histórias de usuário. Na capacitação, o analista apresentou os "3 Cs" propostos por Ron Jeffries.

Assinale a opção que descreve corretamente os três elementos.

(A) Cartão é a especificação completa e definitiva da funcionalidade; Conversa é a reunião em que o PO apresenta o cartão; Confirmação é a assinatura do PO no cartão.

(B) Cartão é o registro breve da necessidade; Conversa ocorre apenas na Sprint Planning; Confirmação é a aprovação formal da história na Sprint Review.

\(C) Cartão é o registro breve que lembra a necessidade; Conversa é o diálogo em que os detalhes são esclarecidos entre equipe, PO e usuários; Confirmação são os critérios de aceitação que permitem verificar se a história foi atendida.

(D) Cartão é o documento de requisitos do sistema; Conversa é a negociação contratual com o fornecedor; Confirmação é o teste unitário escrito pelo desenvolvedor.

(E) Cartão é o item do Sprint Backlog; Conversa é a Daily Scrum; Confirmação é a Definição de Pronto (DoD) do time.

---

## Questão 2

O Product Owner do sistema de custas judiciais organizou as histórias abaixo.

- H1: Como servidor da contadoria, quero cadastrar as tabelas de custas, para manter os valores atualizados.
- H2: Como advogado, quero simular o valor das custas, para saber quanto pagar antes do protocolo. Só pode ser desenvolvida depois de H1.
- H3: Como advogado, quero emitir a guia de pagamento, para quitar as custas. Só pode ser desenvolvida depois de H2.

O PO reclamou que não consegue reordenar essas histórias livremente no backlog.

Considerando o modelo INVEST, o critério mais diretamente comprometido é

(A) Independente.

(B) Negociável.

\(C) Valiosa.

(D) Estimável.

(E) Testável.

---

## Questão 3

Sobre o modelo INVEST para histórias de usuário, assinale a afirmativa **incorreta**.

(A) Uma história valiosa entrega um resultado perceptível para o usuário ou para o cliente.

(B) Uma história estimável tem informação suficiente para que o time avalie o seu tamanho.

\(C) Uma história pequena (*small*) cabe dentro de uma iteração.

(D) Uma história negociável, depois de escrita e aprovada pelo PO, torna-se um contrato fechado de escopo, cujos detalhes não devem mais ser rediscutidos pela equipe.

(E) Uma história testável permite definir critérios objetivos para verificar se foi atendida.

---

## Questão 4

No backlog do novo sistema de gabinete consta a seguinte história:

"Como magistrado, quero um módulo completo de gestão do gabinete, com minutas, agenda de audiências, estatísticas de produtividade e assinatura em lote, para organizar o trabalho da unidade."

O time estimou que a entrega levaria cerca de quatro Sprints de duas semanas.

A conduta mais adequada é

(A) manter a história como está e aumentar a duração da Sprint para dois meses.

(B) tratá-la como épico e dividi-la em histórias menores, cada uma entregando valor ao usuário e cabendo em uma Sprint.

\(C) dividi-la por camadas técnicas (banco de dados, back-end e telas), uma camada por Sprint.

(D) reescrevê-la como requisito não funcional, por envolver vários módulos.

(E) rejeitá-la, pois histórias de usuário só servem para funcionalidades simples.

---

## Questão 5

Um time Scrum do Tribunal registrou as duas definições abaixo.

1. "Todo item entregue deve ter o código revisado por um par, testes unitários com cobertura mínima de 80% e implantação no ambiente de homologação."
2. "Para a história 'emitir certidão negativa', o sistema deve gerar o PDF com QR code de validação e recusar CPF inválido."

Assinale a opção que classifica corretamente as definições 1 e 2.

(A) 1 é a Definição de Pronto (DoD), que vale para todos os itens do Incremento; 2 são critérios de aceitação, específicos daquela história.

(B) 1 são critérios de aceitação; 2 é a Definição de Pronto (DoD).

\(C) Ambas são critérios de aceitação, pois as duas verificam a conclusão de itens.

(D) Ambas compõem a Definição de Pronto (DoD), pois as duas são condições de qualidade.

(E) 1 é a Definição de Pronto (DoD); 2 é a Definição de Preparado (DoR), pois descreve as condições para iniciar a história.

---

## Questão 6

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

(D) Dado, Quando, Então, E.

(E) Dado, Quando, E, Então.

---

## Questão 7

A equipe de qualidade do Tribunal pretende adotar BDD. Sobre BDD, Gherkin e Cucumber, assinale a afirmativa correta.

(A) Gherkin é uma metodologia ágil que substitui o TDD no ciclo de desenvolvimento.

(B) Cucumber é uma ferramenta que interpreta cenários escritos em Gherkin e os executa como testes automatizados, ligando cada passo a um trecho de código.

\(C) Só se pratica BDD com o uso do Cucumber, que é parte obrigatória da abordagem.

(D) Cenários em Gherkin só podem ser escritos em inglês, com as palavras Given, When e Then.

(E) No BDD, os cenários são escritos exclusivamente pelos desenvolvedores, em linguagem técnica, sem participação da área de negócio.

---

## Questão 8

Analise as afirmativas a seguir sobre abordagens de desenvolvimento guiadas por testes.

I\. No TDD, o desenvolvedor escreve um teste de unidade que falha antes de escrever o código de produção.

II\. No ATDD, os critérios de aceitação são definidos em colaboração entre negócio, desenvolvimento e teste antes da implementação, e passam a guiar o desenvolvimento.

III\. O BDD substitui o TDD; por isso, ao adotar BDD, a equipe deixa de escrever testes de unidade.

Está correto o que se afirma em

(A) I, apenas.

(B) II, apenas.

\(C) I e III, apenas.

(D) II e III, apenas.

(E) I e II, apenas.

---

## Questão 9

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

(D)
```
H2: dividir
['H1', 'H4', 'H5'] 0
```

(E)
```
H2: dividir
H3: dividir
['H1', 'H4', 'H5'] 0
```

---

## Questão 10

Assinale a opção que apresenta a história de usuário mais bem escrita, considerando o formato "Como / quero / para" e o modelo INVEST.

(A) Como sistema, quero migrar o banco de dados para PostgreSQL.

(B) Como usuário, quero que o sistema seja rápido.

\(C) Como servidor do cartório, quero consultar processos pelo número CNJ, para localizar os autos sem depender da secretaria.

(D) Como advogado, quero todo o módulo de peticionamento, intimações e pagamento de custas, para usar o PJe.

(E) Como desenvolvedor, quero criar a tabela TB_PROCESSO com índice na coluna NUM_CNJ.

---

## Questão 11

No meio de uma Sprint do sistema de mandados, os Developers descobriram que uma das histórias só atenderá aos critérios de aceitação se for criada uma tarefa extra de ajuste no banco de dados. No mesmo dia, o Product Owner quis incluir uma história nova, não prevista na Sprint Planning. A Sprint Goal continua válida.

De acordo com o Guia do Scrum (2020), é correto afirmar que

(A) os Developers podem incluir a tarefa extra no Sprint Backlog, que pertence a eles; já a inclusão da nova história altera o escopo e deve ser negociada com o Product Owner, sem comprometer a Sprint Goal.

(B) somente o Scrum Master pode alterar o Sprint Backlog durante a Sprint.

\(C) o Product Owner pode alterar o Sprint Backlog diretamente, pois é o responsável por todos os backlogs do produto.

(D) nenhuma alteração no Sprint Backlog é permitida depois da Sprint Planning.

(E) os Developers devem cancelar a Sprint e fazer uma nova Sprint Planning.

---

## Questão 12

O quadro Kanban da equipe de sistemas registrou o seguinte para um pedido da Corregedoria:

- 01/10: pedido registrado na coluna "Backlog";
- 08/10: o time puxou o item para "Em desenvolvimento";
- 15/10: o item foi entregue em produção.

O lead time e o cycle time desse item foram, respectivamente,

(A) 7 dias e 14 dias.

(B) 14 dias e 14 dias.

\(C) 7 dias e 7 dias.

(D) 21 dias e 7 dias.

(E) 14 dias e 7 dias.

---

## Questão 13

Um projeto do Tribunal com requisitos estáveis segue o modelo em V. Os critérios de aceitação definidos com os usuários na fase de requisitos serão usados para validar o sistema ao final.

Assinale a opção que associa corretamente as fases de especificação aos níveis de teste nesse modelo.

(A) Requisitos do usuário ↔ teste unitário · requisitos do sistema ↔ teste de integração · código ↔ teste de aceitação.

(B) Requisitos do usuário ↔ teste de aceitação · requisitos do sistema e arquitetura ↔ teste de sistema · projeto dos módulos ↔ teste de integração · código ↔ teste unitário.

\(C) Requisitos do sistema ↔ teste de aceitação · requisitos do usuário ↔ teste de sistema · código ↔ teste de integração.

(D) Projeto dos módulos ↔ teste de sistema · arquitetura ↔ teste de integração · requisitos do usuário ↔ teste unitário.

(E) Todas as fases de especificação são validadas apenas pelo teste de regressão, executado ao final do projeto.

---

## Questão 14

Considere a proposição:

"Se a história é testável, então ela possui critérios de aceitação."

A negação lógica dessa proposição é

(A) Se a história não é testável, então ela não possui critérios de aceitação.

(B) Se a história possui critérios de aceitação, então ela é testável.

\(C) A história é testável e não possui critérios de aceitação.

(D) A história não é testável ou possui critérios de aceitação.

(E) A história não é testável e não possui critérios de aceitação.

---

## Questão 15

Assinale a frase que está de acordo com a norma-padrão quanto à concordância.

(A) Seguem anexo os critérios de aceitação da história.

(B) É proibido a alteração do Sprint Backlog pelo Product Owner.

\(C) As histórias foram entregues meias prontas na Sprint Review.

(D) Seguem, em anexos, os cenários escritos em Gherkin.

(E) É necessário paciência no refinamento do backlog.

---

## Minhas respostas

| Questão | Resposta |
|---|---|
| 1 | |
| 2 | |
| 3 | |
| 4 | |
| 5 | |
| 6 | |
| 7 | |
| 8 | |
| 9 | |
| 10 | |
| 11 | |
| 12 | |
| 13 | |
| 14 | |
| 15 | |
