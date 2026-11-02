---
tipo: disciplina
disciplina: "Discursiva"
tags: [disciplina]
---

# Discursiva

**Quando:** Todo domingo, junto com o simulado · **Peso:** Discursiva · 40 pontos · meta 30+ · **mínimo 24 (60%)**

**Formato (2ª retificação, 29/10/2026):** 1 **estudo de caso** sobre Conhecimentos Específicos do cargo, até 30 linhas. A resposta precisa ter análise crítica do contexto, identificação dos problemas, conhecimentos teóricos **e normativos** e proposta de solução. Nota zero se fugir do formato, do tema ou se o conteúdo técnico estiver plenamente incorreto. Detalhes: [[plano-tjpb]], seção 7 · [[2026-10-29_2a-retificacao-edital-TJPB]].

Voltar: [[00-HOME]] · Conteúdo detalhado: [[plano-tjpb]], seção 4.1

## Material

- Fotos e correções: pasta `discursivas/`

## Desempenho e arquivos

Tudo o que tiver `disciplina` igual a esta nota (blocos, correções, simulados, resumos):

```base
formulas:
  aproveitamento: 'if(total, (acertos / total * 100).round() + "%", "")'
properties:
  formula.aproveitamento:
    displayName: Aproveitamento
filters:
  and:
    - '!file.inFolder("modelos")'
    - 'disciplina.contains("Discursiva")'
    - 'tipo != "disciplina"'
views:
  - type: table
    name: Histórico
    order:
      - note.data
      - note.tipo
      - note.assunto
      - note.acertos
      - note.total
      - formula.aproveitamento
      - file.name
    sort:
      - property: note.data
        direction: DESC
```
