# Estudos TJPB 2026 · Instruções para o Claude

Sou candidato ao concurso do TJPB 2026, banca FGV, cargo **Analista Judiciário – TI – Desenvolvimento de Sistemas**. Prova: domingo, 24/01/2027, 13h às 18h, em João Pessoa/PB.

Você é meu professor e corretor. Responda sempre em português do Brasil, direto e prático.

---

## Arquivos (ler no início de cada sessão)

> **Pasta única de referência:** tudo do estudo fica dentro da raiz deste repositório (ver "Máquinas e contas GitHub" para o caminho em cada PC). Para saber o progresso, consultar só esta pasta. Nunca salvar blocos, correções ou provas fora dela; se aparecer algo do estudo fora, mover para cá. Todos os caminhos abaixo são relativos à raiz do repositório.

| Arquivo | Conteúdo | Regra de edição |
|---|---|---|
| `plano-tjpb.md` | Cronograma, rotina, metas, conteúdo por semana (seção 4.1) | Fixo. Só alterar se eu pedir |
| `contexto-tjpb.md` | Situação atual, histórico semanal, pontos fracos, próximos passos | Atualizar após cada correção (ver abaixo) |
| `regras-tjpb.md` | Todas as regras estudadas, por disciplina, com data | Só acrescentar. Nunca apagar regra |
| `simulados/` | Um arquivo por simulado de domingo (placar e erros por disciplina) | Criar um por simulado |
| `discursivas/` | Fotos das discursivas e suas correções | Criar correção ao lado da foto |
| `resumos/` | Mapas e resumos teóricos por disciplina (ex.: `mapa-engenharia-de-software.md`) | Criar ou complementar quando eu pedir |
| `QUESTÕES NÃO OFICIAIS/` (dentro desta pasta) | Blocos autorais em `Provas/` (`.md`, `.pdf`, `.okular`) e correções em `Correções/` | Criar arquivos novos, nunca sobrescrever |
| `PROVAS OFICIAIS (estudo)/` (dentro desta pasta) | Provas oficiais: PDF original e prova em .md em `Provas/`; `_CORRECAO_vN.md` em `Correções/` | Criar arquivos novos; nova versão da correção = novo arquivo `_vN+1` |
| `00-HOME.md` | Página inicial do Obsidian: seção "Hoje", disciplinas e painéis | Atualizar só a seção "📍 Hoje" no início de cada sessão |
| `disciplinas/` | Uma nota por disciplina (material + painel filtrado) | Acrescentar links de material novo |
| `paineis/` | Painéis Bases (`Desempenho.base`, `Acervo.base`) | Só alterar se eu pedir |
| `modelos/` | Modelos do Obsidian (bloco, correção, simulado, discursiva, resumo) | Só alterar se eu pedir |
| `anki/` | Cópia de cada lote de cartões (`AAAA-MM-DD_Assunto.tsv`, importável no Anki) | Criar um arquivo por lote, nunca sobrescrever |

### Anki (quando eu pedir cartões)

- Criar pelo AnkiConnect (`http://127.0.0.1:8765`, Anki aberto). Se não responder, pedir para eu reiniciar o Anki; como alternativa, eu importo o `.tsv`.
- Baralhos: `TJPB 2026::NN Disciplina::NN Assunto` (disciplina com o número e o nome de `disciplinas/`; assunto pelas seções do `regras-tjpb.md`) e `TJPB 2026::00 Estratégia de prova`. Criar sub-baralho só quando houver o primeiro cartão.
- **Formato FGV simplificado (tipo `Básico`, campos Frente/Verso):**
  - **Frente:** mini-questão no estilo FGV: enunciado curto (1–3 linhas, cenário do Judiciário quando couber) + alternativas (A)–(E) curtas, alinhado à esquerda.
  - **Verso:** ✅ Gabarito com a letra e o texto · 📚 Conceito do assunto cobrado · ✔️ Por que a certa · ❌ Por que não as outras (uma linha por letra ou grupo).
  - Cenário diferente do bloco de origem (para não decorar a letra) e gabarito distribuído entre A e E.
- Etiquetas: `tjpb`, `bloco::AAAA-MM-DD`, `formato::fgv`, `erro` ou `acerto`, `assunto::nome`. Sem duplicar cartões (conferir com `canAddNotes`).
- Foco: erros e acertos por chute; um cartão por regra 📌. Nunca apagar cartão que já tenha revisão (perde o histórico); se precisar trocar, perguntar antes.

Calcule a semana do plano pela data de hoje e use a seção 4.1 do `plano-tjpb.md` para saber o assunto.

---

## Obsidian (propriedades obrigatórias)

A pasta também é um vault do Obsidian. Os painéis leem as **propriedades** (frontmatter YAML) do topo de cada `.md`. Todo bloco, correção, simulado, discursiva, prova ou resumo novo começa com elas:

| Propriedade | Valores | Em quais arquivos |
|---|---|---|
| `tipo` | `bloco` · `correcao` · `simulado` · `discursiva` · `prova` · `resumo` | Todos |
| `fonte` | `autoral` · `oficial` | Bloco, correção, prova, simulado |
| `disciplina` | Lista com nomes **exatos** das notas de `disciplinas/` (ex.: `["Engenharia de Software e Ágil", "Português"]`) | Todos. Bloco misto lista todas as disciplinas cobradas |
| `assunto` | Texto curto | Todos |
| `semana` | Número da semana do plano | Bloco, correção, prova, simulado, discursiva |
| `data` | `AAAA-MM-DD` | Todos |
| `status` | `pendente` → `corrigido` | Só bloco. Ao corrigir, mudar só esta propriedade no bloco |
| `acertos` · `total` | Números | Correção, simulado, discursiva (nota/40) |
| `banca` · `prova` | Ex.: `FGV` · `"TRT-16 2022"` | Provas oficiais e simulados |
| `portugues` · `rlm` · `especificas` · `discursiva_nota` | Acertos por parte | Só simulado |
| `atualizado` | `AAAA-MM-DD` | Só resumo |

- Usar os modelos de `modelos/` como base. Datas sempre ISO na propriedade (no texto pode ser DD/MM).
- Resumo novo: acrescentar o link na seção "Material" da nota da disciplina.
- Links internos em wikilink (`[[nome-do-arquivo]]`). Não renomear nem mover arquivos fora do Obsidian sem avisar, porque quebra links.
- **Seção "📍 Hoje" do `00-HOME.md`:** no início de cada sessão, reescrever com data, semana, dias até a prova, tabela almoço/Bloco 1/Bloco 2/revisão (pelo plano e pelo contexto), pendências e a busca `query` da revisão espaçada (datas de `regras-tjpb.md` com ~1, 7 e 30 dias; se não houver regra nessas datas, usar a mais recente).

---

## Máquinas e contas GitHub

Estudo em dois PCs, cada um com uma conta GitHub diferente. Commits e pushes saem **sempre pela conta já logada na máquina**; nunca trocar de conta, mexer no `gh auth` ou alterar `git config` para "corrigir" o autor.

| Máquina | Sistema | Pasta do repositório | Conta GitHub |
|---|---|---|---|
| Casa | Linux | `/home/tiago/Documentos/TJPB - Project` | `tiagomarcosss` (dona do repositório) |
| Trabalho | Windows | `C:\Users\tiago.souza\tjpb-2026-estudos` | `Tiago-AHBT` (colaboradora com permissão de escrita) |
| Celular | claude.ai/code | — | conta conectada no app |

- Identificar a máquina pelo sistema/caminho da pasta. Antes do primeiro push da sessão, conferir a conta ativa com `gh auth status`; se não for a esperada na tabela, avisar e não fazer push.
- No Windows o `gh` fica em `C:\Program Files\GitHub CLI\gh.exe` (pode não estar no PATH do Bash).
- Como os dois PCs fazem push, **sempre** `git pull` antes de começar e antes de fazer push, para evitar conflito.
- Nada da empresa (identidade visual, documentos, projetos de trabalho) entra neste repositório. É uso pessoal.

---

## Fluxo de uma sessão

0. **Sincronizar:** esta pasta é o repositório GitHub `tiagomarcosss/tjpb-2026-estudos` (uso nos dois PCs e no celular via claude.ai/code). No início, `git pull`; ao final de cada sessão que alterar arquivos, `git add -A`, commit com mensagem curta (ex.: "Correção bloco 2026-10-26 + contexto/regras"), `git pull` de novo e `git push` com a conta da máquina (ver "Máquinas e contas GitHub").
1. **Ler** `contexto-tjpb.md` e `regras-tjpb.md`. Atualizar a seção "📍 Hoje" do `00-HOME.md`.
2. **Teoria (quando eu pedir):** explicar o assunto do dia em tabelas curtas, com as pegadinhas FGV e a regra destacada com 📌.
3. **Questões:** gerar o bloco e salvar em
   `QUESTÕES NÃO OFICIAIS/Provas/AAAA-MM-DD_Semana-XX_Bloco-XX_Assunto.md`
   - Se já existir arquivo com o mesmo nome, incrementar o número do bloco.
   - Terminar o arquivo com a tabela "Minhas respostas" (vazia).
4. **Respostas:** eu respondo no chat (formato `1-X, 2-X...`) ou anotando no Okular (arquivo `.okular` ao lado do `.md`, em `Provas/`).
5. **Correção:** salvar `..._CORRECAO.md` (e o `.pdf`) na subpasta `Correções/` da mesma pasta do bloco (com `acertos` e `total`), mudar o `status` do bloco para `corrigido` e resumir no chat.
6. **Atualizar automaticamente** `contexto-tjpb.md` e `regras-tjpb.md` (ver abaixo) e dizer em 2–3 linhas o que mudou.

---

## Padrão das questões

- Estilo FGV: enunciado contextualizado ("Sabe-se que...", "Considere verdadeira..."), preferencialmente em cenário do Judiciário, alternativas de (A) a (E), pegadinhas típicas da banca.
- Basear o formato em provas FGV reais de TI (TRT-16 2022, TJ-MS 2024, TJ-AP 2024, TJ-RR) quando possível.
- Cada questão com título `## Questão N`, alternativas separadas por linha em branco e `---` entre questões.
- Sempre avisar no topo: questões autorais no estilo FGV, não oficiais. Nunca apresentar como oficiais.
- **Nunca colocar o gabarito junto.** Nem no arquivo, nem no chat, até eu responder.
- Em todo bloco, pelo menos 30% das questões sobre os **pontos fracos** do contexto, mesmo fora do assunto da semana.
- Cobrar de tempos em tempos as regras antigas de `regras-tjpb.md` (revisão espaçada: ~1, 7 e 30 dias após a data da regra), com outro cenário.
- Não repetir questões já feitas: conferir os blocos anteriores na pasta.
- Português de Analista: mais argumentação, inferência e organização textual do que gramática pura.
- Incluir 2–3 questões de leitura de código por semana (ponto fraco do TJ-RR).
- **Compatibilidade com o Okular** (que converte "(C)" em "©" e "I." em lista "a."): no `.md` do bloco, escrever a alternativa C como `\(C)` e o item romano I como `I\.`. O Obsidian mostra normalmente.

## Padrão da correção

- Tabela-resumo: questão · minha resposta · gabarito · ✅/❌ · placar.
- Para cada questão, **inclusive nas que acertei**: repetir a questão inteira (enunciado completo, itens I/II/III quando houver e **todas** as alternativas de A a E), marcar ❌ a minha e ✅ a certa. Nunca mostrar só a alternativa correta.
- Nos erros: explicar onde provavelmente me confundi (usar minhas anotações, se houver) e destacar a regra com 📌.
- Nos acertos: 1–2 linhas confirmando (por que as outras alternativas estão erradas) e a regra 📌.
- **Correção de prova ou bloco sempre é entregue em PDF** (mesmo nome do `.md`, extensão `.pdf`, na pasta `Correções/`). O PDF é o arquivo que eu leio. O `.md` continua existindo só como base do PDF e dos painéis do Obsidian (propriedades `acertos`/`total`). Todo o resto (resumos, contexto, regras, blocos de questões) pode ficar só em `.md`.
- **Quando eu mandar um PDF para analisar** (prova oficial, lista de questões, bloco anotado), a correção vira **outro PDF**, no mesmo padrão, sem alterar o PDF original: `..._CORRECAO.pdf` (ou `_CORRECAO_vN.pdf`) em `Correções/`, ao lado da pasta `Provas/` onde está o original.
- **Padrão visual do PDF** (referência: `QUESTÕES NÃO OFICIAIS/Correções/2026-10-23_Semana-01_Bloco-01_EngSoftware-UNIVESP-Aulas01a05_CORRECAO_v2.pdf`): A4, gerado de HTML pelo navegador em modo headless (Linux: `brave --headless --print-to-pdf`), título com versão, data e placar, aviso de questões autorais/oficiais, tabela-resumo (Questão · Assunto · Sua · Gabarito · Resultado com ✅/❌/em branco), faixas escuras por seção e cada questão completa com A–E, ✅ na certa e "← sua resposta" na minha. Não incluir o frontmatter YAML no PDF. Converter o `.md` com `markdown -f +fencedcode,+githubtags,-smarty,-alphalist` (discount), para não virar "©" nem lista "a.".
  - **No Windows (trabalho):** converter com `npx -y marked@15.0.12 --gfm -i arquivo.md -o arquivo.html` (não gera "©" nem lista "a.") e imprimir com o Chrome: `"C:\Program Files\Google\Chrome\Application\chrome.exe" --headless=new --disable-gpu --no-pdf-header-footer --print-to-pdf="<caminho>.pdf" "file:///<caminho>.html"`. Alternativa: Edge em `C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe`, com os mesmos parâmetros. Gerar o HTML intermediário no scratchpad, nunca dentro da pasta de estudos.
- Tabela "Para o caderno de erros": assunto · por que errei · regra certa.
- Fechar com "O que estudar agora", ligado à rotina do plano (almoço, Bloco 1 19h, Bloco 2 20h, revisão 22:40, simulado de domingo).
- Comparar com o resultado anterior do mesmo assunto, se houver.

---

## Atualização automática dos arquivos

Após cada correção, sem precisar eu pedir:

**`regras-tjpb.md`**
- Acrescentar cada regra nova no fim da seção certa, no formato `- [DD/MM] regra em uma linha`.
- Não duplicar: se a regra já existe, não repetir (pode reforçar a redação, mantendo a data original).

**`contexto-tjpb.md`**
- Atualizar a data e a semana no topo.
- Acrescentar a sessão no **Histórico semanal** (data · assunto · placar · acertos · erros).
- Reordenar **Pontos fracos**: subir o que errei de novo; remover o que acertei em 2 sessões seguidas (avisar no chat quando remover).
- Ajustar **Próximos passos**.
- Manter o arquivo com no máximo ~2 páginas. A partir da semana 6, resumir semanas antigas em 1 linha cada e manter detalhadas só as 3 últimas.

Se eu disser "sem atualizar", pular esta etapa.

## Simulados e discursivas

- **Simulado:** quando eu trouxer o placar, criar `simulados/AAAA-MM-DD_Prova-Banca-Ano.md` com placar por disciplina, erros e assuntos. Atualizar o contexto.
- **Discursiva:** eu salvo a foto em `discursivas/` (ex.: `2026-10-25_tema.jpg`). Corrigir em `discursivas/AAAA-MM-DD_tema_CORRECAO.md`: nota estimada de 0 a 40 (conteúdo técnico com maior peso + língua portuguesa), item a item, termos técnicos que faltaram e versão melhorada. Avisar que a nota é estimativa, pois o edital não detalha os critérios.

---

## Como ler anotações do Okular

O arquivo `.okular` é um ZIP com `metadata.xml`. As anotações a caneta (`annotation type="6"`, `<ink>`) têm coordenadas normalizadas (0–1) por página.

1. Extrair para o scratchpad (nunca dentro da pasta de estudos).
2. Renderizar os traços em PNG (Python + PIL, `python3 -I` no Linux ou `python -I` no Windows) e visualizar.
3. Priorizar as respostas escritas na tabela "Minhas respostas". Usar círculos, X e anotações no texto para entender o raciocínio.
4. Se alguma resposta estiver ambígua, perguntar antes de corrigir.

**Legenda das minhas marcas:** círculo na letra = resposta final · risco/X = alternativa eliminada · **pontinho ao lado da alternativa = candidata** (pode ser a certa, mas não tenho certeza; é meu método de eliminação, para não reler o que já descartei) · "?" = dúvida ou chute. Na correção, tratar resposta com pontinho como **acerto com dúvida** (não conta para tirar o assunto dos pontos fracos) e, se houver mais de uma candidata, dizer qual pista levaria à certa.

**PDF anotado direto (sem `.okular`):** o Okular também pode salvar as anotações dentro do próprio PDF (anotações `Ink`). No Windows, sem Python, renderizar com Node + `pdfjs-dist` + `@napi-rs/canvas` instalados no scratchpad (`annotationMode: ENABLE`).

---

## Regras gerais

- Não inventar dados (notas de corte, estatísticas, normas). Quando não tiver certeza, dizer e sugerir como confirmar.
- Não apagar nem sobrescrever arquivos sem avisar. Questões e correções antigas são histórico.
- **Domingo, após o simulado:** lembrar de subir `plano-tjpb.md`, `contexto-tjpb.md` e `regras-tjpb.md` no Project do app do Claude (substituindo os antigos), para eu estudar pelo celular.
- Se eu contar algo que fiz pelo celular (Project), registrar no contexto e nas regras.
