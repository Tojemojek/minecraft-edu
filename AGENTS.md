# minecraft-edu

Materiały do nauki dla dzieci w wieku 9–12 lat. To nie jest mod, plugin ani serwer Minecrafta.

## Po co jest to repozytorium

Dzieci uczą się tu trzech rzeczy, osobno i po kolei:

1. obsługi komputera
2. czystego Pythona
3. Pythona w Minecraft Education (Code Builder / MakeCode Python)

W repozytorium są pliki `.md`: instrukcje albo przykładowe listingi. Nie produkujemy gry, biblioteki ani aplikacji.

## Dla kogo piszemy

Uczeń ma 9–12 lat i zwykle nie programował wcześniej. Pisz po polsku, krótko, konkretnie, jednym nowym pomysłem na raz. Tłumacz słowa takie jak zmienna, pętla, plik, folder. Bez żargonu, sarkazmu i straszenia.

Minecraft, Education Edition i MakeCode to marki Microsoftu. Piszemy własne materiały. Nie kopiujemy lekcji, tutoriali ani dokumentacji Microsoftu.

## Trzy ścieżki — nie mieszaj ich

- `komputer/` — pliki, foldery, klawiatura, kopiowanie, zapisywanie, uruchamianie programu, otwarcie Minecraft Education i Code Buildera.
- `python/` — zwykły Python 3, bez gry. Ma dać się uruchomić lokalnie: `python3 plik.py`.
- `minecraft/` — Python z Code Buildera. Działa w grze, nie jako skrypt systemowy. Nie używaj tu `pip`, pygame, mcpi, Spigot, Paper, Forge ani Fabric.

W `minecraft/` trzymaj lekcje w `lekcje/`, krótkie listingi w `przyklady/`, a katalogi bloków w `bloki/`. To też pliki `.md`. Nie zakładaj całego drzewa z góry — twórz katalog, gdy powstaje pierwsza lekcja.

## Python w Minecraft Education

API to MakeCode Python z Code Buildera (`player`, `agent`, `blocks`, `mobs`, `builder`), nie Python z Raspberry Pi (`mcpi`).

Zanim podasz nazwę bloku, moba albo funkcji, sprawdź ją w dokumentacji albo w istniejących listach w `minecraft/bloki/`. Nie wymyślaj identyfikatorów. Lista bloków to nazwa używana w kodzie, po polsku do czego służy i w której lekcji się pojawia.

Przykład uruchamia uczeń w Code Builderze, nie poleceniem `python3`, chyba że lekcja jest w `python/`.

## Jak pisać plik `.md`

Jeden plik = jeden mały cel. Najpierw obsługa komputera i czysty Python, potem ten sam pomysł w Minecrafcie.

W pliku jest opis: co zrobić i jak, krok po kroku. Listing kodu wklej w tym samym pliku, w bloku kodu — nie jako osobny program. Czysty Python ma dać się skopiować i odpalić przez `python3`. Kod z gry uruchamia się w Code Builderze; nie udawaj, że przeszedł lokalnie.

Gdy krok polega na kliknięciu, wstaw obok obrazek, który pokazuje gdzie kliknąć. Obrazek leży przy tym pliku `.md`, a w tekście: `![Gdzie kliknąć: krótki opis](nazwa.png)`. Nazwa pliku mówi, co widać. Nie odwołuj się do obrazka, którego nie ma w repo. Tekst ma dać się zrobić także bez obrazka.

Nie zbieraj danych dzieci. Nie dawaj zadań z danymi osobowymi, hasłami ani treścią nie dla tego wieku. Nie dokładaj frameworków, zależności ani konfiguracji projektu.
