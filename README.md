# Adventure Game Project
This is Project#2 for CS-515 subject
It's a text-based adventure game. Navigate through different sorts of rooms and play with items. Your choices shape the outcome in this captivating journey. 

## How to Play
1. Run the game with `python3 adventure.py [map filename]`.
2. Use commands like `go`, `look`, `get`, `inventory`, and `quit` to navigate and interact.

## Made By
- Shikhar Saxena (Stevens mail id: ssaxena10@stevens.edu)
- CWID: 20021187
## GitHub Repository
[Link to the Public GitHub Repo](https://github.com/Shikhar253/Project-2-Adventure)

## Project Hours
I estimate that I spent approximately 12 hours on this project.
## Code Testing
I tested our code by:
- Performing manual testing of various game scenarios, making various maps and running all possible commands on those maps 

## Known Bugs/Issues
- There are no bugs and issues in the code

## Issue Resolution
One issue I encountered was during imlementation of "help" verb extension. Earlier, I just hard coded the print statements and it wans't reflective of the functions. I had to manually add a command to help, everytime I wanted to implement it. 
I talked to professor and he hinted me about the way and so I implemented a reflective "help" verb functionality.


## Project Extensions
### Help Verb
- **Verb/Command**: help verb tells player what the valid verbs are.
- **How to Exercise**: Just type  "help"
- **Output:** 
```
You can run the following commands:
  drop [item]
  get [item]
  [direction] or go [direction]
  help
  inventory
  look
  quit
```
### "Drop" verb
- **Verb/Command**: The drop verb is the opposite of get: take something from your inventory and put it down in the room.
- **How to Exercise**: just write "drop [item]" wwhere item can be any item present in our inventory at that moment
- **Output**: If I write "drop rose": 
```
You drop the rose.
```
### Directions become verbs
- **Verb/Command**: one can use an exit as a verb. That is, simply typing east instead of go east
- **How to Exercise**: just write "[direction]" instead of go [direction] 
 
## Instructions to check functioning of extensions on the map provided 
Run the commands in the following order. Ignore the text inside square brackets 
- python3 adventure.py map.json
- get rose 
- west    [**Extension**:Directions become verbs ]
- inventory [*this will show you that you have the rose with you in the new room too* ]
- drop rose [**Extension**:Drop verb ]
- inventory [*this will show you that the rose is no more with you*]
- look [*this will show you that the rose is in the items list of the current room*]
- help  [**Extension**:Help verb]
- quit

