# Domek z sześciu ścian

Zbudujesz mały domek. Każda ściana jest z innego materiału. Teoria o `pos_local` jest w [bloki/plot.md](../bloki/plot.md). Nazwy bloków z tej lekcji są w [bloki/domek.md](../bloki/domek.md).

Domek staje przed tobą. Nie kręć myszką, dopóki się nie zbuduje.

## Kod

Wklej to w Code Builderze. Zostaw wcięcia.

```python
def zbuduj_domek():
    blocks.fill(PLANKS_OAK, pos_local(-3, -1, 3), pos_local(3, -1, 8), FillOperation.REPLACE)
    blocks.fill(PLANKS_SPRUCE, pos_local(-3, 3, 3), pos_local(3, 3, 8), FillOperation.REPLACE)
    blocks.fill(STONE_BRICKS, pos_local(-3, 0, 8), pos_local(3, 2, 8), FillOperation.REPLACE)
    blocks.fill(PLANKS_BIRCH, pos_local(3, 0, 3), pos_local(3, 2, 8), FillOperation.REPLACE)
    blocks.fill(SANDSTONE, pos_local(-3, 0, 3), pos_local(-3, 2, 8), FillOperation.REPLACE)
    blocks.fill(BRICKS, pos_local(-3, 0, 3), pos_local(3, 2, 3), FillOperation.REPLACE)
    blocks.fill(AIR, pos_local(0, 0, 3), pos_local(0, 1, 3), FillOperation.REPLACE)
    blocks.place(OAK_DOOR, pos_local(0, 0, 3))
    blocks.fill(AIR, pos_local(3, 1, 5), pos_local(3, 2, 6), FillOperation.REPLACE)
    blocks.fill(AIR, pos_local(-3, 1, 5), pos_local(-3, 2, 6), FillOperation.REPLACE)

player.on_chat("domek", zbuduj_domek)
```

Sześć ścian, po kolei w kodzie:

1. Podłoga: deski dębowe, na ziemi przed tobą.
2. Sufit: deski świerkowe.
3. Tył: cegły kamienne.
4. Lewa ściana: deski brzozowe. Potem dziura z `AIR`.
5. Prawa ściana: piaskowiec. Też dziura z `AIR`.
6. Przód: cegły. W środku drzwi `OAK_DOOR`.

`AIR` to powietrze. Okna na razie są dziurami, nie szkłem.

## Jak uruchomić

1. Stań na płaskim miejscu. Popatrz tam, gdzie ma stanąć przód domku.
2. Otwórz Code Builder przyciskiem C. Wklej kod. Naciśnij zielony start.
3. Wróć do gry. Naciśnij T, wpisz `domek` i naciśnij Enter.

Wejdź przez drzwi. Po lewej i po prawej zobaczysz otwory.

## Domek ze zmiennymi

Ten sam domek, ale rozmiar jest w trzech pudełkach. Zmieniasz liczby na górze, a ściany, drzwi i okna same się przesuwają.

- `szer` to ile bloków w lewo i w prawo od środka. Przy `3` domek ma ściany na `-3` i `3`.
- `wys` to wysokość ścian. Sufit jest jeden blok wyżej.
- `glebokosc` to głębokość, ile bloków do przodu.

Zostaw `szer` co najmniej 2, `wys` co najmniej 3, `glebokosc` co najmniej 4. Inaczej drzwi albo okno wejdą w róg.

Wklej to obok poprzedniego kodu albo zamiast niego. Komenda jest inna: `domek2`.

```python
def zbuduj_domek2():
    szer = 3
    wys = 3
    glebokosc = 6
    przod = 3
    tyl = przod + glebokosc - 1
    srodek = przod + glebokosc // 2
    blocks.fill(PLANKS_OAK, pos_local(-szer, -1, przod), pos_local(szer, -1, tyl), FillOperation.REPLACE)
    blocks.fill(PLANKS_SPRUCE, pos_local(-szer, wys, przod), pos_local(szer, wys, tyl), FillOperation.REPLACE)
    blocks.fill(STONE_BRICKS, pos_local(-szer, 0, tyl), pos_local(szer, wys - 1, tyl), FillOperation.REPLACE)
    blocks.fill(PLANKS_BIRCH, pos_local(szer, 0, przod), pos_local(szer, wys - 1, tyl), FillOperation.REPLACE)
    blocks.fill(SANDSTONE, pos_local(-szer, 0, przod), pos_local(-szer, wys - 1, tyl), FillOperation.REPLACE)
    blocks.fill(BRICKS, pos_local(-szer, 0, przod), pos_local(szer, wys - 1, przod), FillOperation.REPLACE)
    blocks.fill(AIR, pos_local(0, 0, przod), pos_local(0, 1, przod), FillOperation.REPLACE)
    blocks.place(OAK_DOOR, pos_local(0, 0, przod))
    blocks.fill(AIR, pos_local(szer, 1, srodek - 1), pos_local(szer, wys - 1, srodek), FillOperation.REPLACE)
    blocks.fill(AIR, pos_local(-szer, 1, srodek - 1), pos_local(-szer, wys - 1, srodek), FillOperation.REPLACE)

player.on_chat("domek2", zbuduj_domek2)
```

`przod` to 3, żeby domek nie stanął na tobie. `tyl` to ostatni blok w głąb. `//` to dzielenie bez reszty: `6 // 2` daje `3`. Od tego jest środek bocznej ściany, tam jest okno.

Żeby dostać większy domek, zmień tylko `szer`, `wys` albo `glebokosc`. Potem znowu wpisz `domek2`. Odsuń się, bo nowy domek stanie w tym samym miejscu.
