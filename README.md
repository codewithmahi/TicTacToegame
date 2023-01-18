# TicTacToegame
import random
toprow=[1,2,3]
midrow=[4,5,6]
botrow=[7,8,9]
availablenums=[1,2,3,4,5,6,7,8,9]
pname=input("What is your name?\n")
print(toprow)
print(midrow)
print(botrow)
while True:
    pinput=int(input("Please enter a number from 1-9 (1 being the top-left square and 9 being the bottom-right square)\n"))
    if pinput==1:
        toprow[0]="X"
        availablenums.remove(1)
    if pinput==2:
        toprow[1]="X"
        availablenums.remove(2)
    if pinput==3:
        toprow[2]="X"
        availablenums.remove(3)
    if pinput==4:
        midrow[0]="X"
        availablenums.remove(4)
    if pinput==5:
        midrow[1]="X"
        availablenums.remove(5)
    if pinput==6:
        midrow[2]="X"
        availablenums.remove(6)
    if pinput==7:
        botrow[0]="X"
        availablenums.remove(7)
    if pinput==8:
        botrow[1]="X"
        availablenums.remove(8)
    if pinput==9:
        botrow[2]="X"
        availablenums.remove(9)
    compinput=random.choice(availablenums)
    if compinput==1:
        toprow[0]="O"
        availablenums.remove(1)
    if compinput==2:
        toprow[1]="O"
        availablenums.remove(2)
    if compinput==3:
        toprow[2]="O"
        availablenums.remove(3)
    if compinput==4:
        midrow[0]="O"
        availablenums.remove(4)
    if compinput==5:
        midrow[1]="O"
        availablenums.remove(5)
    if compinput==6:
        midrow[2]="O"
        availablenums.remove(6)
    if compinput==7:
        botrow[0]="O"
        availablenums.remove(7)
    if compinput==8:
        botrow[1]="O"
        availablenums.remove(8)
    if compinput==9:
        botrow[2]="O"
        availablenums.remove(9)
    print("___________")
    print(toprow)
    print(midrow)
    print(botrow)
    print("___________")
    if toprow[0] and toprow[1] and toprow[2] == "X":
        print(pname,"wins! Well done",pname,"!")
        break
    elif midrow[0] and midrow[1] and midrow[2] == "X":
        print(pname,"wins! Well done",pname,"!")
        break
    elif botrow[0] and botrow[1] and botrow[2] == "X":
        print(pname,"wins! Well done",pname,"!")
        break
    elif toprow[0] and midrow[0] and botrow[0] == "X":
        print(pname,"wins! Well done",pname,"!")
        break
    elif toprow[1] and midrow[1] and botrow[1] == "X":
        print(pname,"wins! Well done",pname,"!")
        break
    elif toprow[2] and midrow[2] and botrow[2] == "X":
        print(pname,"wins! Well done",pname,"!")
        break
    elif toprow[0] and midrow[1] and botrow[2] == "X":
        print(pname,"wins! Well done",pname,"!")
        break
    elif toprow[2] and midrow[1] and botrow[0] == "X":
        print(pname,"wins! Well done",pname,"!")
        break
