Wczytaj liczbę naturalną do zmiennej n. Znajdź największą liczbę ciągu Fibonacciego mniejszą od liczby n.
```python
def main():
    n = int(input("podaj liczbę: "))
    print(naj(n))

def fibonacci(n):
    fib = [0,1]
    while fib[-1] < n:
        fib.append(fib[-1] + fib[-2])
    return fib
def naj(n):
    wynik = 0
    for i in fibonacci(n):
        if i < n:
            wynik = i
    return wynik
main()
```
