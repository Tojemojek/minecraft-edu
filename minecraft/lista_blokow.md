# Nazwy bloków w kodzie

W Minecraft Education, w Pythonie z Code Buildera, blok zapisujesz wielkimi literami, na przykład `GRASS`,
`DIAMOND_BLOCK`, `STONE`.

Jeśli nazwa nie działa, sprawdź ją w autouzupełnianiu Code Buildera.

## Jak używać

```python
blocks.place(DIAMOND_BLOCK, pos_local(0, 0, 0))
blocks.fill(GRASS, pos_local(0, 0, 0), pos_local(10, 0, 10))
```

`pos_local` jest łatwiejsze niż `pos`. Liczy od tego, w którą stronę patrzysz: pierwsza liczba w lewo, druga w górę,
trzecia do przodu. `pos` liczy wschód i północ. Tego nie widać.

## Podstawowe

| nazwa w kodzie     | co to jest                                   |
|--------------------|----------------------------------------------|
| `AIR`              | powietrze, puste miejsce                     |
| `STONE`            | kamień                                       |
| `GRASS`            | ziemia z trawą na wierzchu                   |
| `DIRT`             | ziemia                                       |
| `COBBLESTONE`      | bruk, kamienie z kopania                     |
| `SAND`             | piasek                                       |
| `GRAVEL`           | żwir                                         |
| `BEDROCK`          | skała na dnie świata, nie da się jej wykopać |
| `WATER_FLOWING`    | płynąca woda                                 |
| `WATER_STATIONARY` | stojąca woda                                 |
| `LAVA_FLOWING`     | płynąca lawa                                 |
| `LAVA_STATIONARY`  | stojąca lawa                                 |
| `GLASS`            | szkło                                        |
| `GLOWSTONE_BLOCK`  | świecący kamień                              |
| `OBSIDIAN`         | obsydian, bardzo twardy czarny blok          |
| `SNOW`             | cienka warstwa śniegu                        |
| `SNOW_BLOCK`       | cały blok śniegu                             |
| `ICE`              | lód                                          |
| `CLAY`             | glina                                        |
| `MOSS_STONE`       | kamień z mchem                               |
| `BRICK_BLOCK`      | cegły                                        |
| `STONE_BRICK`      | cegły z kamienia                             |
| `BOOKSHELF`        | półka z książkami                            |
| `CRAFTING_TABLE`   | stół do robienia przedmiotów                 |
| `FURNACE_ACTIVE`   | piec, który się pali                         |
| `FURNACE_INACTIVE` | piec, wyłączony                              |
| `CHEST`            | skrzynia                                     |
| `TNT`              | dynamit                                      |
| `TORCH`            | pochodnia                                    |
| `LADDER`           | drabina                                      |
| `FENCE`            | płot                                         |
| `FENCE_GATE`       | furtka w płocie                              |
| `CACTUS`           | kaktus                                       |
| `SUGAR_CANE`       | trzcina cukrowa                              |
| `FARMLAND`         | zaorane pole                                 |

## Rudy i bloki surowców

| nazwa w kodzie          | co to jest                    |
|-------------------------|-------------------------------|
| `COAL_ORE`              | ruda węgla                    |
| `IRON_ORE`              | ruda żelaza                   |
| `GOLD_ORE`              | ruda złota                    |
| `DIAMOND_ORE`           | ruda diamentu                 |
| `EMERALD_ORE`           | ruda szmaragdu                |
| `LAPIS_LAZULI_ORE`      | ruda niebieskiego kamienia    |
| `REDSTONE_ORE`          | ruda czerwonego kamienia      |
| `NETHER_QUARTZ_ORE`     | ruda kwarcu z gorącego świata |
| `COAL_BLOCK`            | blok węgla                    |
| `IRON_BLOCK`            | blok żelaza                   |
| `GOLD_BLOCK`            | blok złota                    |
| `DIAMOND_BLOCK`         | blok diamentu                 |
| `EMERALD_BLOCK`         | blok szmaragdu                |
| `LAPIS_LAZULI_BLOCK`    | blok niebieskiego kamienia    |
| `REDSTONE_BLOCK`        | blok czerwonego kamienia      |
| `QUARTZ_BLOCK`          | blok kwarcu                   |
| `QUARTZ_BLOCK_CHISELED` | rzeźbiony blok kwarcu         |

## Drewno, liście, deski

| nazwa w kodzie              | co to jest                              |
|-----------------------------|-----------------------------------------|
| `WOOD`                      | pień dębu                               |
| `WOOD_PLANKS_OAK`           | deski dębowe                            |
| `WOOD_PLANKS_BIRCH`         | deski brzozowe                          |
| `WOOD_PLANKS_SPRUCE`        | deski świerkowe                         |
| `WOOD_PLANKS_JUNGLE`        | deski z drzewa tropikalnego             |
| `WOOD_PLANKS_ACACIA`        | deski z akacji                          |
| `WOOD_PLANKS_DARK_OAK`      | deski z ciemnego dębu                   |
| `ACACIA_WOOD`               | pień akacji                             |
| `BIRCH_WOOD`                | pień brzozy                             |
| `DARK_OAK_WOOD`             | pień ciemnego dębu                      |
| `JUNGLE_WOOD`               | pień drzewa tropikalnego                |
| `SPRUCE_WOOD`               | pień świerku                            |
| `LEAVES_OAK_PERMANENT`      | liście dębu, nie znikają                |
| `LEAVES_BIRCH_PERMANENT`    | liście brzozy, nie znikają              |
| `LEAVES_SPRUCE_PERMANENT`   | liście świerku, nie znikają             |
| `LEAVES_JUNGLE_PERMANENT`   | liście drzewa tropikalnego, nie znikają |
| `LEAVES_ACACIA_PERMANENT`   | liście akacji, nie znikają              |
| `LEAVES_DARK_OAK_PERMANENT` | liście ciemnego dębu, nie znikają       |
| `SAPLING`                   | sadzonka dębu                           |
| `SAPLING_BIRCH`             | sadzonka brzozy                         |
| `SAPLING_SPRUCE`            | sadzonka świerku                        |
| `SAPLING_JUNGLE`            | sadzonka drzewa tropikalnego            |
| `SAPLING_ACACIA`            | sadzonka akacji                         |
| `SAPLING_DARK_OAK`          | sadzonka ciemnego dębu                  |

## Kolory: wełna, szkło, terakota

Zwykła terakota bez koloru to `HARDENED_CLAY` — wypalona glina.

| nazwa w kodzie                     | co to jest                       |
|------------------------------------|----------------------------------|
| `WOOL_WHITE`                       | biała wełna                      |
| `WOOL_ORANGE`                      | pomarańczowa wełna               |
| `WOOL_MAGENTA`                     | wełna w kolorze magenta          |
| `WOOL_LIGHT_BLUE`                  | jasnoniebieska wełna             |
| `WOOL_YELLOW`                      | żółta wełna                      |
| `WOOL_LIME`                        | limonkowa wełna                  |
| `WOOL_PINK`                        | różowa wełna                     |
| `WOOL_GRAY`                        | szara wełna                      |
| `WOOL_LIGHT_GRAY`                  | jasnoszara wełna                 |
| `WOOL_CYAN`                        | wełna w kolorze cyjan            |
| `WOOL_PURPLE`                      | fioletowa wełna                  |
| `WOOL_BLUE`                        | niebieska wełna                  |
| `WOOL_BROWN`                       | brązowa wełna                    |
| `WOOL_GREEN`                       | zielona wełna                    |
| `WOOL_RED`                         | czerwona wełna                   |
| `WOOL_BLACK`                       | czarna wełna                     |
| `STAINED_GLASS_WHITE`              | białe szkło                      |
| `STAINED_GLASS_ORANGE`             | pomarańczowe szkło               |
| `STAINED_GLASS_MAGENTA`            | szkło w kolorze magenta          |
| `STAINED_GLASS_LIGHT_BLUE`         | jasnoniebieskie szkło            |
| `STAINED_GLASS_YELLOW`             | żółte szkło                      |
| `STAINED_GLASS_LIME`               | limonkowe szkło                  |
| `STAINED_GLASS_PINK`               | różowe szkło                     |
| `STAINED_GLASS_GRAY`               | szare szkło                      |
| `STAINED_GLASS_LIGHT_GRAY`         | jasnoszare szkło                 |
| `STAINED_GLASS_CYAN`               | szkło w kolorze cyjan            |
| `STAINED_GLASS_PURPLE`             | fioletowe szkło                  |
| `STAINED_GLASS_BLUE`               | niebieskie szkło                 |
| `STAINED_GLASS_BROWN`              | brązowe szkło                    |
| `STAINED_GLASS_GREEN`              | zielone szkło                    |
| `STAINED_GLASS_RED`                | czerwone szkło                   |
| `STAINED_GLASS_BLACK`              | czarne szkło                     |
| `HARDENED_CLAY`                    | wypalona glina, bez koloru       |
| `HARDENED_CLAY_STAINED_WHITE`      | biała wypalona glina             |
| `HARDENED_CLAY_STAINED_ORANGE`     | pomarańczowa wypalona glina      |
| `HARDENED_CLAY_STAINED_MAGENTA`    | wypalona glina w kolorze magenta |
| `HARDENED_CLAY_STAINED_LIGHT_BLUE` | jasnoniebieska wypalona glina    |
| `HARDENED_CLAY_STAINED_YELLOW`     | żółta wypalona glina             |
| `HARDENED_CLAY_STAINED_LIME`       | limonkowa wypalona glina         |
| `HARDENED_CLAY_STAINED_PINK`       | różowa wypalona glina            |
| `HARDENED_CLAY_STAINED_GRAY`       | szara wypalona glina             |
| `HARDENED_CLAY_STAINED_LIGHT_GRAY` | jasnoszara wypalona glina        |
| `HARDENED_CLAY_STAINED_CYAN`       | wypalona glina w kolorze cyjan   |
| `HARDENED_CLAY_STAINED_PURPLE`     | fioletowa wypalona glina         |
| `HARDENED_CLAY_STAINED_BLUE`       | niebieska wypalona glina         |
| `HARDENED_CLAY_STAINED_BROWN`      | brązowa wypalona glina           |
| `HARDENED_CLAY_STAINED_GREEN`      | zielona wypalona glina           |
| `HARDENED_CLAY_STAINED_RED`        | czerwona wypalona glina          |
| `HARDENED_CLAY_STAINED_BLACK`      | czarna wypalona glina            |

## Rośliny i dekoracje

| nazwa w kodzie        | co to jest                     |
|-----------------------|--------------------------------|
| `DANDELION`           | żółty mlecz                    |
| `FLOWER_CYAN`         | niebieski kwiat                |
| `FLOWER_ALLIUM`       | fioletowy kwiat, czosnek       |
| `FLOWER_AZURE_BLUET`  | biały kwiatek                  |
| `FLOWER_BLUE_ORCHID`  | niebieska orchidea             |
| `FLOWER_OXEYE_DAISY`  | biały rumianek                 |
| `FLOWER_TULIP_ORANGE` | pomarańczowy tulipan           |
| `FLOWER_TULIP_PINK`   | różowy tulipan                 |
| `FLOWER_TULIP_RED`    | czerwony tulipan               |
| `FLOWER_TULIP_WHITE`  | biały tulipan                  |
| `SUNFLOWER`           | słonecznik                     |
| `LILAC`               | lilak, wysoki fioletowy krzew  |
| `PEONY`               | piwonia, wysoki różowy krzew   |
| `ROSE_BUSH`           | krzew róży                     |
| `FERN`                | paproć                         |
| `LARGE_FERN`          | duża paproć                    |
| `GRASS_TALL`          | wysoka trawa                   |
| `DOUBLE_TALLGRASS`    | bardzo wysoka trawa, dwa bloki |
| `DEADBUSH`            | suchy krzak                    |
| `MUSHROOM_BROWN`      | brązowy grzyb                  |
| `MUSHROOM_RED`        | czerwony grzyb                 |
| `MELON_BLOCK`         | arbuz                          |
| `PUMPKIN_INACTIVE`    | dynia                          |
| `PUMPKIN_ACTIVE`      | dynia z wyciętą twarzą, świeci |
| `CARROTS`             | marchewki na polu              |
| `POTATOES`            | ziemniaki na polu              |
| `WHEAT`               | pszenica                       |
| `BEETROOT`            | buraki                         |
| `COCOA_PLANT`         | kakao na pniu                  |
| `NETHER_WART`         | roślina z gorącego świata      |
| `WATERLILY`           | lilia wodna                    |
| `VINE`                | pnącze                         |

## Kamienie, piaskowce i Nether

Nether to gorący świat pod zwykłym światem. End to pusty, ostatni świat.

| nazwa w kodzie           | co to jest                    |
|--------------------------|-------------------------------|
| `STONE_GRANITE`          | granit, różowy kamień         |
| `STONE_GRANITE_SMOOTH`   | gładki granit                 |
| `STONE_DIORITE`          | dioryt, biały kamień w kropki |
| `STONE_DIORITE_SMOOTH`   | gładki dioryt                 |
| `STONE_ANDESITE`         | andezyt, szary kamień         |
| `STONE_ANDESITE_SMOOTH`  | gładki andezyt                |
| `SANDSTONE`              | piaskowiec                    |
| `SANDSTONE_CHISELED`     | rzeźbiony piaskowiec          |
| `SANDSTONE_SMOOTH`       | gładki piaskowiec             |
| `RED_SAND`               | czerwony piasek               |
| `RED_SANDSTONE`          | czerwony piaskowiec           |
| `RED_SANDSTONE_CHISELED` | rzeźbiony czerwony piaskowiec |
| `RED_SANDSTONE_SMOOTH`   | gładki czerwony piaskowiec    |
| `NETHERRACK`             | czerwony kamień z Netheru     |
| `NETHER_BRICK`           | cegły z Netheru               |
| `RED_NETHER_BRICK`       | czerwone cegły z Netheru      |
| `SOUL_SAND`              | piasek dusz, spowalnia        |
| `MAGMA`                  | blok magmy, parzy             |
| `END_STONE`              | kamień z Endu                 |
| `END_BRICKS`             | cegły z kamienia Endu         |
| `PURPUR_BLOCK`           | purpurowy blok z Endu         |
| `PURPUR_PILLAR`          | purpurowy filar z Endu        |
| `PRISMARINE`             | pryzmaryn, kamień z morza     |
| `PRISMARINE_BRICKS`      | cegły z pryzmarynu            |
| `PRISMARINE_DARK`        | ciemny pryzmaryn              |
| `SEA_LANTERN`            | morska latarnia, świeci       |
| `SLIME_BLOCK`            | blok szlamu, sprężysty        |
| `SPONGE`                 | gąbka, zbiera wodę            |
| `SPONGE_WET`             | mokra gąbka                   |
