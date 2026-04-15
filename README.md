# Trabalhando com condicionais no TypeScript

## Descrição

Neste exercício, você irá implementar uma lógica para descobrir as **fraquezas de um Pokémon** com base em seus tipos.

A ideia é praticar:

- Condicionais
- Estrutura de dados
- Tipagem com TypeScript
- Manipulação de arrays e objetos

---

## Entrada

```ts
const pokemons = [
  {
    name: "pikachu",
    types: ["electric"]
  },
  {
    name: "gabite",
    types: ["dragon", "ground"]
  }
]
```
## Saída esperada
```ts
{
  "name": "pikachu",
  "types": ["electric"],
  "weakness": ["ground"]
}
```
---
## Objetivo

Você deve criar uma lógica que:

- Receba um Pokémon com um ou dois tipos
- Identifique suas fraquezas com base na tabela de tipos
- Retorne essas fraquezas

---
## Regras
- Um Pokémon pode ter um ou dois tipos
- As fraquezas devem ser acumuladas
- Não é necessário tratar casos complexos como imunidades ou cancelamento de fraquezas
- Pode haver fraquezas repetidas (não precisa remover duplicadas)

---
## Recursos

Use a tabela abaixo como referência:

| Type     | Forte Contra                        | Fraco Contra                                        | Resistente a                                                         | Imune a          | Vulnerável a                          |
| -------- | ----------------------------------- | --------------------------------------------------- | -------------------------------------------------------------------- | ---------------- | ------------------------------------- |
| Normal   |                                     | Rock, Steel                                         |                                                                      | Ghost            | Fighting                              |
| Fighting | Normal, Rock, Steel, Ice, Dark      | Flying, Poison, Psychic, Bug, Fairy                 | Rock, Bug, Dark                                                      |                  | Flying, Psychic, Fairy                |
| Flying   | Fighting, Bug, Grass                | Rock, Steel, Electric                               | Fighting, Bug, Grass                                                 | Ground           | Rock, Electric, Ice                   |
| Poison   | Grass, Fairy                        | Poison, Ground, Rock, Ghost                         | Fighting, Poison, Grass, Fairy                                       |                  | Ground, Psychic                       |
| Ground   | Poison, Rock, Steel, Fire, Electric | Bug, Grass                                          | Poison, Rock                                                         | Electric         | Water, Grass, Ice                     |
| Rock     | Flying, Bug, Fire, Ice              | Fighting, Ground, Steel                             | Normal, Flying, Poison, Fire                                         |                  | Fighting, Ground, Steel, Water, Grass |
| Bug      | Grass, Psychic, Dark                | Fighting, Flying, Poison, Ghost, Steel, Fire, Fairy | Fighting, Ground, Grass                                              |                  | Flying, Rock, Fire                    |
| Ghost    | Ghost, Psychic                      | Dark                                                | Poison, Bug                                                          | Normal, Fighting | Ghost, Dark                           |
| Steel    | Rock, Ice, Fairy                    | Steel, Fire, Water, Electric                        | Normal, Flying, Rock, Bug, Steel, Grass, Psychic, Ice, Dragon, Fairy | Poison           | Fighting, Ground, Fire                |
| Fire     | Bug, Steel, Grass, Ice              | Rock, Fire, Water, Dragon                           | Bug, Steel, Fire, Grass, Ice, Fairy                                  |                  | Ground, Rock, Water                   |
| Water    | Ground, Rock, Fire                  | Water, Grass, Dragon                                | Steel, Fire, Water, Ice                                              |                  | Grass, Electric                       |
| Grass    | Ground, Rock, Water                 | Flying, Poison, Bug, Steel, Fire, Grass, Dragon     | Water, Grass, Electric, Ground                                       |                  | Flying, Poison, Bug, Fire, Ice        |
| Electric | Flying, Water                       | Grass, Electric, Dragon                             | Flying, Steel, Electric                                              |                  | Ground                                |
| Psychic  | Fighting, Poison                    | Steel, Psychic                                      | Fighting, Psychic                                                    |                  | Bug, Ghost, Dark                      |
| Ice      | Flying, Ground, Grass, Dragon       | Steel, Fire, Water, Ice                             | Ice                                                                  |                  | Fighting, Rock, Steel, Fire           |
| Dragon   | Dragon                              | Steel                                               | Fire, Water, Grass, Electric                                         |                  | Ice, Dragon, Fairy                    |
| Fairy    | Fighting, Dragon, Dark              | Poison, Steel, Fire                                 | Fighting, Bug, Dark                                                  | Dragon           | Poison, Steel                         |
| Dark     | Ghost, Psychic                      | Fighting, Dark, Fairy                               | Ghost, Dark                                                          | Psychic          | Fighting, Bug, Fairy                  |


---

## Requisitos
### Backend
Criar uma função ou endpoint que:
- Receba um Pokémon
- Retorne suas fraquezas

### Frontend

Criar uma interface simples para:

- Listar Pokémon
- Visualizar suas fraquezas
- Filtrar ou buscar Pokémon

---
## Critérios de Aceite
- Suporte a Pokémon com 1 ou 2 tipos
- Retorno correto das fraquezas
- Cada Pokémon possui identificador único
- Backend funcionando
- Integração com frontend (opcional, mas desejavel)
- Interface com busca ou filtro (opcional, mas desejavel)

Cada uma pode fazer uma UI diferente, a questão aqui é vocês explorarem as tecnologias.

---
## Tecnologias sugeridas
- TypeScript
- React
- Next.js (opcional)
- Fetch ou Axios

---
## Dicas
- Evite usar muitos if — tente usar objetos/mapas
- Organize bem os dados antes de começar
- Resolva a lógica antes de pensar na interface

---

Referência

https://www.typescriptlang.org/docs/handbook/2/objects.html

---
Boa sorte!
