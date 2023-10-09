# python
this is my first repositary
import random
rannum=random.randint(1,50)
gueesed=None
guess=0
while(rannum!=gueesed):
    gueesed=int(input("guess a number:"))
    if(rannum==gueesed):
        print("number is right u gueesed right")
        guess+=1
    else:
        print("you gueesed wrong number try again!")
        guess=+1
    if(rannum>gueesed):
        print("the number is small")
    elif(rannum<gueesed):
        print("the number is large")
with open("hiscore.txt","r") as f:
    hiscore= int(f.read())
if(hiscore>guess):
    with open("hiscore.txt","w")as f:
        hiscore=f.write(str(guess))
    
