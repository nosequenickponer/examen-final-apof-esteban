Python

Parte 1
Ej.1 Ejecuta y entiende el siguiente programa.

num1 = int(input('Dime un numero del 1 al 10 '))   
num2 = int(input('Dime otro numero del 1 al 10 '))   
calcula = num1 * num2  
cadenaCalcula = str (calcula)  
print('El resultado es ')   
print (cadenaCalcula)
    
    
    
Ej.2 Realizar el siguiente programa:    
El usuario introduce un número de "dólares" y por pantalla sale su valor en Euros. (multiplicar por 0.9).


num1 = int(input('Dime los dólares'))  
calcula = num1 * 0.9  
cadenaCalcula = str (calcula)  
print('En euros seria ')  
print (cadenaCalcula)
Ej.3 Depura y repara el programa.

num1 = int(input('Dime un numero del 1 al 10 '))   
num2 = int(input('Dime otro numero del 1 al 10 '))    

if num1 > num2:  
    resultado = 'el primero'  
else:  
    resultado = 'el segundo'  
print ('El mayor es ' +str (resultado))



Ej.4 Depura (con puntos de interrupción) para corregir y ejecutar:

nota1 = float(input('Escribe la primera nota '))
nota2 = float(input('Escribe la segunda nota '))
nota3 = float(input('Escribe la tercera nota '))

media = (nota1 + nota2 + nota3)/3

if media > 5:
    resultat = "Aprobado"
else:
    resultat = "Suspendido"

print ('La nota final es ' + str(resultat))



Ej.5 Realizar el siguiente programa:

print("COMPARADOR DE NÚMEROS")
num1 = int(input("Escriba un número: "))
num2 = int(input("Escriba otro número: "))

if num1 > num2:
    print('El mayor es el primero: ' + str(num1))
elif num1 < num2:
    print('El mayor es el segundo: ' + str(num2))
else:
    print("Los dos números son iguales")
    
    
Ej.6 Ejecuta el siguiente programa:


marca = input ("Escribe la marca del coche")
modelo = input ("Escribe modelo del coche")

precio = 10000

if marca == "ford" or marca =="Ford" or marca == "FORD":
    descuento = 10;

if marca == "opel" or marca =="Opel" or marca == "OPEL":
    descuento = 20;

precio = precio - (precio * (descuento/100))
print (' El precio final es ' + str(precio) + '€')
Ej.7 Función del siguiente programa:

flagOK=0

while flagOK==0:
    valor = input ('Introduce seleccion (1-4)')
    numero = int(valor)
    if (numero > 1) and (numero <4):
        flagOK=1
Bucle hasta que escribes 2 o 3



Ej.8 Realizar un programa para una tienda de informática



El usuario introduce la marca y el modelo de la tarjeta gráfica y el programa saca el descuento correspondiente por pantalla. Si la tarjeta a la venta MSI, el descuento es del 5%
Si la tarjeta a la venta MSI, modelo GTX el descuento es del 10%
Si la tarjeta a la venta MSI, modelo IT el descuento es del 20%

marca = input ("Escribe el nombre de la marca")
modelo = input ("¿Es GTX?")
IT = input ("¿Es IT?")
descuento= 0

if marca == "MSI" or marca =="msi" or marca == "Msi":
    descuento = 5;

if modelo == "SI" or modelo =="si" or modelo == "Si":
    descuento = descuento + 5;

if IT == "Si" or IT =="si" or IT == "SI":
    descuento = descuento + 10;
print (' El descuento es ' + str(descuento))



Ej.9 Ejecuta el siguiente programa:


marca = input ("Escribe la marca del coche")
modelo = input ("Escribe modelo del coche")

precio = 10000

if marca == "ford" or marca =="Ford" or marca == "FORD":
    if modelo == "fiesta":
        descuento = 8;
    elif modelo == "focus":
        descuento = 15;
    else:
        descuento = 0;


if marca == "opel" or marca =="Opel" or marca == "OPEL":
    descuento = 20;

precio = precio - (precio * (descuento/100))

print (' El precio final es ' + str(precio) + '€')



Ej.10 Ejecuta el siguiente programa y haz el seguimiento con puntos de interrupción:

print("Comienzo")
for i in [0, 1, 2]:
    print("Hola ", end="")
print()
print("Final")



Ej.11 En base al siguiente código, realizar programa que pide al usuario cuantas veces quiere que aparezca el saludo y también su nombre. El programa saca en pantalla el saludo "Hola nombre" ese número de veces.

print("Comienzo")
nombre = input("Escribe tu nombre")
numero = int(input("Escribe el numero de veces que quieres que te salude"))
for i in range(numero):
    print("Hola "+str(nombre), end=" ")
    
    
    
Ej.12 Modificar siguiente programa para que cuente números impares menores que 50.

cuenta = 0
for i in range(1, 50):
    if (i % 2) == 1:
        cuenta = cuenta + 1

print("Hay " + str(cuenta) +" números impares")



Ej.13 Ejecutar y hacer seguimiento variables con punto interrupción para entender como funciona:

suma = 0
for i in [1, 2, 3, 4]:
    suma = suma + i
print("La suma de los números de 1 a 4 es" + str (suma))



Ej.14 Realizar programa que da como resultado la SUMA, de todos los números pares del 1 al 20.

cuenta = 0
suma = 0
for i in range(1, 20):
    if (i % 2) == 1:
        cuenta = cuenta + 1
        suma = suma + i

print("Hay " + str(cuenta) +" números impares")
print("la suma es " + str(suma) 



Ej.15 En base al siguiente programa, realizar programa que muestre tabla de multiplicar del 5:

print("Comienzo")
for i in [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]:
    print (5 * (i))
Ej.16 En base al siguiente código: realiza un programa donde el usuario introduce una palabra y el ordenador cuenta cuantas vocales "a" hay en dicha palabra.

palabra = input("Escribe una palabra")
contador= 0
for letter in palabra:
    if letter== "a" or letter== "A":
        contador= contador+1
        print(str(contador))
        
        
        
Funciones
Ej.1 Ejecuta el siguiente programa:

def subrutina():
    a = 2
    print("El valor: " + str(a))
    return

subrutina()
a= 5
print("Programa valor: " + str(a))



Ej.2 ) Ejecutar el siguiente programa. ¿La variable 'a' es local o global? "Reparar" el programa para que el resultado sea correcto.

def subrutina():
    print(a)
    a = 2
    print(a)
    return

a = 5
subrutina()
print(a)
Resuelto

def subrutina():
    a = 2
    print(a)
    return

a = 5
subrutina()
print(a)
Solución

La primera "a" es local.
La segunda "a" es global.




Ej.3 Ejecuta el siguiente programa:

def saludar(nombre, mensaje=' Hola '):
    print (mensaje + nombre)

usuario = input ("Nombre")
saludar(usuario)




Ej.4 Crear un programa con dos funciones. En el programa principal el usuario introduce su nombre y edad. En una función llamada 'Saludo' , aparece en pantalla "Buenos dias, nombre" y en la otra función aparece en pantalla "Pareces más joven que x años".

def saludar(nombre, mensaje=' Hola '):
    print (mensaje + nombre)
def edad(n, mensaje=' Pareces más joven que '):
    print (mensaje + str(n))

usuario = input ("Introduce nombre")
saludar(usuario)
anyos = int(input("Introduce tu edad"))
edad(anyos)




Ej.5 Ejecutar el siguiente programa. ¿Qué diferencias hay con el anterior?

def calcula_media(x, y):
    resultado = (x + y) / 2
    return resultado

a = 3
b = 5
media = calcula_media(a, b)
print("Media de " + str(a) + " y " + str(b) + " es: " +str(media))
print("Programa terminado")
Diferencias
Uno tiene op matemáticas mientras que el otro no, además de que en este último hay solo una función, y no hay ningún "intput".




Ej.6 Realizar programa "Calculadora". El usuario introduce 2 numeros por teclado y en el programa hay 5 funciones: suma, resta, división, multiplicación y módulo de ambos números.

def calculadora():

    op= int(input("Escribe la operación: 1= Suma, 2= Resta, 3= Multiplicación, 4= División"))
    num1 = float(input("Escribe un número"))
    num2 = float(input("Escribe otro número"))
    opsuma = num1+num2
    opresta =num1-num2
    opnmulti= num1*num2
    opdivision= num1/num2
    
    restodivision=num1/num2%2
    
    if op== 1:
        print ("El resultado es "+str(opsuma))
    if op== 2:
        print ("El resultado es "+str(opresta))
    if op== 3:
        print ("El resultado es "+str(opmulti))
    if op== 4:
        print ("El resultado es "+str(opdivision))
        print ("El resto es " +str(restodivision))
    return
    
calculadora()