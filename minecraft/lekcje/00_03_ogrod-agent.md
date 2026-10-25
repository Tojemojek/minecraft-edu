# Płot z agentem

Tak, da się to zrobić agentem. Agent to pomocnik w grze. Ma własny nos.

Kod z `pos` stawia słupki względem ciebie. Jak poruszysz myszką, kierunek się obraca i płot wychodzi krzywo. Agent po starcie już się tak nie obraca. Możesz ruszać myszką.

Popatrz w stronę dłuższego boku, zanim wpiszesz komendę. Potem agent idzie sam.

## Kod

Wklej to w Code Builderze zamiast poprzedniego programu. Nie uruchamiaj go przez `python3`. Zostaw wcięcia.

```python
def zbuduj_ogrod():
    szerokosc = 15
    dlugosc = 10
    agent.teleport_to_player()
    agent.set_assist(PLACE_ON_MOVE, False)
    agent.move(FORWARD, 3)
    agent.set_item(OAK_FENCE, 64, 1)
    agent.set_slot(1)
    agent.set_assist(PLACE_ON_MOVE, True)
    for krok in range(2):
        agent.move(FORWARD, szerokosc)
        agent.turn(TurnDirection.LEFT)
        agent.move(FORWARD, dlugosc)
        agent.turn(TurnDirection.LEFT)
    agent.set_assist(PLACE_ON_MOVE, False)

player.on_chat("ogrod", zbuduj_ogrod)
```

`szerokosc` i `dlugosc` to dwa pudełka na liczby. Agent stawia jeden słupek na każdy krok. Idzie 15 kroków, skręca w lewo, idzie 10 kroków, skręca. Pętla robi tę parę boków dwa razy. Wychodzi prostokąt.

`set_item` wkłada 64 słupki do plecaka agenta. Plecak to miejsce na przedmioty. 64 wystarczy na cały płot. Ostatnia linia wyłącza stawianie, żeby agent nie budował przy następnym kroku.

## Jak uruchomić

1. Stań na płaskim, pustym miejscu. Popatrz tam, gdzie ma iść bok z 15 słupków.
2. Otwórz Code Builder przyciskiem C. Wklej kod. Naciśnij zielony start.
3. Wróć do gry. Naciśnij T, wpisz `ogrod` i naciśnij Enter.
4. Zostań w miejscu i patrz. Agent buduje sam.
