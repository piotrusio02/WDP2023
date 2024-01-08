Funkcja czy_zawiera(lista1, lista2) => czy lista2 jest podzbiorem listy1, czy wszystkie 
elementy listy2 należą do listy1, np.: [5,3,1,4,2] i [3,2] => odpowiedź True
```python
def main():
    lista1 = [5,3,1,4,2]
    lista2 = [3,2]
    element = 4
    print(czy_zawiera(lista1,lista2))

def czy_nalezy(lista1,element):
    for i in lista1:
        if element == i:
            return True
    return False

def czy_zawiera(lista1,lista2):
    for i in lista2:
        if czy_nalezy(lista1,i) == False:
            return False
    return True
main()
```
