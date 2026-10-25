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

## pos_local(x, y, z)

`pos_local(x, y, z)` mówi, gdzie postawić blok. Liczy od ciebie, od strony, w którą patrzysz.

- `x` to w lewo albo w prawo. Większa niż zero idzie w lewo. Mniejsza niż zero idzie w prawo. Zero zostawia cię na miejscu.
- `y` to w górę albo w dół. Większa niż zero idzie w górę. Mniejsza niż zero idzie w dół. Zero to wysokość twoich stóp.
- `z` to do przodu albo do tyłu. Większa niż zero idzie do przodu. Mniejsza niż zero idzie do tyłu.

`pos_local` liczy od twojego wzroku. Obracasz się, patrzysz na miejsce budowy i liczby pasują do tego, co widzisz.

Nie kręć myszką w trakcie budowania. „Do przodu” zmienia się razem z twoim wzrokiem.

## Lekcje

Jeden bok ogrodzenia: [plot](../lekcje/plot.md)

Całe ogrodzenie: [ogrod](../lekcje/ogrod.md)

Ogrodzenie zrobione przez agenta: [ogrod-agent](../lekcje/ogrod-agent.md)
