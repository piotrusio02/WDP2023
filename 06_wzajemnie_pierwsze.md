Wczytaj liczbę naturalną do zmiennej n. Znajdź wszystkie liczby mniejsze od n wzajemnie pierwsze z liczbą n.
```python
def main():
    n = int(input("podaj liczbę: "))
    m = 3
    print(wszystkie(n))

def podzielniki(n):
    lista = []
    for i in range(1,n+1):
        if n % i == 0:
            lista.append(i)
    return lista
def NWD(n,m):
    nn = set(podzielniki(n))
    mm = set(podzielniki(m))
    return max(nn.intersection(mm))
def wzajemna(n,m):
    if NWD(n,m) == 1:
        return True
    return False
def wszystkie(n):
    wynik = []
    for i in range(1,n):
        if wzajemna(n,i) == True:
            wynik.append(i)
    return wynik
main()
```
