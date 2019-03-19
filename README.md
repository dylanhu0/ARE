# ARE
1)
from tkinter import *
import random
import time

WIDTH = 800
HEIGHT = 400

root = Tk()
canvas = Canvas(root, width = WIDTH, height= HEIGHT)
root.title('Bouncing Ball')
canvas.pack()

ball = canvas.create_oval(10, 10, 60, 60, fill='orange')
ball2 = canvas.create_oval(10, 10, 60, 60, fill='green')
xspeed = 4
yspeed = 5
xspeed2 = 6
yspeed2 = 6


while True:
    canvas.move(ball, xspeed, yspeed)
    pos = canvas.coords(ball)

    if pos[3] >= HEIGHT or pos[1] <= 0:
        yspeed = -yspeed
    if pos[2] >= WIDTH or pos[0] <= 0:
        xspeed = -xspeed
    
    canvas.move(ball2, xspeed2, yspeed2)
    pos = canvas.coords(ball2)
    if pos[3] >= HEIGHT or pos[1] <= 0:
        yspeed2 = -yspeed2
    if pos[2] >= WIDTH or pos[0] <= 0:
        xspeed2 = -xspeed2

    root.update()
    time.sleep(0.01)

root.mainloop()

2)
# from tkinter import * 

root = Tk()
root.geometry('500x500')


# label
l = Label(root, text= " 1+1")
l.pack(side=LEFT)

def buttonfunction():


   print("TRUE")

b = Button(root, text= "2", command=buttonfunction)
b.place(x=40, y=150, width=50, height=50)
def buttonfunction2():

     print("FALSE")
b2 = Button(root, text= "3", command=buttonfunction2)
b2.pack(side=RIGHT)



root.mainloop()







3)from tkinter import *
import random
import time

root = Tk()
canvas = Canvas(root, width = WIDTH, height= HEIGHT)
root.title('Bouncing Ball')
canvas.pack()
WIDTH = 500
HEIGHT = 400


def buttonfunction():
   
    ball = canvas.create_oval(10, 10, 60, 60, fill='orange')
    ball2 = canvas.create_oval(10, 10, 60, 60, fill='green')
    xspeed = 4
    yspeed = 5
    xspeed2 = 6
    yspeed2 = 6



    while True:
        canvas.move(ball, xspeed, yspeed)
        pos = canvas.coords(ball)

        if pos[3] >= HEIGHT or pos[1] <= 0:
            yspeed = -yspeed
        if pos[2] >= WIDTH or pos[0] <= 0:
            xspeed = -xspeed
    
        canvas.move(ball2, xspeed2, yspeed2)
        pos = canvas.coords(ball2)
        if pos[3] >= HEIGHT or pos[1] <= 0:
            yspeed2 = -yspeed2
        if pos[2] >= WIDTH or pos[0] <= 0:
            xspeed2 = -xspeed2

        root.update()
        time.sleep(0.01)

b = Button(root, text= "Click", command=buttonfunction)
b.place(x=50, y=150, width=50, height=50)
        
root.mainloop()


