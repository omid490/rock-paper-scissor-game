import random

# Creating the choices for user
choices = {0: "Rock", 1: "Paper", 2: "Scissor"}

# Asking user's choice rock scissor and paper...

user = int(input("What do you choose? 0 for Rock 1  for Paper or 2 for Scissor.\n"))
user_choice = (choices[user])
us = user_choice

# random list selection by computer RSP
computer_choice = ["Rock", "Paper", "Scissor"]
cc = random.choice(computer_choice)

print(f"You chose {us}")
print(f"Computer chose {cc}")

# making if computer RSP is equal to R and input is e, print this
if us == "Rock" and cc == "Scissor" or us == "Scissor" and cc == "Paper" or us == "Paper" and cc == "Rock":
    print("You win")
elif us == cc:
    print("it's a draw. No one wins. Try again.")
else:
    print("Computer wins, you lose.")
