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
