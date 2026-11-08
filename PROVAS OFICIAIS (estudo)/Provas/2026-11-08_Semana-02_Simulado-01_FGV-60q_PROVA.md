---
tipo: prova
fonte: oficial
disciplina: ["Português", "RLM", "Engenharia de Software e Ágil", "APF, SAFe e Testes", "Arquitetura e System Design", "Banco de Dados e SQL", "Linguagens e Frameworks", "Segurança", "DevOps e Nuvem", "IA", "Mobile e UI-UX", "Algoritmos, POO, SOLID e GoF", "Judiciário, LGPD e Governança", "Discursiva"]
assunto: "Simulado 01 · 60 questões oficiais FGV no formato TJPB + discursiva autoral (estudo de caso)"
semana: 2
data: 2026-11-08
banca: FGV
prova: "Simulado 01 (DATAPREV 2024 + TJ-AP 2024 + DPE-RS 2023)"
---

# Simulado 01 · formato TJPB 2026 (60 objetivas + estudo de caso)

> ⚠️ **Objetivas: questões oficiais da FGV**, Tipo 1, selecionadas e renumeradas no formato do edital do TJPB (10 Português + 10 RLM + 40 Específicas). **Discursiva: autoral, no estilo FGV, não oficial.** O Português da DATAPREV (já resolvido em 23/10) foi trocado por questões inéditas da TJ-AP 2024.

## Arquivos

| Arquivo | Para quê |
|---|---|
| `2026-11-08_Semana-02_Simulado-01_FGV-60q_PROVA.pdf` | Caderno de questões no modelo FGV (16 páginas): **imprimir frente e verso** |
| `2026-11-08_Semana-02_Simulado-01_FGV-60q_FOLHAS-DE-RESPOSTA.pdf` | Cartão de respostas (1–60) e folha de texto definitivo (30 linhas): **imprimir só frente** |
| `Correções/2026-11-08_Semana-02_Simulado-01_FGV-60q_GABARITO-NAO-ABRIR.pdf` | Gabarito oficial renumerado + padrão de resposta da discursiva. **Abrir só depois** |
| Provas originais | `2024-11-17_FGV-DATAPREV-2024_…`, `2024-03-24_FGV-TJ-AP-2024_…`, `2023-07-09_FGV-DPE-RS-2023_…` (`_PROVA-ORIGINAL.pdf`) |

## Como fazer

- **Tempo:** 5 horas (como no TJPB, 13h–18h): objetiva ~3h30, discursiva ~1h15, marcação ~15 min.
- Sem consulta, cronometrado. **Nada em branco**, **"?"** antes da letra nos chutes, **V/F nas INCORRETA/EXCETO**.
- Ao terminar: mandar as respostas (`1-A, 2-?C…`) e a foto da folha de texto definitivo.

## Composição (nº novo ← questão original)

| Parte | Nº | Prova de origem | Correspondência |
|---|---|---|---|
| Português | 1–10 | TJ-AP 2024 | 1←3, 2←6, 3←8, 4←10, 5←14, 6←15, 7←18, 8←19, 9←22, 10←25 |
| RLM | 11–16 | DATAPREV 2024 | 11←25, 12←26, 13←27, 14←28, 15←29, 16←30 |
| RLM | 17–20 | DPE-RS 2023 | 17←23, 18←25, 19←26, 20←28 |
| Específicas | 21–50 | DATAPREV 2024 | 21←41, 22←42, 23←43, 24←44, 25←45, 26←46, 27←47, 28←48, 29←49, 30←50, 31←51, 32←52, 33←53, 34←54, 35←55, 36←56, 37←57, 38←58, 39←59, 40←60, 41←61, 42←62, 43←63, 44←64, 45←65, 46←66, 47←67, 48←68, 49←69, 50←70 |
| Específicas | 51–60 | TJ-AP 2024 | 51←45, 52←51, 53←52, 54←57, 55←63, 56←67, 57←68, 58←72, 59←78, 60←80 |

## Questão discursiva (estudo de caso · 30 linhas · 40 pontos)

O Tribunal de Justiça do Estado Alfa implantou o sistema *e-CUSTAS*, que calcula e emite as guias de recolhimento de custas judiciais dos processos eletrônicos. Para cumprir o prazo de seis meses fixado pela Presidência, a equipe de desenvolvimento, composta por cinco analistas, decidiu não escrever testes automatizados. Os testes foram feitos manualmente, apenas na semana anterior à implantação, por um único analista, que percorreu as telas principais do sistema.

Nas duas primeiras semanas de funcionamento, a Secretaria de Tecnologia da Informação registrou os seguintes incidentes:

- **I.** guias com valor incorreto sempre que o processo tinha mais de um réu, situação prevista na tabela de custas do Tribunal, mas que não constava em nenhum artefato de requisitos do sistema;

- **II.** após a publicação de uma correção no cálculo dos juros de mora, a emissão de segunda via de guias, que funcionava normalmente, deixou de funcionar;

- **III.** tempo de resposta superior a 40 segundos para emitir guias no último dia dos prazos processuais, quando o número de acessos simultâneos aumentou cerca de dez vezes;

- **IV.** constatação, pela equipe de segurança da informação, de que o campo de busca por número do processo aceitava comandos SQL, o que permitiu a consulta indevida de nomes e números de CPF de partes de processos.

Em reunião, o diretor de TI afirmou que, para a próxima versão, pretende contratar mais três testadores para executar testes manuais ao final de cada entrega, por considerar que “mais pessoas testando significa mais qualidade”.

**Considerando a situação descrita, redija um texto dissertativo que atenda ao que se pede a seguir.**

**a) Analise criticamente o processo de desenvolvimento adotado pela equipe, relacionando cada um dos incidentes I a IV ao tipo de teste ou à atividade de engenharia de requisitos que poderia tê-lo evitado.**

**b) Avalie a proposta do diretor de TI à luz do conceito de pirâmide de testes e da automação de testes em um *pipeline* de integração contínua.**

**c) Proponha encaminhamentos para a próxima versão do *e-CUSTAS*, incluindo a verificação de segurança no ciclo de desenvolvimento e as providências relativas aos dados pessoais expostos.**

**A resposta deve ser redigida em até 30 (trinta) linhas.**

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
| 16 | |
| 17 | |
| 18 | |
| 19 | |
| 20 | |
| 21 | |
| 22 | |
| 23 | |
| 24 | |
| 25 | |
| 26 | |
| 27 | |
| 28 | |
| 29 | |
| 30 | |
| 31 | |
| 32 | |
| 33 | |
| 34 | |
| 35 | |
| 36 | |
| 37 | |
| 38 | |
| 39 | |
| 40 | |
| 41 | |
| 42 | |
| 43 | |
| 44 | |
| 45 | |
| 46 | |
| 47 | |
| 48 | |
| 49 | |
| 50 | |
| 51 | |
| 52 | |
| 53 | |
| 54 | |
| 55 | |
| 56 | |
| 57 | |
| 58 | |
| 59 | |
| 60 | |

**Discursiva:** foto em `discursivas/2026-11-08_e-CUSTAS.jpg`
