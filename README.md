# RockPaperScissorPython 

📘 Rock–Paper–Scissor Game – Code Explanation (Line-by-Line)

Below is the complete explanation of each line of the code, written in the same serial order as your program.
This explanation is suitable for GitHub README documentation.

1. import random** 

This line imports Python's built-in random module, which allows the program to generate random values.
In this project, the module is used to randomly select the computer's move.

2. item_list =["Rock,","Paper","Scissor"]

A list named item_list is created that contains all possible moves of the game: Rock, Paper, and Scissor.
The computer will later select one of these options randomly.
(Important: "Rock," contains a comma in the string — the move will be shown exactly as "Rock," when printed.)

3. user_choice = input("Enter your move = Rock,Paper,Scissor= ")

This line takes input from the user.
The user must manually type either Rock, Paper, or Scissor to play the game.

4. comp_choice = random.choice(item_list)

Using random.choice(), the computer selects one option randomly from the item_list.
This ensures every game round gives an unpredictable result.

5. print(f"User Choice = {user_choice}, Computer choice= {comp_choice}")

This prints both the user’s selected move and the computer’s randomly chosen move.
An f-string is used for clean and readable formatting.

6. if user_choice == comp_choice:

The first condition checks whether both the user and the computer selected the same move.
If both moves are identical, the game results in a tie.

7. elif user_choice =="Rock":

This condition checks whether the user selected Rock.
The next inner condition will determine the winner based on the computer’s move.

7.1 if comp_choice =="Paper":

If the computer selects Paper, then Paper covers Rock → Computer Wins.

7.2 else:

If the computer did not select Paper, it must be Scissor.
Rock smashes Scissor → User Wins.

8. elif user_choice =="Paper":

This block runs when the user selects Paper.

8.1 if comp_choice=="Scissor":

If the computer selects Scissor, then Scissor cuts Paper → Computer Wins.

8.2 else:

If the computer did not select Scissor, then it must be Rock.
Paper covers Rock → User Wins.

9. elif user_choice=="Scissor":

This block runs when the user selects Scissor.

9.1 if comp_choice=="Paper":

If the computer selects Paper, Scissor cuts Paper → User Wins.

9.2 else:

If the computer did not pick Paper, then it must be Rock.
Rock smashes Scissor → Computer Wins.

📌 Summary of Logic

✔ The game follows the classic Rock–Paper–Scissor rules

✔ The program compares the user’s choice with the computer’s random choice

✔ Using nested if-else statements, the winner is determined

✔ Tie → both choices same

✔ All remaining outcomes follow standard game rules
