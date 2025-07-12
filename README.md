# Snake-Gmae
<h2>Control a snake that moves around the screen, eats food to grow longer, and avoids hitting walls or itself. <br>
  The game keeps track of the score and stores the high score persistently in a file (data.txt).
</h2>
<h3>Project Structure</h3>
<ul>
  <li>The project is well-organized into multiple Python files:
  <ul>
    <li>main.py – main game logic</li>
    <li>snake.py – snake behavior</li>
    <li>food.py – food generation</li>
    <li>scoreboard.py – score management</li>
  </li>
</ul>
<h3>📜 main.py – Game Controller</h3>
<ul>
  <li>Functions:
    <ul>
      <li>Initializes the screen.</li>
      <li>Creates instances of Snake, Food, and Scoreboard.</li>
      <li>Runs the game loop:
        <ul>
          <li>Moves the snake.</li>
          <li>Detects collision with food.</li>
          <li>Detects collision with wall or tail.</li>
          <li>Triggers game reset and score update when needed.</li>
        </ul>
      </li>
    </ul>
  </li>
</ul>
<h3>🐍 snake.py – Snake Class</h3>
<ul>
  <li>Features:
    <ul>
      <li>Manages the snake's body segments (Turtle objects).</li>
      <li>ontrols direction with up(), down(), left(), and right() methods.</li>
      <li>Resets the snake after collision.</li>
    </ul>
  </li>
</ul>
<h3>🍎 food.py – Food Class</h3>
<ul>
  <li>Features:
  <ul>
    <li>Randomly generates food positions within bounds.</li>
    <li>Uses refresh() to reposition the food after being eaten.</li>
  </ul>
  </li>
</ul>
<h3>🧮 scoreboard.py – Scoreboard Class</h3>
<ul>
  <li>Features:
  <ul>
    <li>Displays current score and high score.</li>
    <li>Updates score on eating food (increase_score()).</li>
    <li>Stores high score in a file (data.txt).</li>
  </ul>
  </li>
</ul>
<h3>💾 data.txt</h3>
<ul>
  <li>Simple text file to persist high score between runs.</li>
</ul>


<h3>🧩 Modules Used</h3>
<ul>
  <li>✅ Built-in Modules:
  <ul>
    <li>time :To control snake speed with time.sleep(0.1)</li>
    <li>random :To randomly place food within the game screen</li>
  </ul>
  </li>
</ul>

<h3>🐢 turtle Module:</h3>
<ul>
  <li>Python's built-in graphics library for simple GUI/game projects.
  <ul>
    <li>Turtle() – Create game objects (snake, food, score)</li>
    <li>Screen() – Controls game screen</li>
    <li>screen.listen() – Detects user key presses</li>
    <li>screen.onkey() – Binds arrow keys to movement</li>
    <li>screen.tracer(0) – Manual control over screen updates</li>
    <li>screen.update() – Updates game frame</li>
    <li>turtle.goto(x, y) – Moves turtle to specific coordinates</li>
    <li>turtle.distance() – Calculates distance to another turtle (for collision detection)</li>
    <li>turtle.write() – Draws text (score)</li>
    <li>turtle.hideturtle() – Hides the turtle shape (used for the scoreboard)</li>
  </ul>
  </li>
</ul>
