#3 Java Class : SnakeGame (main class)
               GamePanel 
               GameFrame
               
1. SnakeGame -> Contains the 'main' functions. Calls GameFrame class by creating it's object.
2. GameFrame -> Initializes a GamePanel Object. Extends 'JFrame', helps in creating a window to run the game, specify attricutes such as title, window visiability etc.
3. GamePanel -> 
             The main logic of the game is implemented in the GamePanel class, which extends the JPanel class and implements the ActionListener interface.
             The GamePanel class contains several fields that hold the state of the game, such as the current direction of the snake, the position of the apple,
             the number of body parts of the snake, and the number of apples eaten.
             
             The paintComponent method is responsible for rendering the game on the screen. It first calls the draw method to draw the apple and the snake on the screen,
             and then displays the current score on the screen using the drawString method.
             
             The move method is called every time the timer ticks, and it updates the position of the snake based on its current direction. The checkApple method checks
             if the snake's head is at the same position as the apple, and if so, it increases the number of body parts and randomly places a new apple on the screen.
             
             The checkCollisions method checks if the snake collides with itself or the edges of the grid, and if so, it stops the game.
             
             The MyKeyAdapter class extends the KeyAdapter class and overrides the keyPressed method to handle the player's keyboard input. It changes the direction
             of the snake based on the arrow keys pressed by the player.
             
             The startGame method initializes the game state and starts the timer that controls the game loop. The gameOver method is called when the game is over, 
             and it displays a message on the screen with the final score.
             
             Overall, this code provides a good starting point for implementing a simple game using Java Swing. However, it can be improved in several ways,
             such as adding sound effects, implementing different game modes, or improving the graphic
