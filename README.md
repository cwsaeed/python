#Animation

import turtle as t
import colorsys

t.bgcolor("white")
t.speed("fastest")
t.tracer(1000)
t.pencolor("white")
hue = 5
t.hideturtle()

def func():
    global hue
    for i in range(4):
        global hue
        for i in range(4):
            color = colorsys.hsv_to_rgb(hue,1, 1)
            hue+=0.01
            t.fillcolor(color)
            t.begin_fill()
            t.fd(100)
            t.right(108)
            t.fd(100)
            t.lt(22)
            t.end_fill()

for j in range(400):
    func()
    t.goto(9, 9)
    t.rt(188888)

t.exitonclick()

