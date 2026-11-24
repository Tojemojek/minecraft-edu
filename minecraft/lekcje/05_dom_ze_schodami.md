# Dom ze schodami

```python
lewa = 3
prawa = -3
przod = 3
tyl = 10
wysokosc = 5
okno_start = 4
okno_stop = 6
okno_wys_start = 1
okno_wys_stop = 3

def sciany():
    # boki
    blocks.fill(IRON_BLOCK, pos(lewa, 0, przod), pos(lewa, wysokosc, tyl), FillOperation.REPLACE)
    blocks.fill(DIAMOND_BLOCK, pos(prawa, 0, przod), pos(prawa, wysokosc, tyl), FillOperation.REPLACE)
    # przod
    blocks.fill(IRON_BLOCK, pos(lewa, 0, przod), pos(prawa, wysokosc, przod), FillOperation.REPLACE)
    # tyl
    blocks.fill(IRON_BLOCK, pos(lewa, 0, tyl), pos(prawa, wysokosc, tyl), FillOperation.REPLACE)

def drzwi():
    blocks.fill(AIR, pos(0, 0, przod), pos(0, 2, przod), FillOperation.REPLACE)
    blocks.place(OAK_DOOR, pos(0, 0, przod))

def okna():
    blocks.fill(BLUE_STAINED_GLASS, pos(lewa, okno_wys_start, okno_start), pos(lewa, okno_wys_stop, okno_stop), FillOperation.REPLACE)
    blocks.fill(RED_STAINED_GLASS, pos(prawa, okno_wys_start, okno_start), pos(prawa, okno_wys_stop, okno_stop), FillOperation.REPLACE)

def dach():
    blocks.fill(PLANKS_OAK, pos(lewa, wysokosc, przod), pos(prawa, wysokosc, tyl), FillOperation.REPLACE)

def schody2():
    agent.teleport(pos(0,0,0), SOUTH)
    agent.set_item(CHERRY_STAIRS, 64, 1)
    agent.set_slot(1)
    for j in range (4):
        for i in range (4):
            agent.place(FORWARD)
            agent.move(UP, 1)
            agent.move(FORWARD, 1)
        agent.turn(TurnDirection.LEFT)

def caly_dom():
    sciany();
    drzwi();
    okna();
    dach();
    schody2();


player.on_chat("dom", caly_dom)

```