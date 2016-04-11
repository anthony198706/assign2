# assign2
'''
This assignment is due by 11:59 pm MST on Monday (03/28/2016). You must submit it on Blackboard by clicking the above title link for the assignment.
You must use Python 3.x to implement these programs.
Your grade will be based on functionality (does the program do what it is suppose to do) and understandability (are the literals meaningful and is the code modular and well documented with appropriate comments).
Deliverables:

You should submit one doc (or docx or pdf) file named assign2.doc (or .docx or .pdf). This file should contain your python code for the program(s) in the assignment along with the screen shot(s) of your program's sample runs (with output). Make sure to put your python code correctly in this file (with correct indentation). If you have any text for the grader to read before grading, you can include it at the top of this file. 
You should also submit a python file named assign2.py. This file should contain your python code for the program(s) in the assignment. If needed, the code in this file will be executed to confirm the output presented in the word file.
____________________________________________________________________________________________________

(10 points) In this assignment you will use the `turtle` python module to draw a snowman. You may NOT use the Turtle.circle function to draw circles.

Snowman description:

The outline of the snowman should be in black.
The snowman’s body should be made of 3 circles.
Each circle should be centered above the one below it (except the bottom circle, which can be located anywhere).
There should be no gap between the circles.
Give the snowman eyes, a nose and four buttons (a hat is optional).
you can use the dot() function or stamp() function for eyes and buttons
you can draw a small triangle (or dot) for the nose
you should increase the width of turtle before using the dot function. use the width() function to set the width of turtle.
Optional parts (not required, but can get you two bonus points if done):

The snowman should be on a blue background, and should be drawn filled with white.
You can include two stick-arms and at least two fingers on each hand.
Draw some trees, simply draw green triangle with brown rectangle as stem. '''


#Anthony Tolbert
#Assignment 2

import turtle #import turle module

wn = turtle.Screen()    #create window
wn = turtle.bgcolor("blue")

turtleCirc = turtle.Turtle()    #create turtle named turtleCirc
turtleCirc.pen(fillcolor = "white", pensize = 2)
turtleCirc.speed(0)
turtleCirc.hideturtle()

turtleCirc.up() #setting the turtles in their starting positions
turtleCirc.setposition(0, -270)
turtleCirc.down()

turtleCirc.begin_fill() #create bottom circle
for i in range(313):
    turtleCirc.forward(2.5)
    turtleCirc.left(1.15)
turtleCirc.end_fill()

turtleCirc.up() #change position of turtle
turtleCirc.setposition(0, -20)
turtleCirc.down()

turtleCirc.begin_fill() #create middle circle
for i in range(313):
    turtleCirc.forward(1.7)
    turtleCirc.left(1.15)
turtleCirc.end_fill()

turtleCirc.up() #change position of turtle
turtleCirc.setposition(0, 150)
turtleCirc.down()

turtleCirc.begin_fill() #create top circle
for i in range(313):
    turtleCirc.forward(1.1)
    turtleCirc.left(1.15)
turtleCirc.end_fill()

turtleCirc.up() #create left eye for snowman
turtleCirc.setposition(-15, 220)
turtleCirc.down()
turtleCirc.pensize(4)
turtleCirc.color("black")
turtleCirc.dot(20)

turtleCirc.up() #Create right eye for snowman
turtleCirc.setposition(15, 220)
turtleCirc.down()
turtleCirc.color("black")
turtleCirc.dot(20)

turtleCirc.up() #Create nose for snowman
turtleCirc.setposition(-5, 190)
turtleCirc.down()
turtleCirc.color("orange")

for i in range(3):
    turtleCirc.forward(10)
    turtleCirc.left(120)

turtleCirc.up() #create first button
turtleCirc.setposition(0, 120)
turtleCirc.down()
turtleCirc.color("red")
turtleCirc.dot(20)

turtleCirc.up() #create second button
turtleCirc.setposition(0, 90)
turtleCirc.down()
turtleCirc.color("red")
turtleCirc.dot(20)

turtleCirc.up() #create third button
turtleCirc.setposition(0, 60)
turtleCirc.down()
turtleCirc.color("red")
turtleCirc.dot(20)

turtleCirc.up() #create fourth button
turtleCirc.setposition(0, 30)
turtleCirc.down()
turtleCirc.color("red")
turtleCirc.dot(20)




Coloring of different items: buttons, eyes, nose, hat.
