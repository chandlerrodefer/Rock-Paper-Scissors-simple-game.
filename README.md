# Rock-Paper-Scissors-simple-game.
Simple rock, paper, scissors game using ascii art. Takes user input and returns it's own value.

Project Code:
rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''

import random

RPS = [rock, paper, scissors]

user_choice = int(input("Type 0 for Rock, 1 for Paper, or 2 for Scissors.\n"))
if user_choice >=3 or user_choice < 0:
  print("You typed an invalid number. Choose again.")
else:
  print("You chose:")
  print(RPS[user_choice])

  computer_choice = random.randint(0, 2)
  print("Computer chose:")
  print(RPS[computer_choice])


  if user_choice == 0 and computer_choice == 2:
    print("You win!")
  elif computer_choice == 0 and user_choice == 2:
    print("You lose!")
  elif computer_choice > user_choice:
    print("You lose!")
  elif user_choice > computer_choice:
    print("You win!")
  elif computer_choice == user_choice:
    print("It's a draw!")

Photo of code:

<img src="https://i.imgur.com/U9mp62M.png" height="100%" width="100%" alt="Password generator"/>
<img src="https://i.imgur.com/1AmmyFr.png" height="100%" width="100%" alt="Password generator"/>
