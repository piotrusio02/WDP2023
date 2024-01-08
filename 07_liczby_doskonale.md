Wczytaj liczbę naturalną do zmiennej n. Znajdź wszystkie liczby doskonałe mniejsze od n.
```python
def main():
    n = int(input("podaj liczbę: "))
    print(wszystkie(n))

def podzielniki(n):
    lista = []
    for i in range(1,n):
        if n % i == 0:
            lista.append(i)
    return lista
def suma(lista):
    sum = 0
    for i in lista:
        sum += i
    return sum
def doskonala(n):
    dz = podzielniki(n)
    su = suma(dz)
    return su == n
def wszystkie(n):
    wynik = []
    for i in range(1,n):
        if doskonala(i) == True:
            wynik.append(i)
    return wynik
main()
```
