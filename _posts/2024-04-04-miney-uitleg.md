---
title: "Miney FAQ"
description: "Hoe moet dat ook alweer?"

date: 2024-04-04 02:00:00 +0100
categories: [ Hulpbronnen ]
tags: [ ]
pin: false
math: true
mermaid: true
---

## Miney FAQ

### Hoe kom ik achter de positie van de speler?
__Trefwoorden: `Positie`, `Coördinaten`, `Locatie`__ \
Als je op ``F5`` drukt, dan zie je linksbovenin informatie over de wereld.
Specifiek zie je de x, y en z coördinaten van de speler, deze staan onder `pos(x,y,z)`.
**Je zult hier echter wel gehele getallen van moeten maken**.

![Desktop View](/assets/img/dev/positie.png){: width="auto" height="auto" }

### Welke blokjes kan ik allemaal plaatsen?
__Trefwoorden: `Blok`, `Type`__ \
Als je opzoek bent naar een specifiek blokje, kan je het beste de [Minetest wiki](https://wiki.minetest.net/Games/Minetest_Game/Nodes) raadplegen.
Hier staan alle blokjes die je kan plaatsen in Miney. Je zult dan op de pagina van een blokje moeten zoeken naar de naam van het blokje.
De naam van het blokje is de naam die je moet gebruiken in een functie. De naam is te vinden onder `Itemstring`.
![Desktop View](/assets/img/dev/wiki_item.png){: width="auto" height="auto" }


### Hoe maak ik een platte wereld aan?
__Trefwoorden: `Wereld`, `Flat`, `Plat`__ \

Begin bij het opstarten van Miney doormiddel van de Miney launcher, klik op Start Minetest
![Desktop View](/assets/img/dev/start.png){: width="auto" height="auto" }

Klik op nieuw om een nieuwe wereld aan te maken
![Desktop View](/assets/img/dev/nieuw.png){: width="auto" height="auto" }


Vul de naam van je nieuwe wereld bovenaan in, je mag deze zelf kiezen naar wens.
Selecteer bij Wereldgenerator **flat**.
![Desktop View](/assets/img/dev/opslaan.png){: width="auto" height="auto" }

Vink de opties aan de zijkant uit
![Desktop View](/assets/img/dev/vink uit.png){: width="auto" height="auto" }

Klik op opslaan!
![Desktop View](/assets/img/dev/starten.png){: width="auto" height="auto" }


Start je zelf gekozen wereld!
![Desktop View](/assets/img/dev/spelen.png){: width="auto" height="auto" }


