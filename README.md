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

Type	Forte Contra	Fraco Contra	Resistente a	Vulnerável a
Normal		Rock, Ghost, Steel	Ghost	Fighting
Fighting	Normal, Rock, Steel, Ice, Dark	Flying, Poison, Psychic, Bug, Ghost, Fairy	Rock, Bug, Dark	Flying, Psychic, Fairy
Flying	Fighting, Bug, Grass	Rock, Steel, Electric	Fighting, Ground, Bug, Grass	Rock, Electric, Ice
Poison	Grass, Fairy	Poison, Ground, Rock, Ghost, Steel	Fighting, Poison, Grass, Fairy	Ground, Psychic
Ground	Poison, Rock, Steel, Fire, Electric	Flying, Bug, Grass	Poison, Rock, Electric	Water, Grass, Ice
Rock	Flying, Bug, Fire, Ice	Fighting, Ground, Steel	Normal, Flying, Poison, Fire	Fighting, Ground, Steel, Water, Grass
Bug	Grass, Psychic, Dark	Fighting, Flying, Poison, Ghost, Steel, Fire, Fairy	Fighting, Ground, Grass	Flying, Rock, Fire
Ghost	Ghost, Psychic	Normal, Dark	Normal, Fighting, Poison, Bug	Ghost, Dark
Steel	Rock, Ice, Fairy	Steel, Fire, Water, Electric	Normal, Flying, Poison, Rock, Bug, Steel, Grass, Psychic, Ice, Dragon, Fairy	Fighting, Ground, Fire
Fire	Bug, Steel, Grass, Ice	Rock, Fire, Water, Dragon	Bug, Steel, Fire, Grass, Ice	Ground, Rock, Water
Water	Ground, Rock, Fire	Water, Grass, Dragon	Steel, Fire, Water, Ice	Grass, Electric
Grass	Ground, Rock, Water	Flying, Poison, Bug, Steel, Fire, Grass, Dragon	Ground, Water, Grass, Electric	Flying, Poison, Bug, Fire, Ice
Electric	Flying, Water	Ground, Grass, Electric, Dragon	Flying, Steel, Electric	Ground
Psychic	Fighting, Poison	Steel, Psychic, Dark	Fighting, Psychic	Bug, Ghost, Dark
Ice	Flying, Ground, Grass, Dragon	Steel, Fire, Water, Ice	Ice	Fighting, Rock, Steel, Fire
Dragon	Dragon	Steel, Fairy	Fire, Water, Grass, Electric	Ice, Dragon, Fairy
Fairy	Fighting, Dragon, Dark	Poison, Steel, Fire	Fighting, Bug, Dragon, Dark	Poison, Steel
Dark	Ghost, Psychic	Fighting, Dark, Fairy	Ghost, Psychic, Dark	Fighting, Bug, Fairy


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
