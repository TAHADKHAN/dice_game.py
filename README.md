# dice_game.py
"A simple Python dice game where players roll dice to score points in a fun, interactive command-line interface."
# Python Dice Game

import random

def roll_dice():
    return random.randint(1,6)

def main():
    while 'True':
        roll = input("rolled the dice? (yes/no):").strip().lower()
        if roll == 'yes':
            print(f"you rolled a {roll_dice()}!")
        elif roll == 'no':
            print("goodbye!")   
            break
        else: 
            print("invalid in put please enter 'yes' or 'no'.")
if __name__ == "__main__":
    main()                
