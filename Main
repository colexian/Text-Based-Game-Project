
#Globals
#------------------------------------
playerclass = 0
playerName = 0

warriorStats = {
		"Strength" : 15,
		"Dexterity" : 13,
		"Constitution" : 14,
		"Intelligence" : 12,
		"Wisdom" : 8,
		"Charisma" : 10
	}

wizardStats = {
		"Strength" : 8,
		"Dexterity" : 10,
		"Constitution" : 13,
		"Intelligence" : 15,
		"Wisdom" : 14,
		"Charisma" : 12
	}

#------------------------------------

#Beginning of game, lets player choose player character class
def intro():
    
    print("Welcome, Player 1. This is the world of NAMEPENDING")
    print("Choose your class. Choose wisely, this will determine your abilities and stats")
    
    
    print("1: Warrior, A fighter rigorously trained in hand-to-hand combat. Wields all melee weapons. High Strength and Constitution growth")
    print("2: Wizard, A studious magician that can conjure and project magic to harm enemies. Wields staves or wands. High Intelligence and Wisdom growth")
    global playerclass
    playerclass = input("Type 1 for Warrior or 2 for Wizard")

    return playerclass

#Lets player set name of player character. Better exception handling? Double check?
def playerName():
    global playerName
    playerName = input("What is your name?", playerclass,"?")
    if type(playerName) != str:
        print("Please, use only strings for a name")
    else: print("Welcome to the world of NAMEPENDING,", playerName,".")
    return playerName

#Tie class to number, probably would be better as a dictionary or array with larger number of classes
def classname(classNumber):
    if classNumber == "1":
        classname = "Warrior"
    else:
        classname = "Wizard"
    return(classname)


intro()


#Checks to make sure player is comfortable with class choice, gives chance to repick. Better exception handling?
while True:
    while True:
        answer = input('Are you sure? (y/n): ')
        if answer in ('y', 'n'):
            break
        print('Invalid input.')
    if answer != 'y':
        intro()
    else:
        playerName()
