# Snake_Game_Project
This Python code implements a classic Snake game using Pygame. Players control a snake to eat fruits, growing longer while avoiding collisions. The game features real-time scoring and a graphical interface.

Project Name: Snake Game 
Project Objective:
This code aims to implement a simple Snake game using the Pygame library in Python. The player controls a snake that moves around the game window, eating randomly spawned fruits to increase its length and score. The game continues until the snake collides with the window boundaries or itself.

Key Features:
1. User Input Handling: The game responds to arrow key inputs to change the snake's direction.
2. Snake Movement: The snake moves continuously in the specified direction.
3. Collision Detection: The game checks for collisions with window boundaries, the snake's body, and the fruit.
4. Score Tracking: The player's score is incremented when the snake eats a fruit, and it is continuously displayed on the screen.
5. Game Over Handling: The game ends when the snake collides, displaying the final score, and quits after a brief delay.

   
Advanced Features Used:
1. Pygame Library: The code utilizes the Pygame library for handling game development aspects such as graphics and input.
2. Game Loop: A continuous game loop ensures ongoing updates, allowing for real-time gameplay.
3. Collision Detection: The code implements collision detection for various scenarios, including fruit consumption and self-collision.
4. Score Display: The game continuously displays the player's score on the screen.
5. Random Fruit Spawn: Fruits are spawned at random positions when consumed by the snake.

   
Submission:
To submit the game, you could provide the source code along with any necessary instructions on how to run the game. If applicable, include any external dependencies or libraries needed for execution. Additionally, you might include a README file with a brief description, controls, and other relevant information.

Testing:
Testing the game involves running it and ensuring that it performs as expected. Test cases should include checking for proper snake movement, collision detection, score updates, and game-over conditions. Verify that the game responds correctly to user input and that the displayed score accurately reflects the player's progress. Consider edge cases, such as testing the boundaries of the game window and the snake's collision with itself.

Code Breakdown:

Initialization:
Pygame is initialized, and the game window is set with a title.
Colors are defined for the snake, background, fruit, and text.

Game Variables:
snake_speed: Controls the speed of the snake.
window_x and window_y: Define the dimensions of the game window.
Snake and fruit positions, as well as the snake body, are initialized.
direction: Keeps track of the current direction the snake is moving.
change_to: Stores the direction to change, based on user input.
score: Keeps track of the player's score.

Main Game Loop:
The main game loop runs continuously, handling events and updating the game state.

Event Handling:
The code handles key events to change the direction of the snake.

Snake Movement:
The snake moves in the specified direction, and its position is updated.

Snake Growth:
If the snake collides with the fruit, the score is incremented, and a new fruit is spawned. The snake's body grows.

Drawing:
The game window is filled with a black color.
The snake's body and the fruit are drawn on the window.

Game Over Conditions:
If the snake collides with the window boundaries or its own body, the game_over() function is called.

Score Display:
The player's score is continuously displayed on the window.

FPS Control:
The frames per second (fps) are controlled to regulate the speed of the game.

Game Over Function:
Displays the player's final score, waits for 2 seconds, and then quits the game.

Update Display:
The game window is updated in each iteration.

FPS Tick:
The frames per second are controlled with the fps.tick(snake_speed) method.
