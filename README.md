# Trabalhando com condicionais no Typescript

```typescript
const pokemons = [
{
  name: "pikachu",
  types: ["eletric"]
},
{
  name: "gabite",
  types: ["dragon", "ground"]
},
]
```

Retorno:

```json
{
  name: "pikachu",
  types: ["eletric"],
  weakness: ["ground"]
}
```

## Objetivo

O objetivo é que você consiga verificar as fraquezas de cada pokemon, por exemplo:
A fraqueza de pikachu é tipo elétrico, logo sua fraqueza é ground e será listada essa fraqueza, outras também, caso tenham.

## Recursos

Você pode seguir a matriz abaixo:

[![matriz pokemon]([https://upload.wikimedia.org/wikipedia/commons/thumb/9/97/Pokemon_Type_Chart.svg/2048px-Pokemon_Type_Chart.svg.png](https://i.redd.it/y1otlvy1p67e1.jpeg))]([https://upload.wikimedia.org/wikipedia/commons/thumb/9/97/Pokemon_Type_Chart.svg/2048px-Pokemon_Type_Chart.svg.png](https://i.redd.it/y1otlvy1p67e1.jpeg))

Nesse exercicio podemos usar as condicionais. Importante também utilizar tipos e objetos.

<https://www.typescriptlang.org/docs/handbook/2/objects.html>

Você vai receber o tipo do pokemon e retornar suas fraquezas.
Lembrando que um pokemon pode ter mais de um tipo.

## Critérios de Aceite

- Pokemon pode ter dois tipos e suas fraquezas serão listadas, mesmo que ele tenha algum tipo que anule alguma fraqueza, pode listar todas (essa lógica não é tão necessária).
- Ter uma tela onde eu possa filtrar por alguma das informações
- Cada pokemon deve ter um identificador unico, seja pelo nome ou ID
- Deve ser feito endpoints do backend e conexão com frontend

### Backend

Precisa ser next? Não necessariamente, mas eu aconselharia vocês a usarem, já que como não é um exercício complexo, vocês podem focar em aprender o next para o backend.

### Frontend

Precisa ter next? Não também, mas mesmo conselho que acima.
Posso usar bibliotecas? Sim, vocês podem usar material-ui, tailwind, etc.. A ideia do front é vocês terem a liberdade criativa de vocês. Ou seja, usem lógica no backend o máximo que puderem, pra deixar bem tranquilo pra na hora do frontend vocês terem essa liberdade.
Cada uma pode fazer uma UI diferente, a questão aqui é vocês explorarem as tecnologias.

> Podem fazer tela para cada pokemon, lista de pokemons, lista de tipos de pokemons, barra de pesquisa, vocês são livres para isso. Contudo que no exercício vocês contem TODAS as fraquezas do pokemon, mesmo se ele tiver mais de um tipo.

## Tecnologias

- Axios ou Fetch
- React
- Next para front (opcional)
- Next para backend (opcional)

Boa sorte!
