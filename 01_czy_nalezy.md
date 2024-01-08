Funkcja czy_nalezy(lista, element) => czy element należy do list, czy element jest w liście, 
np.: [5,3,1,4,2] i 4  => odpowiedź True
```python
def main():
    lista = [5,3,1,4,2]
    element = 4
    print(czy_nalezy(lista,element))

def czy_nalezy(lista,element):
    for i in lista:
        if element == i:
            return True
    return False
main()
```

