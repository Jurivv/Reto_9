# Reto_9
1.De los retos anteriores selecione 3 funciones y escribalas en forma de lambdas.
```python
# Programa, calculo de promedio
if __name__=="__main__":
 # Declaramos las 5 variables
 a : float = float(input("Piense en un numero y digitelo: \n "))
 b : float = float(input("Digite un numero completo y seguido del dia, mes y año de su nacimiento\nejemplo, dia 19 mes 10 año 2005, numero resultante 19102005: \n "))
 c : float = float(input("Digite su edad sumando el año en el que estamos: \n "))
 d : float = float(input("Digite un numero re random: \n "))
 e : float = float(input("Preguntele a su amigo un numero mayor a 500 y escribalo: \n "))
 #Utilizamos la función Lambda
promedio = (lambda a,b,c,d,e:(a+b+c+d+e)/5)(a,b,c,d,e)
# Mostrar resultado funcion Anonima
print("El promedio de los números digitados es: ",promedio)
```
```python
'''cantidad de carne de aves en kilos si se tienen N gallinas,
M gallos y K pollitos cada uno pesando 6 kilos, 7 kilos y 1 kilo respectivamente.
'''
if __name__ == "__main__":
# nombramos las variables
 n: float= float(int(input("Cantidad de gallinas: ")))
 m: float= float(int(input("Cantidad de gallos: ")))
 k: float= float(int(input("Cantidad de pollitos: ")))
 #Utilizamos función lambda
 #Suponemos que una gallina pesa 6kg, un gallo 7kg y un pollito 1kg
masa=(lambda n,m,k:(n*6)+(m*7)+(k*1))(n,m,k)
print("El peso de ",n, "gallinas, ",m, "gallos y ",k, "pollitos es de ",masa, "kilos")

```
```python
#Calcular una función Racional
if __name__ == "__main__":
 #Nombramos las variables
 z = float(input("Digite un número: "))
 #Utilizamos la función lambda
 fx= (lambda z : z/(z**(1/3)-1))(z)
 #Mostrar resultado
 print("El resultado de su funcion F(x) es: ",fx)
```
2.De los retos anteriores selecione 3 funciones y escribalas con argumentos no definidos (*args).
```python
def listado(*args)-> int: # Definimos variable
  cuadrado : int = 0 # inicializamos el programa
  for num in args: # para los numeros que hay en args aplicar el cuadrado
    cuadrado=num**2
  return cuadrado
if __name__ == "__main__": 
    a = int(input("Ingrese numero : ")) 
    print("el cuadrado del numero es " + str(listado(a)))

```
```python
def factorial(*args)-> int: # Definimos variable
   for num in args: # para los numeros que hay en args aplicar la condicion impuesta
       a = 1
       b = 1
       while a <= num:# se hace un bucle para poder realizar el factorial del numero
        b = b * a
        a += 1
   return b
if __name__ == "__main__":
    c = int(input("Ingrese numero : "))
    if 0 <= c:
       print("el factorial del numero es " + str(factorial(c)))
    else:
     print("Digtaste un número fuera de los parametros")

```
```python
def ASCII(*args)-> int: #definimos l variable
     for num in args: #para los numeros que hay en args aplicar la condicion impuesta en a,la cual es convertir un entero a codigo ASCII
      a=(chr(num))
     return a
if __name__ == "__main__":
      a = int(input("Digite un numero entero"))
      if a > 97 and a < 122: #establecemos un intervalo donde tiene sentido el código ASCII
        print("El numero entero corresponde a una vocal minuscula en el codigo ASCII, es:"+(ASCII(a)))
      else:
        print("No corresponde a una vocal minuscula en el codigo ASCII")

```

3.Escriba una función recursiva para calcular la operación de la potencia.
```python
'''función recursiva para la potencia de un número
creamos una función'''
def potencia(num1,num2):
    '''Ordenamos al programa restricciones para seguir operando
    si el exponente es 0 o 1 el resultado es inmediato,
    sin embargo si es diferente de estos, se le debera restar 1'''
    if num2 ==0:
        return 1
    elif num1 == 0:
        return 0
    elif num2==1:
        return num1
    else:
        return num1 * potencia(num1, num2-1)
   
if __name__=="__main__":
    num1=float(input("Digite numero 1: "))
    num2=float(input("Digite numero 2: "))
    print("Su numero es: "+str(potencia(num1,num2)))

```

4.Utilice la siguiente plantilla de code para contar el tiempo:
```python
import time

start_time = time.time()
# instrucciones sobre las cuales se quiere medir tiempo de ejecución
end_time = time.time()

timer = end_time - start_time
print(timer)
```
Realice pruebas para calcular fibonacci con iteración o con recursión. Determine desde que número de la serie la diferencia de tiempo se vuelve significativa. 

```python

```

5.
[![image.png](https://i.postimg.cc/cLW92tbT/image.png)](https://postimg.cc/Wh9wJzjJ)

6.

[![image.png](https://i.postimg.cc/59n268wQ/image.png)](https://postimg.cc/c6tSzgkd)
