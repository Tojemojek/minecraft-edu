# Płot

- Będziemy używać bloku o nazwie: `OAK_FENCE`
- Po polsku: płot z dębu, jeden słupek ogrodzenia

## Nowa funkcja

Funkcja to nazwa dla kilku poleceń zebranych razem. W Pythonie tworzysz ją tak:

```python
def nazwa():
    polecenie
```

- `def` znaczy: tu zaczyna się nowa funkcja.
- `nazwa` to nazwa, które sam wybierasz.
- `()` to puste nawiasy. Na razie nic do nich nie wpisujesz.
- Dwukropek `:` kończy pierwszą linię.
- Polecenia w środku są przesunięte w prawo. To wcięcie. Mówi Pythonowi: to należy do tej funkcji.

Funkcja sama nic nie robi, dopóki jej nie uruchomisz.

## Pętla for

Pętla powtarza polecenie. W Pythonie tworzysz ją tak:

```python
for krok in range(10):
    polecenie
```

- `for` znaczy: powtarzaj.
- `krok` to licznik. Przy każdym powtórzeniu ma kolejną liczbę: 0, potem 1, potem 2.
- `in range(10)` znaczy: zrób to 10 razy. Zamiast 10 możesz wstawić zmienną.
- Dwukropek `:` kończy pierwszą linię.
- Polecenie w środku jest przesunięte w prawo, tak jak w funkcji.

`krok` liczy pętla. Tego pudełka nie zakładasz sam.

## pos(x, y, z)

`pos(x, y, z)` mówi, gdzie postawić blok. Liczy względem kierunków świata. 

- x - to wschód / zachód 
- y - to góra / dół 
- z - to południe, północ

Zanim zaczniesz budować - ustaw się twarzą na południe.

Nie poruszaj się w czasie budowania. To zmieni punkt od którego liczone są współrzędne.

## Lekcje

Jeden bok ogrodzenia: [płot](../lekcje/00_01_plot.md)

Całe ogrodzenie: [ogród](../lekcje/00_02_ogrod.md)

Ogrodzenie zrobione przez agenta: [ogród robiony przez agenta](../lekcje/00_03_ogrod-agent.md)
