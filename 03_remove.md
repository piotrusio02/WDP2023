Napisz funkcję remove(napis, usuwany), której wynikiem jest napis powstały poprzes usunięcie z napisu będącego jej 
pierwszym argumentem, pierwszego wystąpienia napisu będącego jej drugim argumentem. Przykładowo, wynikiem wywowłania
remove("abrakadabra","ab") będzie napis "rakadabra". W funkcji main przestestuj działanie funkcji remove.
```python
def main():
    napis = "abrakadabra"
    usuwany = "ab"
    print(remove(napis,usuwany))

def remove(napis, usuwany):
    for i in range(len(napis)):
        if napis[i] == usuwany[0]:
            x = i + len(usuwany)
            nowe = napis[i:x]
            if nowe == usuwany:
                return napis[:i] + napis[x:]
    return napis
main()
```
