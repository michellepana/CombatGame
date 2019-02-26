# CombatGame
A one-user-two-player combat game made with C++


How to compile

There is a “makefile” included. 
To compile, navigate into this folder in the console, and type “make”.

Game Flow

This game is a one-user-two-player game. User will be able to select different types of fighters for 2 teams. After this, the game will go on by itself.

There are five different types of fighters, each with their own special ability:
1.	Vampire – may charm the opponent into NOT attacking
2.	Barbarian – no special ability
3.	Blue Men – very strong. But defense ability will decrease as HP drps
4.	Medusa – may kill the opponent instantly
5.	Harry Potter – may come back to life with doubled strength

Once all fighters for the 2 teams are selected, the ones queued at the front of the team will fight each other. The winner will be placed to be at the back of the team queue, heal some HP, and win the team 2 points. The loser will be removed from their team, added to the top of the Loser team, and cost their team 1 point.

At the end of a game, user may choose to play again, or exit the program.

Design

The CharQueue Class will be a queue implemented with doubly linked lists. It will be composed of CharNodes. In each CharNode, there will be a pointer to the Character class, which serves as the base abstract class for the Barbarian, the BlueMen, the HarryPotter, the Medusa and the Vampire classes.
