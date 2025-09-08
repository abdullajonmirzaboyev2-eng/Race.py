# Race.py
Oddiy va yaxshi#
    
	import turtle
	from random import randint as r
    def race():
	tsbq1 = turtle.Turtle()
	           turtle.bgcolor('forestgreen')
	      
	tsbq1.shape('turtle')
	tsbq1.color('blue')
	tsbq1.penup()
	tsbq1.goto(-300, 200)
	tsbq1.pendown()
 
    tsbq2 = turtle.Turtle()
	tsbq2.shape('turtle')
	tsbq2.color('red')
	tsbq2.penup()
	tsbq2.goto(-300, 100)
	tsbq2.pendown()
	
	tsbq3 = turtle.Turtle()
	tsbq3.shape('turtle')
	tsbq3.color('yellow')
	tsbq3.penup()
	tsbq3.goto(-300, 0)
	tsbq3.pendown()
	
	finish = turtle.Turtle()
	finish.hideturtle()
	finish.speed(0)
	finish.penup()
	finish.pensize(5)
	finish.goto(300, 250)
	finish.pendown()
 
	for i in range(3):
		qiymat = True
		while qiymat:
			tezlik1 = r(1,5)
			tezlik2 = r(1,5)
			tezlik3 = r(1,5)
			
			tsbq1.penup()	
			tsbq1.forward(tezlik1)
			tsbq2.penup()	
			tsbq2.forward(tezlik2)
			tsbq3.penup()
			tsbq3.forward(tezlik3)
			
			if tsbq1.xcor() >= 300:
				tsbq1.penup()
				tsbq1.goto(0, 300)
				tsbq1.goto(-300, 200)
				tsbq2.goto(-300, 100)
				tsbq3.goto(-300, 0)
				break
				
			elif tsbq2.xcor() >= 300:
				tsbq2.penup()
				tsbq2.goto(0, 300)
				tsbq1.goto(-300, 200)
				tsbq2.goto(-300, 100)
				tsbq3.goto(-300, 0)
				break
				
			elif tsbq3.xcor() >= 300:
				tsbq3.penup()
				tsbq3.goto(0, 300)
				tsbq1.goto(-300, 200)
				tsbq2.goto(-300, 100)
				tsbq3.goto(-300, 0)
				break
		
				
			
				
	
	turtle.mainloop()	race()




