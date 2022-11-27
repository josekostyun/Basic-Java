# Basic-Java
A board game that requires two players to move a knight piece 1 square diagonally first player to reach bottom right square of board wins. 

### Project ### 

We are going to play a fun strategy game that only requires two players! In this game, we have an 8 x 8 board and a Knight chess piece that starts on the top left of the board. Each player gets to move the Knight piece one square over either down, diagonal, or to the right of its current position (a player cannot move the piece two or more squares). The Knight piece can keep moving until it reaches the bottom right corner of the board. The respective player that moves the Knight to the bottom right corner of the board wins the game! In this assignment you are going to implement the winning strategy for both players.

**Requirements**
1. You will create a public class called Game.
2. The Game Class will have the following attributes:
   * 2D integer array that symbolizes the board.
   * 1D primitive char array (not a String object) that will store computerize moves. There is no need to use the Random Class. Hint: This should be used in one of the
hypothetical strategies for one of the players to always win.
3. The Game Class has a constructor that takes two parameters
   * A primitive integer that represents the size of board (assume the board is always a square)
   * A String object reference that contains the name of a file that keeps the moves the player 2 will use in the game.
4. The Game Class has a public non static method called readMoves. readMoves will scan the respective text files of moves and store them in the character array attribute. The characters ‘r’, ‘b’, and ‘d’ represent the moves.
   * ‘r’ means move to the right one square
   * ‘b’ means move down one square
   * ‘d’ means move diagonal one square
   
   The method has one String reference parameter that represents the name of the text file. 
   This method should be invoked when the object of the class is instantiated.

5. The Game class has a public non static method called play. play will simulate a round of the game. The method has one parameter that represents the player you want to win the game. If a one is passed, then player 1 must win. If a two is passed, then player 2 must win. The method returns an integer type value that represents the winner of the game (1 being player 1 and 2 being player 2). You can assume that player 1 will always go first in the game, however based on the value past, you need to determine the appropriate strategy for always winning the game for the appropriate player. This also includes what the other player must do in their respective move.
6. You are allowed to create helper methods as long as they are not called directly from the driver file. The helper methods must be called from your solution file.

A driver file (GameDriver.java) has been provided for you to show you how the methods are called along with 10 test cases to see if you get the same scenario result.
