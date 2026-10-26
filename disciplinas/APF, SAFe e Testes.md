---
tipo: disciplina
disciplina: "APF, SAFe e Testes"
tags: [disciplina]
---

# APF, SAFe e Testes

**Quando:** Semana 2 (02–08/11) · **Peso:** Conhecimentos Específicos

Voltar: [[00-HOME]] · Conteúdo detalhado: [[plano-tjpb]], seção 4.1

## Material

- Regras estudadas: [[regras-tjpb#APF, SAFe e Testes]]

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
    - 'disciplina.contains("APF, SAFe e Testes")'
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
