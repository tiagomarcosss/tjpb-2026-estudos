---
tipo: correcao
fonte: autoral
disciplina: ["APF, SAFe e Testes"]
assunto: "SAFe (ART, PI, papéis, backlog, PI Planning, ROAM, WSJF, IP Iteration, configurações) · 12 questões"
semana: 2
data: 2026-11-06
acertos: 9
total: 12
---

# Correção · SAFe · padrão FGV · 12 questões

**Bloco de 05/11, corrigido em 06/11/2026** · **Semana 2** · **Placar: 9/12 (75%)** · 3 erros · 0 em branco · **7 dos 9 acertos com dúvida (pontinho)**

**Respostas lidas das anotações do PDF:** 1-B · 2-A · 3-B · 4-B · 5-D · 6-D · 7-A · 8-C · 9-E · 10-B · 11-B · 12-A

> Questões autorais no estilo FGV, elaboradas para treino. Não são questões oficiais.

> **Como li as marcas:** a tabela "Minhas respostas" ficou vazia; usei os círculos nas letras. **Pontinho = candidata:** Q3 (B e E), Q4 (B e C), Q5 (A e D), Q6 (C e D), Q7 (A), Q8 (C e D, com A e B riscadas), Q9 (C, D e E, com A e B riscadas), Q10 (B e D). **Na Q9 há um "?" ao lado da (D)**: li como "não sei o que é Solution Demo". Q1, Q2, Q11 e Q12 sem pontinho. Na Q5 e na Q6 você fez as contas na margem, e estão certas. Na Q12 você marcou I ✓, II ✗ e III ✓. No topo da página 3 há uma nota digitada, "sempre o cliente em primeiro lugar", que não está ligada a nenhuma alternativa; não usei na correção.

| Questão | Assunto | Sua | Gabarito | Resultado |
|---|---|---|---|---|
| 1 | Papéis: RTE × Product Management | B | C | ❌ |
| 2 | Hierarquia do backlog (feature) | A | A | ✅ |
| 3 | Voto de confiança baixo | B | E | ❌ |
| 4 | ROAM | B | B | ✅ (com dúvida) |
| 5 | WSJF (conta) | D | D | ✅ (com dúvida) |
| 6 | 💻 WSJF em Python | D | D | ✅ (com dúvida) |
| 7 | IP Iteration | A | A | ✅ (com dúvida) |
| 8 | Objetivo do PI não comprometido | C | C | ✅ (com dúvida) |
| 9 | Eventos do ART | E | E | ✅ (com dúvida; "?" em Solution Demo) |
| 10 | Configurações (Large Solution) | B | B | ✅ (com dúvida) |
| 11 | Deploy × release / CD Pipeline | B | E | ❌ |
| 12 | ART (I/II/III) | A | A | ✅ |

**Por tipo:**

| Tipo | Questões | Placar |
|---|---|---|
| Papéis e configurações | 1, 10 | 1/2 |
| Backlog e ART | 2, 12 | 2/2 (sem dúvida) |
| PI Planning (voto, ROAM, IP Iteration, objetivos) | 3, 4, 7, 8 | 3/4 |
| WSJF (conta e código) | 5, 6 | 2/2 |
| Eventos do ART | 9 | 1/1 |
| Release on demand e CD Pipeline | 11 | 0/1 |

**Comparação:** primeiro bloco de SAFe. Na mesma disciplina, APF teve 3/8 em 03/11 e Tipos de teste 8/15 em 04/11; **SAFe teve 9/12, o melhor placar da Semana 2**. Mas só 2 acertos foram firmes (Q2 e Q12): os outros 7 vieram com pontinho em mais de uma candidata. O conteúdo foi reconhecido, só ainda não está firme. O ponto forte foi o **WSJF**: as duas contas estão certas, inclusive a da leitura de código (ponto fraco desde 30/10).

---

## Questão 1 · ❌ Errou

O Tribunal de Justiça organizou os nove times que desenvolvem o sistema JUSTIÇAPB+ em um Agile Release Train (ART), de acordo com o SAFe 6.0. A analista Ana foi designada para facilitar o PI Planning e as reuniões semanais de sincronização do trem, acompanhar os riscos do ART e ajudar a remover impedimentos que envolvem mais de um time. Ana não define o conteúdo das entregas nem prioriza o backlog do trem, e atua como líder-servidora.

O papel exercido por Ana no SAFe é o de:

(A) Product Owner;

❌ **(B) Product Management;** ← sua resposta

✅ **\(C) Release Train Engineer (RTE).**

(D) System Architect;

(E) Business Owner.

**Onde você se confundiu:** você grifou as pistas certas ("facilitar o PI Planning", "reuniões semanais", "riscos do ART", "remover impedimentos", "um time"), mas não usou a frase que **eliminava a B**: "Ana **não define o conteúdo** das entregas **nem prioriza o backlog** do trem". Definir o conteúdo e priorizar o ART Backlog é **exatamente** o trabalho do Product Management. Quando o enunciado diz o que a pessoa *não* faz, está riscando uma alternativa para você.

| Papel | Nível | O que faz |
|---|---|---|
| **RTE** | Trem (ART) | **Facilita**: PI Planning, sincronizações, riscos, impedimentos entre times. Líder-servidor |
| **Product Management** | Trem (ART) | **Define o quê**: features e prioridade do ART Backlog |
| Product Owner | Time | Stories e Team Backlog |
| System Architect | Trem | Visão técnica e arquitetura |
| Business Owner | Trem | Valor de negócio, aceita os objetivos do PI |

📌 **RTE = Scrum Master do trem** (facilita, é líder-servidor, não define escopo) · **Product Management = PO do trem** (define e prioriza as features). "Não prioriza o backlog" elimina o Product Management.

---

## Questão 2 · ✅ Acertou

No ART responsável pelo sistema e-PROTOCOLO, foi registrado o item "Assinatura com certificado ICP-Brasil no peticionamento eletrônico". A estimativa indica que ele será entregue por três times ao longo de um único PI. O item descreve uma hipótese de benefício ("reduzir em 30% as petições devolvidas por falta de assinatura") e tem critérios de aceite definidos. Ele está registrado no ART Backlog.

De acordo com o SAFe, esse item é classificado como:

✅ **(A) feature, cuja priorização no ART Backlog cabe ao Product Management;** ← sua resposta

(B) story, cuja priorização cabe ao Product Owner de cada um dos três times;

\(C) épico, que exige Lean Business Case e é aprovado pelo Product Management;

(D) capability, mantida no ART Backlog e priorizada pelo Release Train Engineer;

(E) feature, cuja priorização no ART Backlog cabe ao Release Train Engineer.

Acerto firme. Você grifou "um único PI" e "Product Management". A (E) acerta o tipo e erra o dono (o RTE não prioriza nada; veja a Q1). A (B) é story, que cabe numa iteração e num só time. O épico (C) passa de um PI e é aprovado no portfólio. A capability (D) fica no Solution Backlog, na configuração Large Solution.

📌 **Épico** (> 1 PI, Lean Business Case, portfólio) > **Capability** (vários ARTs, Large Solution) > **Feature** (1 PI, hipótese de benefício + critérios de aceite, ART Backlog, **Product Management**) > **Story** (1 iteração, **PO**).

---

## Questão 3 · ❌ Errou

Ao final do segundo dia do PI Planning do ART do sistema e-CUSTAS, depois da análise dos riscos, o Release Train Engineer conduziu o voto de confiança: cada participante levantou de um a cinco dedos para indicar sua confiança no cumprimento dos objetivos do PI. A média obtida foi de dois dedos, e vários times apontaram que o plano dependia de uma equipe de infraestrutura já sobrecarregada.

Segundo o SAFe, diante desse resultado:

(A) o RTE registra o resultado e o plano segue sem alterações, pois o voto tem caráter apenas informativo;

❌ **(B) os Business Owners redefinem os objetivos comprometidos de cada time, sem participação dos próprios times;** ← sua resposta

\(C) o plano é aprovado, e a baixa confiança será tratada no Inspect & Adapt, ao final do PI;

(D) os objetivos de baixa confiança passam automaticamente para a IP Iteration;

✅ **(E) o plano é retrabalhado ainda durante o evento, até que se alcance um nível de confiança aceitável.**

**Onde você se confundiu:** você ficou entre B e E (pontinho nas duas) e escolheu a B. A pista para descartá-la está no fim: "**sem participação dos próprios times**". No SAFe, **quem planeja e se compromete são os times**. Os Business Owners dão valor de negócio (1 a 10) aos objetivos, mas não reescrevem o plano por cima dos times. Tirar os times do próprio compromisso vai contra a ideia do voto de confiança, que é justamente perguntar a eles se acreditam no plano.

As outras: (A) o voto não é só informativo, porque confiança baixa obriga a agir; (C) não se adia para o I&A, porque o PI começaria com um plano em que ninguém acredita; (D) a IP Iteration não recebe objetivos (veja a Q7).

📌 **Voto de confiança** (1 a 5 dedos, no fim do PI Planning): média baixa → **os times retrabalham o plano ainda no evento**, até a confiança ficar aceitável. Quem se compromete com o plano são os times.

---

## Questão 4 · ✅ Acertou (com dúvida)

Durante o PI Planning do ART do sistema SIGEP-PB, os seguintes riscos foram discutidos com todo o trem:

I\. o fornecedor do módulo de biometria pode atrasar a entrega da biblioteca; o analista Carlos assumiu a responsabilidade de acompanhar o contrato e reportar a situação na sincronização semanal;

II\. havia o risco de faltar licença do servidor de homologação, mas a compra foi confirmada pela Diretoria de TI durante o próprio evento;

III\. uma eventual greve dos servidores pode reduzir a disponibilidade dos usuários para validação; como não há ação possível do ART, o trem decidiu seguir com o plano;

IV\. a API de autenticação do Gov.br pode não ficar pronta a tempo; foi definido o uso temporário de login local, para reduzir o impacto caso o atraso ocorra.

De acordo com a técnica ROAM, os riscos I, II, III e IV foram tratados, respectivamente, como:

(A) Resolved, Owned, Accepted e Mitigated;

✅ **(B) Owned, Resolved, Accepted e Mitigated;** ← sua resposta

\(C) Owned, Resolved, Mitigated e Accepted;

(D) Mitigated, Resolved, Accepted e Owned;

(E) Accepted, Resolved, Owned e Mitigated.

Você ficou entre B e C, que só diferem em III e IV. A pista para desempatar: no III, "**não há ação possível** … seguir com o plano" = **Accepted** (aceita-se o risco). No IV, "**para reduzir o impacto**" = **Mitigated** (existe um plano B). A (C) troca os dois.

📌 **ROAM:** **R**esolved = deixou de ser risco · **O**wned = alguém assume acompanhar · **A**ccepted = nada a fazer, segue o plano · **M**itigated = há ação para reduzir a probabilidade ou o impacto.

---

## Questão 5 · ✅ Acertou (com dúvida)

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

✅ **(D) Alerta de prazo, Integração com o Gov.br, Migração de relatórios e Painel estatístico;** ← sua resposta

(E) Integração com o Gov.br, Painel estatístico, Alerta de prazo e Migração de relatórios.

Suas contas na margem estão certas:

| Feature | Custo do atraso | ÷ Tamanho | WSJF | Ordem |
|---|---|---|---|---|
| Alerta de prazo | 5 + 8 + 2 = 15 | 3 | **5,0** | 1º |
| Integração Gov.br | 8 + 5 + 8 = 21 | 5 | **4,2** | 2º |
| Migração | 3 + 2 + 1 = 6 | 2 | **3,0** | 3º |
| Painel | 13 + 5 + 5 = 23 | 13 | **1,77** | 4º |

O pontinho na (A) mostra a armadilha: **(A) ordena só pelo custo do atraso** (23, 21, 15, 6) e esquece de dividir pelo tamanho. A (B) ordena só pelo **menor tamanho**, a (C) é a ordem **invertida** e a (E) ordena só pela redução de risco.

📌 **WSJF = custo do atraso ÷ tamanho**, com custo do atraso = valor + criticidade de tempo + redução de risco/oportunidade. **Maior WSJF primeiro.** O item grande e valioso (Painel) cai para o fim.

---

## Questão 6 · ✅ Acertou (com dúvida)

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

✅ **(D) ['Intimacoes', 'Custas', 'Peticionamento'];** ← sua resposta

(E) ['Peticionamento', 'Custas', 'Intimacoes'].

Bom rastreio: na margem você escreveu 13/13 = 1, 16/5 = 3,2 e 6/2 = 3, e numerou a ordem. `reverse=True` = do maior para o menor → Intimacoes (3,2), Custas (3,0), Peticionamento (1,0). A (C), onde você pôs pontinho, é a ordem **só pelo custo do atraso** (16, 13, 6), a mesma armadilha da Q5. A (A) é a lista na ordem original (sem o `sorted`), e a (E) é a ordem com `reverse=False`.

📌 **`sorted(..., reverse=True)`** = do maior para o menor. Na conta do WSJF, conferir sempre se a alternativa **dividiu pelo tamanho**: "maior custo do atraso primeiro" é o distrator clássico.

---

## Questão 7 · ✅ Acertou (com dúvida)

No PI Planning do ART do sistema e-JUS PB, a capacidade das quatro iterações de desenvolvimento não foi suficiente para todas as features desejadas. O gestor Marcos propôs reservar a IP Iteration, a última iteração do PI, para encaixar as três features que sobraram. A analista que atua como Release Train Engineer explicou que, segundo o SAFe, a proposta não é adequada, porque:

✅ **(A) não se planejam features para a IP Iteration, destinada a inovação, capacitação, Inspect & Adapt e planejamento do próximo PI, além de servir como margem de estimativa;** ← sua resposta

(B) a IP Iteration existe justamente para absorver o escopo que excede a capacidade das iterações de desenvolvimento, desde que aprovado pelos Business Owners;

\(C) a IP Iteration só existe na configuração Portfolio, não se aplicando a um ART que adota apenas o Essential SAFe;

(D) a IP Iteration deve ser eliminada sempre que houver features pendentes, para aumentar a velocidade do ART;

(E) as features só podem ser planejadas na IP Iteration se forem classificadas como objetivos comprometidos.

Você circulou "não é adequada" e foi direto na A. A (B) diz o contrário do SAFe (é justamente o que o Marcos quer fazer). A (C) erra porque a IP Iteration existe em **todas** as configurações, inclusive na Essential, já que faz parte do PI. A (D) é antipadrão: sem a IP, some a margem do plano. A (E) inventa uma exceção.

📌 **IP Iteration** (Innovation and Planning, a última do PI) = inovação, capacitação, Inspect & Adapt, planejamento do próximo PI e **margem de estimativa**. **Nunca se planejam features nela.**

---

## Questão 8 · ✅ Acertou (com dúvida)

No PI Planning do ART do sistema SISJUD-PB, o time de integração planejou o objetivo "Disponibilizar o login pelo Gov.br no portal do advogado". Como a entrega depende de uma API externa com cronograma incerto, a analista Beatriz, Scrum Master/Team Coach do time, sugeriu registrá-lo como objetivo do PI não comprometido.

De acordo com o SAFe, em relação a esse objetivo, é correto afirmar que:

(A) fica fora do plano e da capacidade do time, sendo executado apenas se sobrar tempo ao final do PI;

(B) não recebe valor de negócio dos Business Owners, pois não integra o compromisso do time;

✅ **\(C) integra o plano e consome capacidade do time, mas não conta como compromisso caso não seja entregue em razão da incerteza;** ← sua resposta

(D) é transferido automaticamente para o ART Backlog do PI seguinte, sem passar por nova priorização;

(E) passa a ser responsabilidade do Release Train Engineer, que deve garantir sua entrega.

Você riscou A e B (certo) e ficou entre C e D. A pista contra a (D): "**automaticamente**" e "**sem passar por nova priorização**". No SAFe, tudo o que volta ao backlog é **priorizado de novo** pelo WSJF. Palavras absolutas como essas costumam marcar o distrator.

📌 **Objetivo não comprometido:** **está no plano, consome capacidade e recebe valor de negócio**, mas não conta como compromisso se não for entregue. Serve para proteger a previsibilidade quando há incerteza.

---

## Questão 9 · ✅ Acertou (com dúvida; "?" em Solution Demo)

O ART do sistema e-PROTOCOLO realiza, entre outros, os seguintes eventos:

- ao final de cada iteração de duas semanas, os times apresentam aos Business Owners e demais interessados o sistema completo, já integrado, funcionando em ambiente de homologação;
- semanalmente, o Release Train Engineer reúne os Scrum Masters/Team Coaches dos times para tratar impedimentos e dependências entre eles;
- ao final do PI, o trem faz uma demonstração de tudo o que foi entregue, analisa métricas de previsibilidade e conduz um workshop de solução de problemas com análise de causa raiz.

Os eventos descritos correspondem, respectivamente, a:

(A) Solution Demo, PO Sync e PI Planning;

(B) System Demo, PO Sync e Inspect & Adapt;

\(C) Iteration Review, Coach Sync e PI Planning;

(D) Solution Demo, Coach Sync e Inspect & Adapt;

✅ **(E) System Demo, Coach Sync e Inspect & Adapt.** ← sua resposta

Você riscou A e B pelo PO Sync (certo: quem se reúne é o **RTE com os Scrum Masters**, então é o Coach Sync). O "?" ficou na (D), ou seja, a dúvida era **Solution Demo × System Demo**:

| Demo | Configuração | Quem integra | Quando |
|---|---|---|---|
| Iteration Review | Time | Só o incremento do time | Fim de cada iteração |
| **System Demo** | **ART** (Essential) | **O sistema inteiro do trem**, integrado | Fim de **cada iteração** |
| **Solution Demo** | **Large Solution** | **Vários ARTs + fornecedores** | No PI (no fim ou perto dele) |

O cenário é **um ART** (o do e-PROTOCOLO) a cada iteração → **System Demo**. Solution Demo só aparece quando há Solution Train (Q10).

📌 **System Demo** = sistema integrado do ART, a cada iteração · **Solution Demo** = vários ARTs (Large Solution) · **Coach Sync** = RTE + Scrum Masters · **PO Sync** = Product Management + POs · **I&A** = fim do PI (PI System Demo + métricas + workshop de causa raiz).

---

## Questão 10 · ✅ Acertou (com dúvida)

Um consórcio de tribunais vai desenvolver um sistema nacional de execução penal. A solução exigirá a coordenação de três Agile Release Trains, cada um com cerca de 100 pessoas, e de dois fornecedores externos, que entregarão componentes de hardware e de software. Os ARTs têm muitas dependências entre si, e as entregas precisam ser integradas e demonstradas em conjunto.

A configuração SAFe mais enxuta que contempla essa coordenação, com a estrutura correspondente, é:

(A) Essential SAFe, com um único ART ampliado para incluir todos os profissionais dos três trens;

✅ **(B) Large Solution SAFe, com um Solution Train que coordena os ARTs e os fornecedores, facilitado pelo Solution Train Engineer;** ← sua resposta

\(C) Portfolio SAFe, com o Release Train Engineer de um dos ARTs acumulando a coordenação dos três trens;

(D) Large Solution SAFe, com as capabilities priorizadas pelo Product Owner de cada time;

(E) Essential SAFe, com o Solution Management substituindo o Product Management em cada ART.

Você ficou entre B e D, que acertam a configuração. A diferença está no **dono**: capabilities são priorizadas pelo **Solution Management**, nunca pelo PO de um time (o PO cuida de stories). A (A) é impossível: 300 pessoas não cabem num ART (50 a 125). A (C) não é "a mais enxuta" e dá ao RTE um papel que é do **STE**. A (E) põe um papel do Large Solution dentro da Essential.

📌 **Large Solution** = vários ARTs + fornecedores → **Solution Train**, **STE** (o "RTE dos trens"), **Solution Management** (prioriza capabilities) e **Solution Demo**. Regra de três: RTE → STE · Product Management → Solution Management · feature → capability.

---

## Questão 11 · ❌ Errou

O ART do sistema e-PROTOCOLO implanta código em produção toda semana. Uma nova funcionalidade de petição intermediária simplificada já está em produção, mas permanece desativada por uma feature toggle. A Presidência do Tribunal decidiu que ela só será ativada para os advogados após uma campanha de divulgação, daqui a um mês, no meio do PI.

Sobre essa situação, à luz do SAFe, é correto afirmar que:

(A) o ART viola o princípio da cadência, pois as liberações aos usuários devem coincidir com o fim do PI;

❌ **(B) trata-se do aspecto Continuous Exploration da Continuous Delivery Pipeline, que consiste em levar o código ao ambiente de produção;** ← sua resposta

\(C) a prática é incompatível com o SAFe, que exige que todo deploy seja imediatamente liberado aos usuários;

(D) deploy e release são sinônimos no SAFe, de modo que a funcionalidade já foi liberada aos advogados;

✅ **(E) o cenário ilustra a separação entre deploy e release, coerente com o lema "develop on cadence, release on demand".**

**Onde você se confundiu:** você grifou as pistas certas ("permanece desativada por uma feature toggle", "só será ativada para os advogados após uma campanha"). Elas descrevem **código em produção, mas ainda não liberado** = deploy sem release. A (B) mistura os nomes da pipeline: **Continuous Exploration** é a etapa de **decidir o que construir** (hipóteses, pesquisa com usuários, alinhamento). Quem leva o código à produção é o **Continuous Deployment**. Mesmo que a (B) tivesse o nome certo, ela não explica a situação, que é o atraso proposital da liberação.

| Aspecto da pipeline | Pergunta | No cenário |
|---|---|---|
| Continuous Exploration | O que construir? | (antes: a ideia da petição simplificada) |
| Continuous Integration | Build + testes automatizados passam? | — |
| **Continuous Deployment** | **Está em produção?** | Sim, toda semana, mas **oculta** pela toggle |
| **Release on Demand** | **O usuário já tem acesso?** | Só depois da campanha, quando o negócio decidir |

As outras: (A) inverte o lema, porque a liberação **não** precisa coincidir com o fim do PI; (C) e (D) negam a separação deploy × release, que é justamente o ponto do SAFe.

📌 **Deploy ≠ release.** Deploy = pôr em produção (pode ficar oculto por **feature toggle**) · release = liberar ao usuário quando o negócio quiser. **"Develop on cadence, release on demand."** Pipeline: **Exploration** (o quê?) → **Integration** (build/testes) → **Deployment** (produção) → **Release on Demand** (usuário).

---

## Questão 12 · ✅ Acertou

A Secretaria de Tecnologia da Informação do Tribunal estuda adotar o SAFe e elaborou as seguintes afirmativas sobre o Agile Release Train (ART):

I\. o ART é uma equipe de equipes ágeis, normalmente com 50 a 125 pessoas, organizada em torno de um fluxo de valor e de existência duradoura; → **V**

II\. ao término de cada projeto, o ART é desmontado e seus membros são realocados, pois o SAFe financia projetos, e não fluxos de valor; → **F**

III\. os times de um ART trabalham com iterações sincronizadas, com as mesmas datas de início e de término, e planejam juntos no PI Planning. → **V**

Está correto o que se afirma em:

✅ **(A) I e III, apenas;** ← sua resposta

(B) I, apenas;

\(C) II, apenas;

(D) II e III, apenas;

(E) I, II e III.

Acerto firme, com V/F escrito ao lado de cada item (✓ ✗ ✓) e "projetos" grifado no II. O II inverte o SAFe, que **financia o fluxo de valor (o trem) e não o projeto**; por isso o ART é permanente.

📌 **ART** = equipe de equipes (50 a 125 pessoas), **permanente**, em torno de um **fluxo de valor**, com iterações sincronizadas e PI Planning conjunto. SAFe financia fluxo de valor, não projeto.

---

## Para o caderno de erros

| Assunto | Por que errei | Regra certa |
|---|---|---|
| RTE × Product Management (Q1) | Ignorei a frase "não define o conteúdo nem prioriza o backlog" | RTE facilita (Scrum Master do trem) · Product Management define e prioriza as features. Frase de "não faz" no enunciado = eliminar quem faz |
| Voto de confiança (Q3) | Entre B e E, aceitei que os Business Owners refazem os objetivos sem os times | Confiança baixa → os **times** retrabalham o plano ainda no evento |
| CD Pipeline / deploy × release (Q11) | Confundi Continuous Exploration (o que construir) com Continuous Deployment (pôr em produção) | Feature toggle = deploy sem release · "develop on cadence, release on demand" |
| System × Solution Demo (Q9, "?") | Não sabia o que é Solution Demo | System Demo = 1 ART, a cada iteração · Solution Demo = vários ARTs (Large Solution) |

---

## O que estudar agora

| Quando | O que fazer |
|---|---|
| Hoje · almoço | Próximo item de Português da fila: **A3** (pronome, preposição, conjunção), abrindo com 10 min de predicativo × adjunto e OD × OI |
| Hoje · 19h (Bloco 1) | **SAST × DAST × IAST e SonarQube** (fila nº 7). Antes, 5 min: reler o mapa SAFe nas seções de **papéis** (RTE × PM × STE) e da **CD Pipeline** |
| Hoje · 20h (Bloco 2) | Bloco só de SAST/DAST |
| Hoje · 22:40 (revisão) | Reler as 11 regras 📌 de SAFe. Refazer **sem olhar**: Q1 (dizer em voz alta "quem facilita × quem prioriza"), Q3 e Q11 (desenhar a pipeline de 4 caixas e marcar onde fica a feature toggle) |
| Sáb 07/11 | Recuperação: bloco de Requisitos (fila nº 4) → APF real (nº 8) |
| Dom 08/11 · 13h | 1º simulado oficial |
