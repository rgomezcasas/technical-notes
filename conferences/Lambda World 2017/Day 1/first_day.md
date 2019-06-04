# LAMBDA WORLD 2017

## Keywords
- Puretest library: declarative tests

## Typelevel unconference

### Juanma talk about spark
- Same as the one he did in scalabcn
- How to abstract data transformation DSL
- Problem with classtags

### Talk about haskell
- Use deriving to have instant access to type classes
  provided by the compiler directly.
- Examples: Show, toJSON, fromJSON with 0 lines of code

### Javier Fuentes - Testing purely functional programs
- One generic test for all implementations
- Context:
  - Tic tac toe
  - Tagless final
    - transformers: placeStone, resetBoard
    - observers: stoneIn, hasWon, activeTurn
  - Errors DSL: OccupiedPosition, NotInTheBoard, WrongTurn, etc
- Test -> StateT[Either, BoardState, A]
- Non-Declarative Tests
  - As we had in poker
  - Hard because you have to deal with the runF and check either states and stuff
- Declarative tests
  - Your test extends from FunStuite[P], type parameters at the test level
  - `trait TicTacToeSpec[P[_]] extends FunSpec[P]`
  - Your test now returns a P[Boolean] -> library handles the rest
  - Can also fail with errors -> there's DSL for it, you only see DOMAIN!!!
- Instantiate Tests
  - Then you have the implementation of the test, concrete with StateT or whatever
  - Must provide Tester[P] and MonadError[P], that's it!
- https://github.com/hablapps/puretest

## Category Theory from the very beginning - Rúnar Bjarnason
- 
