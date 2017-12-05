print("DIBUJANDO POLIGONOS")
from VALID import OKI, OK, ns
from turtle import Turtle
import subprocess
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


            
preg=ns(input("¿Activar Turtle?: "))
if preg==("s"):
    subprocess.call(["cmd.exe","/C","cls"])
    t=Turtle()
    t.hideturtle()
    while True:
        print("DIBUJANDO POLIGONOS")

        cf=set_color(input("Indica el color del fondo: "))
        ct=set_color2(input("Indica el color de la línea: "))
        while ct==cf or ct==(""):
            ct=set_color2(input("Especifica un color diferente para la línea: "))
        qc=ns(input("¿Especificar coordenadas?: "))
        if qc==("s"):
            cordenada_x=OKI(input("Introduce coordenada\'x\': "))
            cordenada_y=OKI(input("Introduce coordenada\'y\': "))
            t.color(cf)
            t.setx(cordenada_x)
            t.sety(cordenada_y)
        t.screen.bgcolor(cf)
        t.color(ct)
        gt=OK(input("Indica el grosor de la línea: "))
        t.pensize(gt)
        n=OKI(input("Indica el número de lados del polígono: "))
        ln=OK(input("Indica la longitud de la línea: "))
        ang=180-(((n-2)/n)*180)
        for i in range(n):
            t.left(ang)
            t.fd(ln)
        conti=ns(input("¿Dibujar nuevo poligono?: "))
        if conti==("s"):
            t.clear()
            subprocess.call(["cmd.exe","/C","cls"])
    t.screen.mainloop()


