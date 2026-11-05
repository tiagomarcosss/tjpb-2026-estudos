---
tipo: bloco
fonte: autoral
status: pendente
disciplina: ["APF, SAFe e Testes"]
assunto: "SAFe (ART, PI, papéis, backlog, PI Planning, ROAM, WSJF, IP Iteration, configurações)"
semana: 2
data: 2026-11-05
---

# Bloco · SAFe · padrão FGV (12 questões)

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

> Assunto único: SAFe (fila nº 6), com base no SAFe 6.0. Papéis, ART, PI, hierarquia do backlog, PI Planning, ROAM, objetivos do PI, WSJF, eventos do ART, IP Iteration, release on demand e configurações. Mapa: [[mapa-safe]]. Marque "?" no que não souber e nunca deixe em branco.

## Questão 1

O Tribunal de Justiça organizou os nove times que desenvolvem o sistema JUSTIÇAPB+ em um Agile Release Train (ART), de acordo com o SAFe 6.0. A analista Ana foi designada para facilitar o PI Planning e as reuniões semanais de sincronização do trem, acompanhar os riscos do ART e ajudar a remover impedimentos que envolvem mais de um time. Ana não define o conteúdo das entregas nem prioriza o backlog do trem, e atua como líder-servidora.

O papel exercido por Ana no SAFe é o de:

(A) Product Owner;

(B) Product Management;

\(C) Release Train Engineer (RTE);

(D) System Architect;

(E) Business Owner.

---

## Questão 2

No ART responsável pelo sistema e-PROTOCOLO, foi registrado o item "Assinatura com certificado ICP-Brasil no peticionamento eletrônico". A estimativa indica que ele será entregue por três times ao longo de um único PI. O item descreve uma hipótese de benefício ("reduzir em 30% as petições devolvidas por falta de assinatura") e tem critérios de aceite definidos. Ele está registrado no ART Backlog.

De acordo com o SAFe, esse item é classificado como:

(A) feature, cuja priorização no ART Backlog cabe ao Product Management;

(B) story, cuja priorização cabe ao Product Owner de cada um dos três times;

\(C) épico, que exige Lean Business Case e é aprovado pelo Product Management;

(D) capability, mantida no ART Backlog e priorizada pelo Release Train Engineer;

(E) feature, cuja priorização no ART Backlog cabe ao Release Train Engineer.

---

## Questão 3

Ao final do segundo dia do PI Planning do ART do sistema e-CUSTAS, depois da análise dos riscos, o Release Train Engineer conduziu o voto de confiança: cada participante levantou de um a cinco dedos para indicar sua confiança no cumprimento dos objetivos do PI. A média obtida foi de dois dedos, e vários times apontaram que o plano dependia de uma equipe de infraestrutura já sobrecarregada.

Segundo o SAFe, diante desse resultado:

(A) o RTE registra o resultado e o plano segue sem alterações, pois o voto tem caráter apenas informativo;

(B) os Business Owners redefinem os objetivos comprometidos de cada time, sem participação dos próprios times;

\(C) o plano é aprovado, e a baixa confiança será tratada no Inspect & Adapt, ao final do PI;

(D) os objetivos de baixa confiança passam automaticamente para a IP Iteration;

(E) o plano é retrabalhado ainda durante o evento, até que se alcance um nível de confiança aceitável.

---

## Questão 4

Durante o PI Planning do ART do sistema SIGEP-PB, os seguintes riscos foram discutidos com todo o trem:

I\. o fornecedor do módulo de biometria pode atrasar a entrega da biblioteca; o analista Carlos assumiu a responsabilidade de acompanhar o contrato e reportar a situação na sincronização semanal;

II\. havia o risco de faltar licença do servidor de homologação, mas a compra foi confirmada pela Diretoria de TI durante o próprio evento;

III\. uma eventual greve dos servidores pode reduzir a disponibilidade dos usuários para validação; como não há ação possível do ART, o trem decidiu seguir com o plano;

IV\. a API de autenticação do Gov.br pode não ficar pronta a tempo; foi definido o uso temporário de login local, para reduzir o impacto caso o atraso ocorra.

De acordo com a técnica ROAM, os riscos I, II, III e IV foram tratados, respectivamente, como:

(A) Resolved, Owned, Accepted e Mitigated;

(B) Owned, Resolved, Accepted e Mitigated;

\(C) Owned, Resolved, Mitigated e Accepted;

(D) Mitigated, Resolved, Accepted e Owned;

(E) Accepted, Resolved, Owned e Mitigated.

---

## Questão 5

O Product Management do ART do sistema JURIS-PB usa o WSJF (Weighted Shortest Job First) do SAFe para priorizar quatro features. As notas relativas atribuídas foram:

| Feature | Valor para o negócio/usuário | Criticidade de tempo | Redução de risco/Habilitação de oportunidade | Tamanho do trabalho |
|---|---|---|---|---|
| Alerta de prazo processual | 5 | 8 | 2 | 3 |
| Painel estatístico da Presidência | 13 | 5 | 5 | 13 |
| Integração com o Gov.br | 8 | 5 | 8 | 5 |
| Migração de relatórios antigos | 3 | 2 | 1 | 2 |

Aplicando corretamente o WSJF, a ordem de prioridade das features, da primeira para a última, é:

(A) Painel estatístico, Integração com o Gov.br, Alerta de prazo e Migração de relatórios;

(B) Migração de relatórios, Alerta de prazo, Integração com o Gov.br e Painel estatístico;

\(C) Painel estatístico, Migração de relatórios, Integração com o Gov.br e Alerta de prazo;

(D) Alerta de prazo, Integração com o Gov.br, Migração de relatórios e Painel estatístico;

(E) Integração com o Gov.br, Painel estatístico, Alerta de prazo e Migração de relatórios.

---

## Questão 6

O analista Douglas escreveu o script Python a seguir para apoiar a priorização das features do ART do sistema e-PROTOCOLO pelo WSJF.

```python
features = [
    {"nome": "Peticionamento", "valor": 8, "tempo": 3, "risco": 2, "tamanho": 13},
    {"nome": "Intimacoes",     "valor": 5, "tempo": 8, "risco": 3, "tamanho": 5},
    {"nome": "Custas",         "valor": 3, "tempo": 2, "risco": 1, "tamanho": 2},
]

for f in features:
    custo_atraso = f["valor"] + f["tempo"] + f["risco"]
    f["wsjf"] = custo_atraso / f["tamanho"]

ordem = sorted(features, key=lambda f: f["wsjf"], reverse=True)
print([f["nome"] for f in ordem])
```

Ao ser executado, o script exibirá:

(A) ['Peticionamento', 'Intimacoes', 'Custas'];

(B) ['Custas', 'Intimacoes', 'Peticionamento'];

\(C) ['Intimacoes', 'Peticionamento', 'Custas'];

(D) ['Intimacoes', 'Custas', 'Peticionamento'];

(E) ['Peticionamento', 'Custas', 'Intimacoes'].

---

## Questão 7

No PI Planning do ART do sistema e-JUS PB, a capacidade das quatro iterações de desenvolvimento não foi suficiente para todas as features desejadas. O gestor Marcos propôs reservar a IP Iteration, a última iteração do PI, para encaixar as três features que sobraram. A analista que atua como Release Train Engineer explicou que, segundo o SAFe, a proposta não é adequada, porque:

(A) não se planejam features para a IP Iteration, destinada a inovação, capacitação, Inspect & Adapt e planejamento do próximo PI, além de servir como margem de estimativa;

(B) a IP Iteration existe justamente para absorver o escopo que excede a capacidade das iterações de desenvolvimento, desde que aprovado pelos Business Owners;

\(C) a IP Iteration só existe na configuração Portfolio, não se aplicando a um ART que adota apenas o Essential SAFe;

(D) a IP Iteration deve ser eliminada sempre que houver features pendentes, para aumentar a velocidade do ART;

(E) as features só podem ser planejadas na IP Iteration se forem classificadas como objetivos comprometidos.

---

## Questão 8

No PI Planning do ART do sistema SISJUD-PB, o time de integração planejou o objetivo "Disponibilizar o login pelo Gov.br no portal do advogado". Como a entrega depende de uma API externa com cronograma incerto, a analista Beatriz, Scrum Master/Team Coach do time, sugeriu registrá-lo como objetivo do PI não comprometido.

De acordo com o SAFe, em relação a esse objetivo, é correto afirmar que:

(A) fica fora do plano e da capacidade do time, sendo executado apenas se sobrar tempo ao final do PI;

(B) não recebe valor de negócio dos Business Owners, pois não integra o compromisso do time;

\(C) integra o plano e consome capacidade do time, mas não conta como compromisso caso não seja entregue em razão da incerteza;

(D) é transferido automaticamente para o ART Backlog do PI seguinte, sem passar por nova priorização;

(E) passa a ser responsabilidade do Release Train Engineer, que deve garantir sua entrega.

---

## Questão 9

O ART do sistema e-PROTOCOLO realiza, entre outros, os seguintes eventos:

- ao final de cada iteração de duas semanas, os times apresentam aos Business Owners e demais interessados o sistema completo, já integrado, funcionando em ambiente de homologação;
- semanalmente, o Release Train Engineer reúne os Scrum Masters/Team Coaches dos times para tratar impedimentos e dependências entre eles;
- ao final do PI, o trem faz uma demonstração de tudo o que foi entregue, analisa métricas de previsibilidade e conduz um workshop de solução de problemas com análise de causa raiz.

Os eventos descritos correspondem, respectivamente, a:

(A) Solution Demo, PO Sync e PI Planning;

(B) System Demo, PO Sync e Inspect & Adapt;

\(C) Iteration Review, Coach Sync e PI Planning;

(D) Solution Demo, Coach Sync e Inspect & Adapt;

(E) System Demo, Coach Sync e Inspect & Adapt.

---

## Questão 10

Um consórcio de tribunais vai desenvolver um sistema nacional de execução penal. A solução exigirá a coordenação de três Agile Release Trains, cada um com cerca de 100 pessoas, e de dois fornecedores externos, que entregarão componentes de hardware e de software. Os ARTs têm muitas dependências entre si, e as entregas precisam ser integradas e demonstradas em conjunto.

A configuração SAFe mais enxuta que contempla essa coordenação, com a estrutura correspondente, é:

(A) Essential SAFe, com um único ART ampliado para incluir todos os profissionais dos três trens;

(B) Large Solution SAFe, com um Solution Train que coordena os ARTs e os fornecedores, facilitado pelo Solution Train Engineer;

\(C) Portfolio SAFe, com o Release Train Engineer de um dos ARTs acumulando a coordenação dos três trens;

(D) Large Solution SAFe, com as capabilities priorizadas pelo Product Owner de cada time;

(E) Essential SAFe, com o Solution Management substituindo o Product Management em cada ART.

---

## Questão 11

O ART do sistema e-PROTOCOLO implanta código em produção toda semana. Uma nova funcionalidade de petição intermediária simplificada já está em produção, mas permanece desativada por uma feature toggle. A Presidência do Tribunal decidiu que ela só será ativada para os advogados após uma campanha de divulgação, daqui a um mês, no meio do PI.

Sobre essa situação, à luz do SAFe, é correto afirmar que:

(A) o ART viola o princípio da cadência, pois as liberações aos usuários devem coincidir com o fim do PI;

(B) trata-se do aspecto Continuous Exploration da Continuous Delivery Pipeline, que consiste em levar o código ao ambiente de produção;

\(C) a prática é incompatível com o SAFe, que exige que todo deploy seja imediatamente liberado aos usuários;

(D) deploy e release são sinônimos no SAFe, de modo que a funcionalidade já foi liberada aos advogados;

(E) o cenário ilustra a separação entre deploy e release, coerente com o lema "develop on cadence, release on demand".

---

## Questão 12

A Secretaria de Tecnologia da Informação do Tribunal estuda adotar o SAFe e elaborou as seguintes afirmativas sobre o Agile Release Train (ART):

I\. o ART é uma equipe de equipes ágeis, normalmente com 50 a 125 pessoas, organizada em torno de um fluxo de valor e de existência duradoura;

II\. ao término de cada projeto, o ART é desmontado e seus membros são realocados, pois o SAFe financia projetos, e não fluxos de valor;

III\. os times de um ART trabalham com iterações sincronizadas, com as mesmas datas de início e de término, e planejam juntos no PI Planning.

Está correto o que se afirma em:

(A) I e III, apenas;

(B) I, apenas;

\(C) II, apenas;

(D) II e III, apenas;

(E) I, II e III.

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
