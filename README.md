while True:
    print("Rock paper or scissors(r/p/s)")
    option = input().lower()
    import random
    computer= random.choice(["r", "p", "s"])
    if option == "r" and computer == "s":
        print("You win! I chose scissors.")
        break
    elif option == "r" and computer == "p":
        print("You lose! I chose paper.")
        break
    elif option == "p" and computer == "r":
        print("You win! I chose rock.")
        break
    elif option == "p" and computer == "s":
        print("You lose! I chose scissors.")
        break
    elif option == "s" and computer == "p":
        print("You win! I chose paper.")
        break
    elif option == "s" and computer == "r":
        print("You lose! I chose rock.")
        break
    elif option == computer:
        print("It's a tie! We both chose the same.")
        break
    else:
        print("Invalid input")
