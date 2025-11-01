Project: zuul-bad
Authors: Michael Kölling and David J. Barnes

This project is part of the material for the book

   Objects First with Java - A Practical Introduction using BlueJ
   Seventh edition
   David J. Barnes and Michael Kölling

This project is a simple framework for an adventure game. In this version,
it has a few rooms and the ability for a player to walk between these rooms.
That's all.

To start this application, create an instance of class "Game" and call its
"play" method.

This version of the game contains some very bad class design. It should NOT
be used as a basis for extending the project without fixing these design
problems. It serves as an example to discuss good and bad design (chapter 8
of the book).

Chapter 8 of the book contains a detailed description of the problems in this
project, and how to fix them.

The project 'zuul-better' contains a version of this project with better
designed class structure. It includes the fixes discussed in the book.


PART 1: ZUUL-BAD
1.
This application lets the player explore different locations. 
The game takes the commands "go"(followed by the direction: north, south, east or west), "help" and "quit".
   -"go" command takes the player to another location depending on the direction; 
   -"help" command, when called, gives the player more info on the other commands, and the 
   -"quit" command makes the player terminate the game.
5 rooms
pub <-­> outside <->theater
         ^
         |
         v
        lab -> office
2. Parser: reads user input and interprets it as a command and returns it as an object of the Command class.
   Command:
3. A Knight tries to save a Princess from an evil Witch.
9. It "Returns a Set view of the keys contained in this map."(from the documentation).
13.
17. No, because if you already added the new command to the validCommands array, the showAll method takes it into consideration, so the Game class doesn't need to be changed.
18. I think using a static method might make the code clearer and quicker to write(since you wouldn't have to create an instance of the class and could simply tie the method directly to the class). But, I think a con would be that there are more limits to what you can do with a static method(?).
