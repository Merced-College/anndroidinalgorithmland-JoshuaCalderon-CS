[![Open in Codespaces](https://classroom.github.com/assets/launch-codespace-2972f46106e565e64193e422d61a12cf1da4916b45550586e14ef0a7c637dd04.svg)](https://classroom.github.com/open-in-codespaces?assignment_repo_id=23091959)
# AnnDroidInAlgotihmLand
a sample project to practice sorting and searching

🎵 Download Required Audio File

This project uses an audio file that is too large to store directly in the GitHub repository.
Please download the file from Google Drive before running the program.

Download the audio file here:

➡️ Download the required audio file from Google Drive

Instructions

Open the Google Drive folder using the link above.

Download the ZIP file that contains the audio file.

Extract (unzip) the file on your computer.

Place the extracted audio file into the project folder named content.

Download all of the whole content folder, and put this in your project.

Examine the UML Diagram

## Code Exploration

### Step 1 — Project Structure
1. The `src` folder contains all the Java source code files like `Main.java`, `AppRouter.java`, `MainMenuPanel.java`, and `Assets.java`.
2. The `content` folder contains game assets such as images (`.png`) and audio files (`.wav`).
3. The `uml` folder contains UML diagrams showing class relationships, inheritance, and interactions.
4. Code is separated from content/assets so the program logic stays organized and assets can be updated without touching the code.

### Step 2 — Main Program
1. The class containing main() is `Main.java` in the `level1` package.
2. At startup, main() runs on the Swing event thread, creates the JFrame, sets up frame properties, creates an `AppRouter` object, and finally makes the frame visible.
3. Objects/classes created at start: `JFrame`, `AppRouter`, `Assets`.

### Step 3 — Program Execution
1. The class responsible for drawing graphics is `MainMenuPanel` (and other panels extending `JPanel`).
2. The class responsible for loading files and content is `Assets.java`.
3. The game updates the screen by refreshing panels when game state changes. `AppRouter` manages which panel is visible.
4. Player actions are handled by panels using key and mouse listeners that update player/game objects.

### Step 4 — UML Diagram
1. The UML diagram shows how classes inherit from each other, interact, and the overall program structure.
2. The central class in the system is `AppRouter`.
3. Classes that interact with others: panels depend on `Assets` for images/audio, `AppRouter` manages all panels, and `Main` creates `AppRouter`.

### Step 5 — Score System
1. Scores are stored in the class that manages game state or player data, usually in an array or ArrayList.
2. Scores are stored as `int` or custom `Score` objects containing a player name and score.
3. Sorting should be implemented in the same class that stores the scores since it already manages the score data.
