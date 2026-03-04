# OOP_basic_design_worksheet

## Before you write any code, clone and run the project to ensure your computer is set-up correctly

## Instructions (Read all before writing code)

Practice your new found skills in Single responsibility & encapsulation.

You are to write a simple "game" where you move a circle "Player" around the scene using the cursor keys. The circle should not leave the playarea (screen).

Your game will need at least 4 classes for 4 different responsibilities. **Before coding** draw the four classes and their relationships in UML: 

- [ ] Player class: responsibility of knowing how the player moves in the world (including keeping player on screen)

- [ ] PlayerRender class:  responsibility of drawing player at correct location on screen

- [ ] PlayerController class:  responsibility of converting keyboard input into Player movement instructions

- [ ] Boundary class:  responsibility of _constraining_ a point is inside a rectangle representing the playarea

### Notes

- The player class should not have *any* SFML dependencies, at all **(no `sf::` anywhere in Player**)!
- Write all the classes in the same file as main()
- No class is allowed to have a setter method (use the constructor)
- limit the getters as much as possible - (but you will probabaly need to use one or two)
- Use "Tell, don't ask" principle
- Watch out for Demeter violations
- It's ok for classes to contain other classes, but you don't have to.
- Put all decisions (`if` statements) in the class that has the responsibility of that decision
- PlayerRenderer will need some position information from Player — think carefully about the minimum it needs to know.

## [Optional] Advanced Step (if you've completed the 4 classes)

Your implementation of PlayerRenderer probably calles a getter on Player. Can you redesign this so PlayerRenderer has zero getters to call on Player?

If you are struggling with this, consider — the Visitor / double-dispatch pattern.


## Submission

Upload the `.cpp` file to the assignment on BB
