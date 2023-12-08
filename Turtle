import turtle

def draw_fractal(t, order, size):
    if order == 0:
        t.forward(size)
    else:
        for angle in [60, -120, 60, 0]:
            draw_fractal(t, order - 1, size / 3)
            t.left(angle)

def main():
    screen = turtle.Screen()
    screen.bgcolor("white")

    fractal_turtle = turtle.Turtle()
    fractal_turtle.shape("turtle")
    fractal_turtle.color("blue")
    fractal_turtle.speed(2)

    fractal_order = 4
    fractal_size = 300

    fractal_turtle.penup()
    fractal_turtle.goto(-fractal_size / 2, -fractal_size / 2)
    fractal_turtle.pendown()

    draw_fractal(fractal_turtle, fractal_order, fractal_size)

    screen.exitonclick()

if __name__ == "__main__":
    main()
