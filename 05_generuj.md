Funkjca generuj(n, start, koniec) ma za zadanie wygenerować listę z n - elementami, każdy element ma być losowany 
z przedziału [start, koniec).
```python
import random
def main():
    n = 5
    start = 100
    koniec = 200
    print(generuj(n,start,koniec))

def generuj(n,start,koniec):
    wynik = []
    for i in range(0,n):
        los = random.randint(start,koniec)
        wynik.append(los)
    return wynik
main()
```
