# Snake-Water-Gun
#Snake drinks Water 🐍 > 💧 → Snake wins  Gun kills Snake 🔫 > 🐍 → Gun wins  Water damages Gun 💧 > 🔫 → Water wins
import random

computer = random.choice ([1,2,3])
youstr= input("enter your choice :")
youdict= {"s": 1,"w":2,"g": 3,}
reverseddict={1: "snake", 2: "water", 3: "gun"}
if youstr not in youdict:
    print("Invalid input! Please choose 's', 'w', or 'g'.")
    exit()
you =youdict[youstr]

print(f"your choice: {reverseddict[you]}\n computer choice: {reverseddict[computer]}")
if (computer==you):
    print("its draw")
else: 
    
    if (computer==1 and you ==2):
        print("you lose")
    elif (computer==1 and you ==3):
        print("you win")
    elif (computer==2 and you ==1):
        print("you win")
    elif (computer==2 and you ==3):
        print("you lose")
    elif (computer==3 and you ==2):
        print("you win")
    elif (computer==3 and you ==1):
        print("you lose")
    else:
        print("somthing want wrong:")
