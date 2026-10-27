# Płot szeroki na 15 i długi na 10

Płot z pierwszej lekcji był jedną linią. Teraz zamykasz prostokąt: 15 bloków w bok i 10 bloków do przodu.

Jak poruszysz myszką w trakcie budowania, ten płot może wyjść krzywo. 

## Dwie zmienne

Zmienna to pudełko na liczbę. Teraz są dwa pudełka.

- `szerokosc` to 15. Tyle słupków ma bok w lewo i w prawo.
- `dlugosc` to 10. Tyle słupków ma bok do przodu.

## Cztery boki

Prostokąt ma cztery boki. Dwie pętle wystarczą: pierwsza stawia dwa długie boki, druga dwa krótkie.

Ostatni słupek stoi o jeden mniej niż liczba w pudełku, bo liczenie zaczyna się od zera. Przy szerokości 15 ostatnie miejsce to `szerokosc - 1`, czyli 14.

## Kod

Wklej to pod poprzednim programem. Zostaw wcięcia.

```python
def zbuduj_ogrod():
    szerokosc = 15
    dlugosc = 10
    for krok in range(szerokosc):
        blocks.place(OAK_FENCE, pos(krok, 0, 2))
        blocks.place(OAK_FENCE, pos(krok, 0, 2 + dlugosc - 1))
    for krok in range(dlugosc):
        blocks.place(OAK_FENCE, pos(0, 0, 2 + krok))
        blocks.place(OAK_FENCE, pos(szerokosc - 1, 0, 2 + krok))

player.on_chat("ogrod", zbuduj_ogrod)
```

`OAK_FENCE` to ten sam płot z dębu.

## Jak uruchomić

1. Stań na płaskim miejscu. Popatrz tam, gdzie ma iść dłuższy bok.
2. Otwórz Code Builder przyciskiem C. Wklej kod. Naciśnij zielony start.
3. Wróć do gry. Naciśnij T, wpisz `ogrod` i naciśnij Enter.

Obok ciebie stanie prostokątny płot: 15 bloków szerokości i 10 bloków długości.
