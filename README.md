# Stone-paper-scissor-game

import random
game = False
while not game:
    f=input("Do you want to play the game(yes or no): ")
    g=f.lower()
    if f=="yes":
        print("Select one to play the game")
        a = input("Choose one (stone, paper, scissor):").lower() 
        c = ["stone", "paper", "scissor"]
        d = random.randint(0, 2)
        e = c[d]

        print(f"Computer chose: {e}")

        if (a == "paper" and e == "stone") or (a == "stone" and e == "scissor") or (a == "scissor" and e == "paper"):
            print("User won the match")
        elif (e == "paper" and a == "stone") or (e == "stone" and a == "scissor") or (e == "scissor" and a == "paper"):
            print("Computer won the match")
        else:
            print("Tie")
    else:
        game=True
print("Thanks for playing game....")
