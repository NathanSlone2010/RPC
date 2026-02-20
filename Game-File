import time
import os
import random
import platform
#These are the required modules.


os_type = platform.system()
if os_type == "Windows":
    print("Operating System owner: Microsoft | WINDOWS-OS")
elif os_type == "Darwin":
    print("Operating System owner: Apple Computer, Inc. | MacOS")
elif os_type == "Linux":
    print("Operating System owner: OPEN SOURCE OS | Linux Kernel")
elif os_type in ["FreeBSD", "OpenBSD", "NetBSD"]:
    print("Operating System owner: OPEN SOURCE OS | BSD")
elif os_type == "iOS":
    print("Operating System owner: Apple Computer, Inc. | iOS")
else:
    print("\nUNKNOWN OPERATING SYSTEM DETECTED... PROGRAM MAY NOT RUN AS EFFICIENTLY")
#OS detection.


print("\nWelcome to Rock, Paper, or Scissors!")

choice = ["Rock", "Paper", "Scissors"]

player_score = 0
computer_score = 0

while True:
    computer = random.choice(choice)
    player = input("Choose Rock, Paper, or Scissors [exit to end]: ").capitalize()

    if player.lower() == "exit":
        print("Thanks for playing!")
        break

    if player not in choice:
        print("Invalid input, try again.\n")
        continue

    print(f"Computer chose: {computer}")

    win = (player == "Rock" and computer == "Scissors") or (player == "Scissors" and computer == "Paper") or (player == "Paper" and computer == "Rock")

    if player == computer:
        time.sleep(0.5); print("TIE.\n")
    elif win:
        player_score += 1
        time.sleep(1); print("PLAYER WINS!\n")
    else:
        computer_score += 1
        time.sleep(0.7); print("COMPUTER WINS!\n")

    print(f"Player: {player_score} | Computer: {computer_score}\n")
