---
title: "IDLE uitleg"
description: "Uitleg hoe de editor IDLE werkt binnen Miney."

date: 2024-04-04 02:00:00 +0100
categories: [Ontwikkelomgeving]
tags: []
pin: false
math: true
mermaid: true
---



## IDLE
IDLE is de ontwikkelomgeving die standaard wordt meegegeven met Python.
Binnen IDLE kan je Python programma's schrijven en uitvoeren.
> Als je via Quickstart ben gestart, mag je stap 1 **overslaan**
{: .prompt-info }


## Werking
1. Als je binnen Miney Launcher klikt op start Pythons IDLE, dan zal IDLE worden opgestart.

![IDLE](/assets/img/dev/start idle.png){: width="auto" height="auto" }

2. Het ziet er dan als volgt uit:

![IDLE](/assets/img/dev/idle shell.png){: width="auto" height="auto" }

Hierin kan simpele python code worden geschreven en uitgevoerd, maar wij willen onze eigen programma's schrijven.
Daarom gaan we een nieuw bestand aanmaken.

1. Klik op `File` en vervolgens op `New File`.
![Aanmaken van een nieuw bestand.](/assets/img/dev/new file made.png){: width="auto" height="auto" }


2. Als het goed is krijg je dan het volgende scherm te zien:
![Leeg bestand](/assets/img/dev/new file.png){: width="auto" height="auto" }

3. We zullen nu dit bestand opslaan door op `File` en vervolgens op `Save As` te klikken.
![Leeg bestand](/assets/img/dev/save.png){: width="auto" height="auto" }
4. Kies een logische bestandsnaam en sla deze op in een map waar je het kan terugvinden.
5. Als je het bestand hebt opgeslagen, kan je het bestand uitvoeren door op `Run` en vervolgens op `Run Module` te klikken. 
Om niet elke keer met de muis erop hoeven te klikken, kan je ook op `F5` drukken.
![RUN](/assets/img/dev/run.png){: width="auto" height="auto" }

## Standaard code
Als je en project in Miney wilt gebruiken zul je de standaard code moeten toevoegen. De standaard code moet bovenaan het bestand zetten.
```python
import miney

def place_block(x, y, z, block_type):
    mt = miney.Minetest()
    mt.node.set({'x': x, 'y': y, 'z': z}, block_type)

def plaats_blok(x, y, z, block_type):
    place_block(x, y, z, block_type)

```
Als je het eenmaal erin hebt gezet ziet het er als volgt uit:
![Standaard code](/assets/img/dev/place_block.png){: width="auto" height="auto" }

