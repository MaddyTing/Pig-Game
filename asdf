#Game of Pig 
#Final Version

import random

playersum = 0
compsum = 0
playerturn = 0
compturn = 0

player = input("Type GO to roll the die. ")

if(player == "GO"):
    if(playersum < 100 and compsum < 100):
        while(playersum < 100 and compsum < 100):
            die = random.randint(1, 6)
            if(die != 1):
                playerturn = playerturn + die
                print("\nYou rolled: " + str(die))
                print("Your turn total at this time is: " + str(playerturn))
                print("Your total at this time is: " + str(playersum))                
                playerhold = input("\nWould you like to hold? YES or NO? ")
                if(playerhold == "YES"):
                    playersum = playersum + playerturn
                    playerturn = 0
                    print("\nYour total at this time is: " + str(playersum))
                    print("Alright then, you've decided to hold! It's the computer's turn now!")
                    die = random.randint(1, 6)
                    print("\nThe computer rolled: " + str(die))
                    if(die == 1):
                        compturn = 0
                        print("The computer rolled a 1! It's your turn now!")
                        player = input("\nType GO to roll the die. ") 
                    elif(die != 1):
                        compturn = compturn + die
                        print("The computer's turn total at this time is: " + str(compturn))
                        print("The computer's total at this time is: " + str(compsum))
                        comphold = random.randint(1, 2)
                        while(comphold == 1):
                            print("The computer has decided not to hold. It's still the computer's turn!")
                            die = random.randint(1, 6)
                            if(die == 1):
                                compturn = 0
                                print("\nThe computer rolled a 1! It's your turn now!")
                                player = input("\nType GO to roll the die. ")     
                            elif(die != 1):
                                compturn = compturn + die
                                print("\nThe computer rolled: " + str(die))
                                print("The computer's turn total at this time is: " + str(compturn))
                                print("The computer's total at this time is: " + str(compsum))
                                comphold = random.randint(1, 2) 
                        if(comphold == 2):
                            compsum = compsum + compturn
                            compturn = 0
                            print("\nThe computer's total at this time is: " + str(compsum))
                            print("The computer has decided to hold. It's your turn!")
                            player = input("\nType GO to roll the die. ")  
                if(playerhold == "NO"):
                    print("You've chosen not to hold! Continue on.")
                    player = input("Type GO to roll the die. ")
                    die = random.randint(1, 6)
            elif(die == 1):
                playerturn = 0
                print("\nYou rolled a 1 - It's the computer's turn now!") 
                die = random.randint(1, 6)
                print("\nThe computer rolled: " + str(die))
                if(die == 1):
                    compturn = 0
                    print("The computer rolled a 1! It's your turn now!")
                    player = input("\nType GO to roll the die. ")                      
                elif(die != 1):
                    compturn = compturn + die
                    print("The computer's turn total at this time is: " + str(compturn))
                    print("The computer's total at this time is: " + str(compsum))
                    comphold = random.randint(1, 2)                   
                    while(comphold == 1):
                        print("The computer has chosen not to hold. It's still the computer's turn!")
                        die = random.randint(1, 6)
                        print("The computer rolled: " + str(die))
                        if(die == 1):
                            compturn = 0
                            print("\nThe computer rolled a 1! It's your turn now!")
                            player = input("\nType GO to roll the die. ") 
                        elif(die != 1):
                            compturn = compturn + die
                            print("The computer's turn total at this time is: " + str(compturn))
                            print("The computer's total at this time is: " + str(compsum))
                            comphold = random.randint(1, 2) 
                    if(comphold == 2):
                        compsum = compsum + compturn
                        compturn = 0
                        print("\nThe computer's total at this time is: " + str(compsum))
                        print("The computer has decided to hold. It's your turn!")
                        player = input("\nType GO to roll the die. ")  
        if(playersum >= 100 and compsum < 100):
            print("\nYou have won! Good game, and congrats!")
            print("Your final total is: " + str(playersum))
            print("The computer's final total is: " + str(compsum))
        elif(compsum >= 100):
            print("\nThe computer has won! You have lost. Better luck next time!")
            print("Your final total is: " + str(playersum))
            print("The computer's final total is: " + str(compsum))
else:
    print("You did not roll the dice :P")

                
