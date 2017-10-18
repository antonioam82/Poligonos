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
def set_color(cf):
    try:
      t.screen.bgcolor(cf)
		except:
		  cf=set_color(input("Color no valido: "))
		return cf
def set_color2(ct):
    try:
		  t.color(ct)
		except:
		  ct=set_color2(input("Color no valido: "))
		return ct

t=Turtle()
t.hideturtle()
cf=set_color(input("Indica el color del fondo: "))
ct=set_color2(input("Indica el color de la linea: "))
while cf==ct:
    ct=input("Los colores del fondo y de la línea coinciden usa otro color: ")
qc=ns(input("¿Especificar coordenadas?: ")
if qc==("s"):
   cordenada_x=OK(input("cordenada x: "))
	 cordenada_y=OK(input("cordenada y: "))
	 t.color(cf)
	 t.setx(cordenada_x)
	 t.sety(cordenada_y)
t.screen.bgcolor(cf)
t.color(ct)
gt=input("Indica el grosor de la linea: ")
t.pensize(gt)
n=OKI(input("Indica el número de lados del poligono: "))
ln=OK(input("Indica la longitud de la línea: "))
ang=180-(((n-2)/n)*180)
for i in range(n):
    t.left(ang)
		t.fd(ln)
t.screen.mainloop()



  
