# Poligonos
print("DIBUJANDO POLIGONOS")
from turtle import Turtle
def OKI(n):
    try:
		   n=int(n)
		except:
		   n=OKI(input("Caracter no valido: "))
		return n
def OK(n):
    try:
		   n=float(n)
		except:
		   n=OK(input("Caracter no valido: "))
		return n
t=Turtle()
t.hideturtle()
cf=input("Indica el color del fondo: ")
ct=input("Indica el color de la linea: ")
while cf==ct:
    ct=input("Los colores del fondo y de la línea coinciden usa otro color: ")
gt=input("Indica el grosor de la linea: ")
t.screen.bgcolor(cf)
t.color(ct)
t.pensize(gt)
n=OKI(input("Indica el número de lados del poligono: "))
ln=OK(input("Indica la longitud de la línea: "))
ang=180-(((n-2)/n)*180)
for i in range(n):
    t.left(ang)
		t.fd(ln)
t.screen.mainloop()



  
