```
def stopien(numer):
    blocks.place(PLANKS_OAK, pos(0, numer, 3 + numer))

def schody():
    for numer in range(6):
        stopien(numer)

player.on_chat("schody", schody)

```
