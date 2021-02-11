# -Python-Project-2
#2 Magician or/and Expert

def is_magician(message):
    userInput = str(input(message)).lower()
    if userInput == "yes":
        return 1
    elif userInput == "no":
        return 0
    else:
        return is_magician("Hey,hey, hey! Please, use 'yes' or 'no' to answer.\n")

def is_expert(message):
    userInput = str(input(message)).lower()
    if userInput == "yes":
        return 1
    elif userInput == "no":
        return 0
    else:
        return is_expert("Woa! Use 'yes' or 'no'.\n")

magician = is_magician("Do you can use magic ?\n")
expert = is_expert("Are you a expert ?\n")

if magician == True and expert == True:
    print("You\'re a master magician!\n")
if magician == 1 and expert == 0:
    print("At least you\'re getting there.\n")
if magician == 0 and expert == 1:
    print("So... You\'re a expert... Hm... Interesting!\n")
if magician == 0 and expert == 0:
    print("You need some magic powers, fella !\n")
