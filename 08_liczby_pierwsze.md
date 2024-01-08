Wczytaj liczbę naturalną do zmiennej n. Znajdź wszystkie podzielniki liczby n, będące liczbami pierwszymi.
```python
def main():
    n = int(input("podaj liczbę: "))
    print(wszystkie(n))

def podzielniki(n):
    lista = []
    for i in range(1,n+1):
        if n % i == 0:
            lista.append(i)
    return lista
def pierwsza(n):
    if n < 2:
        return False
    for i in range(2, int(n**0.5)+1):
        if n % i == 0:
            return False
    else:
        return True
def wszystkie(n):
    wynik = []
    for i in podzielniki(n):
        if pierwsza(i) == True:
            wynik.append(i)
    return wynik

main()
```
