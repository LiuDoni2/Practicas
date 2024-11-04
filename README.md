# Algoritmo de Ordenamiento Burbuja

El **ordenamiento burbuja** es un algoritmo simple utilizado para ordenar listas. Funciona comparando elementos adyacentes y cambiándolos de posición si están en el orden incorrecto. Este proceso se repite hasta que la lista queda completamente ordenada.

## ¿Cómo funciona?

1. Compara el primer elemento con el segundo.
2. Si el primer elemento es mayor que el segundo, se intercambian.
3. Se repite este proceso para cada par de elementos adyacentes en la lista.
4. Se repite el proceso para toda la lista hasta que no se necesitan más intercambios.

## Implementaciones en Diferentes Lenguajes

### Python

```python
def burbuja(lista):
    for i in range(len(lista)):
        for j in range(len(lista) - 1):
            if lista[j] > lista[j + 1]:
                lista[j], lista[j + 1] = lista[j + 1], lista[j]

n = int(input("¿Cuántos números quieres ingresar? "))
lista = [int(input(f"Ingrese el número en la posición {i + 1}: ")) for i in range(n)]

print("Lista original:", lista)
burbuja(lista)
print("Lista ordenada:", lista)

