## Viking board game

# play
  [tafl](http://tafl.herokuapp.com)

## Rules
 - can move horizontally or vertically as many steps
 - get the king(piece at center) to any one of the corner
 - to kill a piece surround it from 2 sides
 - aim of the swords or red team is to capture king

## Interesting ideas
 - may not be optimized but in the current version there is no 11x11 matrix, only thing that is being tracked are pieces nothing about white space
 - using leveldb as database, even for future autentication
 - first time thought of using a logger function that prints of all global variables, like a debugger
   - in future rather than making global variables make a global object and then the logger simply prints property and value of the global object
 - todo, refactoring, security markdown file for each project, helps me think and separates concern
 - 

## future changes
 - maybe for some optimizations a global board state with white spaces
 - try rxjs

## Todo
 - control panel
    - suggestions checkbox
    - versions of game like different board
- rules
- AI(single player mode)
- hover hightlight
- suggestions including different color for capturing
- start new game
- save game state

## Events
 - client ==> server ==> other client , client ==> server <== other client, client <==> server <==> other client
 - connection ==> server
 - my-room ==> server

## Databse Todo
 - add count of players to each room 0,1,2 after its created
 - reduce count on disconnect
 - state of game, if after disconnect player reconnects sync happens
 - for the state an array can be used where move objects are put and resent to rejoint player
 - keep score in same room

## petty todo
 - decide either swords or sword
 - turn wise coloring or cursor change
