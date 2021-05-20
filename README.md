# Snake-Game
Creating a snake game using Python

main.py holds all the game logic:
  1. Setting up the screen and keyboard commands to allow player to move
  2. Setting up the game and keeping the game going as long as there is no collision or player ending the game
  3. Checking for collision with food
  4. Checking for collision with the wall
  5. Checking for collision with the tail

snake.py creates each segment of the snake as a separate turtle class and establish the head as the first position in the list of segments. 
It adds a snake segment to the end of the snake segment through the add_segment function which is called through the extend function. 
THe move function loops through the segments to move them at a default move speed.
A heading function is set up for each direction which is attached to keyboard buttons in the main.py file. 
When the game resets it sends the current snake segments off screen to remove them.

food.py establishes the food class attributes and moves it around the screen when the snake collides with it.

scoreboard.py writes the score at the top of the screen. When the player collides with food the score increases by one. 
If the player dies with a current score that is greater than the high score the scoreboard will write to a data file updating the high score.
When the game is restarted the scoreboard will read the data file and present the current high score. 
  
