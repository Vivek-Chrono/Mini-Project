# Mini-Project

#code
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        // MINI PROJECT

        Scanner sc = new Scanner(System.in);

        int myNumber = (int) (Math.random() * 100);
        int userNumber = 0;

        do {
            System.out.println("Guess my number: ");
            userNumber = sc.nextInt();

            if (userNumber == myNumber) {
                System.out.println("WOOHOO CORRECT NUMBER!!!");
                break;
            } else if (userNumber > myNumber) {
                System.out.println("Your number is too large");
            } else {
                System.out.println("Your number is too small");
            }

        } while (userNumber >= 0);

        System.out.print("My number was: ");
        System.out.println(myNumber);

        sc.close();
    }
}

#Output
![image](https://github.com/user-attachments/assets/c761481d-d3e5-44ed-82a2-cb1fbb977fbc)

#Number Guessing Game in Java

This project is a simple console-based number-guessing game implemented in Java. The program randomly generates a number between 0 and 99, and the player has to guess the correct number. The game provides feedback on whether the guessed number is too high, too low, or correct.

Features:
Random Number Generation: The program generates a random number between 0 and 99 each time it runs.

User Input: Players input their guesses, and the program responds with hints until the correct number is guessed.

Exit Option: Players can exit the game at any time by entering a negative number.

Loop Control: The game continues until the correct number is guessed or the player decides to exit.

How to Play:

Run the program.
Guess the number by entering a value between 0 and 99.
The program will indicate if your guess is too high, too low, or correct.
If you want to exit the game, simply enter a negative number.
After guessing correctly or exiting, the program will reveal the randomly generated number.
