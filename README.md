# Reto_cuatro
Reto 4, programación de Computadoras
En este repositorio se desarrolla el reto 4 :)

## Primer Punto
### Dado un número entero, determinar si ese número corresponde al código ASCII de una vocal minúscula
```
num = int (input ("Ingrese un numero entero"))
if (num == 97):
    print (f"El numero {num} corresponde a la vocal {chr(num)} en codigo ASCII")
elif (num == 101):
    print (f"El numero {num} corresponde a la vocal {chr(num)} en codigo ASCII")
elif (num == 105):
    print (f"El numero {num} corresponde a la vocal {chr(num)} en codigo ASCII")
elif (num == 111):
    print (f"El numero {num} corresponde a la vocal {chr(num)} en codigo ASCII")
elif (num == 117):
    print (f"El numero {num} corresponde a la vocal {chr(num)} en codigo ASCII")
else:
    print (f"El numero {num} no corresponde a ninguna vocal minuscula en el codigo ASCII")
```
## Segundo punto
### Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no.
```
letra : str; conversion : int
letra = str (input ("Ingrese una letra"))
conversion = ord(letra)
if (conversion %2 == 0):
    print (f"La letra {letra} corresponde al codigo ASCII {conversion} el cual es PAR")
else:
    print (f"La letra {letra} tiene un codigo {conversion} el cual es PAR")
```
## Tercer punto
### Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no.
```
caracter = str (input ("Ingrese un caracter"))
conversion = ord (caracter)
if (48 <= conversion <= 57):
    print (f"El caracter {caracter} segun el codigo ASCII es un digito y tiene el codigo: {conversion}")
else:
    print (f"El caracter {caracter} segun el codigo ASCII no es un digito")
```
## Cuarto punto
### Dado un número real x, construya un programa que permita determinar si el número es positivo, negativo o cero. Para cada caso de debe imprimir el texto que se especifica a continuación:Positivo: "El número x es positivo", Negativo: "El número x es negativo", Cero (0): "El número x es el neutro para la suma"
```
num: float
num = float (input("Ingrese un numero real"))
if (num > 0):
    print (f"El numero {num} es positivo")
elif (num < 0):
    print (f"El numero {num} es negativo")
else:
    print (f"El numero {num} es neutro para la suma")

```

## Quinto punto
### Dado el centro y el radio de un círculo, determinar si un punto de R2 pertenece o no al interior del círculo.
```
centro_x : float; centro_y : float; radio_circulo : float; cordenada_x_2 : float; cordenada_y_2 : float
centro_x = float (input("Ingrese la cordenada del centro del circulo en X: "))
centro_y = float (input("Ingrese la cordenada del centro del circulo en Y: "))
radio_circulo = float (input("Ingrese el radio del circulo: "))
cordenada_x_2 = float (input("Ingrese la cordenada del punto 2 en X: "))
cordenada_y_2 = float (input("Ingrese la cordenada del punto 2 en Y: "))

distancia = ((cordenada_x_2-centro_x)**2 + (cordenada_y_2-centro_y**2))**1/2
if (distancia <= radio_circulo):
    print (f"El punto ({cordenada_x_2},{cordenada_y_2} ) esta dentro del circulo")
else:
    print (f"El punto ( {cordenada_x_2},{cordenada_y_2}) NO esta dentro del circulo")
```
## Sexto punto
### Dadas tres longitudes positivas, determinar si con esas longitudes se puede construir un triángulo.
```
lado_1 : float; lado_2 : float; lado_3 : float; suma : float
lado_1 = float (input("Ingrese el lado 1"))
lado_2 = float (input("Ingrese el lado 2"))
lado_3 = float (input("Ingrese el lado 3"))

if (lado_1 > lado_2 and lado_1 >lado_3):
    suma = lado_2 + lado_3
    if (suma > lado_1):
        print (f"Es posible construir un triangulo")
elif (lado_2 > lado_1 and lado_2 >lado_3):
    suma = lado_1 + lado_3
    if (suma > lado_2):
        print (f"Es posible construir un triangulo")
elif (lado_3 > lado_2 and lado_3 >lado_1):
    suma = lado_2 + lado_1
    if (suma > lado_3):
        print (f"Es posible construir un triangulo")
else: 
    print ("No es posible contruir un triangulo con esas longitudes")
```
