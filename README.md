# Rock Paper Scissors Game

# Introduction:
Welcome to the Rock Paper Scissors Game! This is a simple command-line game where you can play Rock, Paper, Scissors against the computer.
The game continues until you decide to quit.

# Installation:
1.Clone the repository:
git clone https://github.com/your-username/rock-paper-scissors.git
2.Navigate to the project directory:
cd rock-paper-scissors
3.Set up the environment:
Ensure you have Python installed on your system

# Usage:
1.Run the game
2.Follow the on-screen instructions to play the game:
Choose "Rock", "Paper", or "Scissors".
Type "quit" or "exit" to end the game.

# Game Rules:
1.Rock beats Scissors
2.Scissors beats Paper
3.Paper beats Rock
4.If both choices are the same, it is a tie.

# Features:
1.Simple command-line interface.
2.Randomized computer choices.
3.Continuous play until the user decides to quit.

# Example:
import random

print("\nLet's play Rock-Paper-Scissors!")
choices = ["rock", "paper", "scissors"]

while True:
    user_choice = input("Choose Rock, Paper, or Scissors (or type 'quit' to exit): ").strip().lower()
    if user_choice == "quit" or user_choice == "exit":
        print("Thanks for playing! Goodbye!")
        break

    if user_choice in choices:
        computer_choice = random.choice(choices)
        print(f"Your choice: {user_choice.capitalize()}")
        print(f"Computer's choice: {computer_choice.capitalize()}")

        if user_choice == computer_choice:
            print("It's a tie!")
        elif (
            (user_choice == "rock" and computer_choice == "scissors") or
            (user_choice == "paper" and computer_choice == "rock") or
            (user_choice == "scissors" and computer_choice == "paper")
        ):
            print("You win!")
        else:
            print("Computer wins!")
    else:
        print("Invalid choice. Please choose Rock, Paper, or Scissors or type 'quit' to exit.")

# output:
Let's play Rock-Paper-Scissors!
Choose Rock, Paper, or Scissors (or type 'quit' to exit): rock
Your choice: Rock
Computer's choice: Rock
It's a tie!Let's play Rock-Paper-Scissors!
Choose Rock, Paper, or Scissors (or type 'quit' to exit): rock
Your choice: Rock
Computer's choice: Rock
It's a tie!
Choose Rock, Paper, or Scissors (or type 'quit' to exit): paper
Your choice: Paper
Computer's choice: Scissors
Computer wins!
Choose Rock, Paper, or Scissors (or type 'quit' to exit): scissors
Your choice: Scissors
Computer's choice: Paper
You win!
Choose Rock, Paper, or Scissors (or type 'quit' to exit): quit
Thanks for playing! Goodbye!
Choose Rock, Paper, or Scissors (or type 'quit' to exit): paper
Your choice: Paper
Computer's choice: Scissors
Computer wins!
Choose Rock, Paper, or Scissors (or type 'quit' to exit): scissors
Your choice: Scissors
Computer's choice: Paper
You win!
Choose Rock, Paper, or Scissors (or type 'quit' to exit): quit
Thanks for playing! Goodbye!







