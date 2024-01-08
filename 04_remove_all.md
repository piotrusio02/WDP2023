Napisz funkcję remove_all(napis, usuwany), której wynikiem jest napis powstały poprzez usunięcie z napisu będącego jej
pierwszym argumentem, wszystkich wystąpień napisu będącego jej drugim argumentem. Przykładowo, wynikiem wywołania
remove_all("abrakadabra", "ab") będzie napis "rakadra". W funkcji main przetestuj działanie funkcji remove_all.
```python
def main():
    napis = "abrakadabra"
    usuwany = "ab"
    print(remove_all(napis,usuwany))

def remove(napis, usuwany):
    for i in range(len(napis)):
        if napis[i] == usuwany[0]:
            x = i + len(usuwany)
            nowe = napis[i:x]
            if nowe == usuwany:
                return napis[:i] + napis[x:]
    return napis

def remove_all(napis, usuwany):
    i = 0
    while i < len(napis):
        napis = remove(napis, usuwany)
        i += 1
    return napis
main()
```
