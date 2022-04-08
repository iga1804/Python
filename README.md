# Python
#This is a guess the number game.
import random
secretNum=random.randint(1,1000)
print("I am thinking of a number between 1 and 1000.")

#Ask player to guess 5 times.
for guessesTaken in range(1,6):
    print("Take a guess.")
    guess=int(input())
    
    if guess<secretNum:
        print("You guess is too low.")
    elif guess>secretNum:
        print("You guess is too high.")
    else:
        break
        
if guess==secretNum:
    print("Good job! You guessed my number in " + str(guessesTaken) + " guess!")
else:
    print("Nope. The number I was thinking of was " + str(secretNum))
