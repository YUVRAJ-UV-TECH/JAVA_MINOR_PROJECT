# JavaMinorProject - Guesser Game

## Introduction
Guesser Game is a simple Java-based console game where a Guesser selects a number, and multiple players attempt to guess it. An Umpire determines the winner(s) based on the closest match to the Guesser's number.

## Features
- Single Guesser selects a secret number.
- Multiple players attempt to guess the number.
- Umpire compares guesses and announces the winner(s).
- Option to replay the game.

## How to Play
1. The Guesser enters a secret number.
2. Each player enters their guessed number.
3. The Umpire evaluates the guesses and declares the winner(s).
4. Players are prompted to replay or exit the game.

## Code Structure
### 1. `Guesser` Class
Responsible for taking the secret number input from the Guesser.
```java
class Guesser {
    public int GuesserNumb() {
        Scanner scan = new Scanner(System.in);
        System.out.println("Guesser, kindly guess the number");
        return scan.nextInt();
    }
}
```

### 2. `Player` Class
Each player inputs a guessed number.
```java
class Player {
    public int PlayerNumb() {
        Scanner scan = new Scanner(System.in);
        return scan.nextInt();
    }
}
```

### 3. `Umpire` Class
Handles collecting numbers from the Guesser and Players, and compares them to declare the winner(s).
```java
class Umpire {
    public void Compare() {
        // Compares the numbers and announces the winner(s)
    }
}
```

### 4. `GuesserGame` (Main Class)
Controls the game flow and provides an option to replay the game.
```java
public class GuesserGame {
    public static void main(String[] args) {
        // Game loop and execution
    }
}
```

## Prerequisites
- Install [Java JDK](https://www.oracle.com/java/technologies/javase-downloads.html)
- Use any Java IDE (e.g., IntelliJ, Eclipse, VS Code) or run in the terminal.

## How to Run
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/JavaMinorProject.git
   ```
2. Navigate to the project directory:
   ```sh
   cd JavaMinorProject
   ```
3. Compile and run the Java program:
   ```sh
   javac GuesserGame.java
   java GuesserGame
   ```

## Future Enhancements
- Implement a graphical interface (GUI) using Java Swing or JavaFX.
- Allow dynamic player count selection.
- Add difficulty levels (easy, medium, hard).

## License
This project is open-source and available under the MIT License.

## Author
**Yuvraj Nagre** - Developer & Maintainer

