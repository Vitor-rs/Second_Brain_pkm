---
id: zettelkasten
title: Zettelkasten
desc: 'Sistema de notas interconectadas'
created: 2023-07-01
---

# Zettelkasten

Esta seção implementa a metodologia Zettelkasten para criar um sistema de notas interconectadas e evolutivas.

## O que é Zettelkasten?

Zettelkasten é:
- Um sistema de tomada de notas desenvolvido por Niklas Luhmann
- Baseado em notas atômicas e interconectadas
- Projetado para facilitar conexões não óbvias entre ideias

## Tipos de Notas

### Notas Passageiras (Fleeting Notes)
- [[fleeting]] - Notas rápidas e temporárias que serão processadas posteriormente

### Notas de Literatura (Literature Notes)
- [[literature]] - Notas baseadas em fontes externas (livros, artigos, palestras)

### Notas Permanentes (Permanent Notes)
- [[permanent]] - Notas refinadas e permanentes com ideias claramente expressas

## Como usar o Zettelkasten

1. Capture ideias iniciais como Notas Passageiras (Fleeting Notes)
2. Ao consumir conteúdo, crie Notas de Literatura (Literature Notes)
3. Refine e processe essas notas em Notas Permanentes (Permanent Notes)
4. Estabeleça conexões entre notas usando links [[nota-relacionada]]
5. Adicione tags para facilitar agrupamentos temáticos

## Template para Notas Permanentes (Zettel)

```markdown
---
id: permanent.[timestamp]
title: [Título conciso da ideia]
desc: '[Uma frase explicativa]'
created: [Data]
tags: [tags relevantes]
---

# [Título conciso da ideia]

[Explicação clara e concisa de uma única ideia]

## Conexões
- [[Link para nota relacionada 1]] - [Explicação breve da relação]
- [[Link para nota relacionada 2]] - [Explicação breve da relação]

## Referências
- [Referência 1]
- [Referência 2]

## Contexto
[Contexto opcional em que esta ideia surgiu]
```
