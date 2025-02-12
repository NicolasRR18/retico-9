# retico-9

=============================================================

El objetivo era resolver el reto 9, el cual consistia en
realizar algoritmos con arreglos de listas
A continuacion adjunto la imagen del repo del profe Felipe:

============================================================

![image](https://github.com/user-attachments/assets/ed972b7e-ec66-4cde-b812-3c4cfd39ab83)

============================================================

 >-Asi que adjuntare capturas mostrando como estan
 >diseñados los codigos para cumplir con cada punto del reto,
 >los realice en visual studio code, a su vez adjuntaré
 >los codigos para que puedan ser copiados y probados.

============================================================

# Punto-1

![image](https://github.com/user-attachments/assets/6c0c394b-2089-46fb-a04e-a21c1ccf0e95)

```

def añadir_numeros(*args) -> list:
    numeros = [] 
    while True:
        n = float(input("Ingrese numeros. (para terminar ingrese (0))"))
        if n == 0:
            break 
        numeros.append(n)
    return numeros

if __name__ == "__main__":

    añadir = añadir_numeros()
    i = 0
    for x in añadir:
        i += x
    if len(añadir) > 0: 
        promedio = i/len(añadir)
        print("el promedio es:", promedio )
    else:
        print("no se ingresaron numeros")
        

```

============================================================

# Punto-2

![image](https://github.com/user-attachments/assets/d69a8e77-60af-46bf-b3f2-35708f2cc42c)

```

def añadir_numeros(*args) -> list:
    numeros_1 = [] 
    while True:
        n = float(input("Ingrese numeros. (para terminar ingrese (0))"))
        if n == 0:
            break 
        numeros_1.append(n)
    return numeros_1
def producto_punto(numeros_1, numeros_2):
    if len(numeros_1) != len(numeros_2):
        return "Las listas deben tener la misma longitud"
    
    resultado = 0
    for i in range(len(numeros_1)):
        resultado += numeros_1[i] * numeros_2[i]
    
    return resultado
if __name__ == "__main__":
    print("Cree esta primera lista")
    añadir_1 = añadir_numeros()
    print("Ingrese una segunda lista de igual longitud")
    añadir_2 = añadir_numeros()
    solucion = producto_punto(añadir_1, añadir_2)
    print("el producto punto de ", añadir_1," y ", añadir_2, " es ", solucion)
        

```
============================================================

# Punto-3

![image](https://github.com/user-attachments/assets/00461bb6-a3bb-4668-baa5-800535424922)

```

def añadir_numeros(*args) -> list:
    numeros_1 = [] 
    numeros_2 = []
    while True:
        n = float(input("Ingrese numeros. (para terminar ingrese (-1))"))
        if n == -1:
            break
        elif n == 0:
            numeros_2.append(n)
        else:
            numeros_1.append(n)
    return numeros_1 + numeros_2

if __name__ == "__main__":
    añadir_1 = añadir_numeros()
    print(añadir_1)
        

```

============================================================

# Punto-4

Bubble Sort es un algoritmo de ordenamiento básico pero no muy eficiente. Se basa en comparar pares de elementos adyacentes e ir intercambiándolos si están en el orden incorrecto. Este proceso se repite varias veces hasta que la lista esté completamente ordenada.

¿Cómo funciona?
Se comparan los dos primeros elementos de la lista.
Si el primero es mayor que el segundo, se intercambian.
Luego se pasa al siguiente par y se repite el proceso.
Cuando se llega al final, el elemento más grande ya está en su posición correcta (como si “flotara” al final, de ahí el nombre Bubble Sort).
Se repite todo el proceso, ignorando el último elemento ya ordenado, hasta que no haya más intercambios.
Ejemplo paso a paso:
Supongamos que tenemos la lista [5, 3, 8, 4, 2].

(5 y 3) → [3, 5, 8, 4, 2]
(5 y 8) → No se cambia
(8 y 4) → [3, 5, 4, 8, 2]
(8 y 2) → [3, 5, 4, 2, 8] (el 8 ya quedó en su lugar)
Se repite el proceso hasta que la lista quede ordenada: [2, 3, 4, 5, 8]

Complejidad del algoritmo
Peor caso y caso promedio: 
𝑂
(
𝑛
2
)
O(n 
2
 ) (cuando la lista está invertida o desordenada)
Mejor caso: 
𝑂
(
𝑛
)
O(n) (cuando la lista ya está ordenada, y solo hacemos una pasada)
En terminos de eficiencia se queda un poco atras puesto que para listas grandes, hay mejores algoritmos como Merge Sort o Quick Sort. Sin embargo, es fácil de entender y bueno para aprender sobre ordenamiento.

============================================================
# REFERENCIAS
-https://www.geeksforgeeks.org/bubble-sort-algorithm/
-https://www.cuemath.com/algebra/dot-product/
