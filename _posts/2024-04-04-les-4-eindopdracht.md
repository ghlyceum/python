---
title: "4: Eindopdracht"
description: Alles goede dingen komen tot een einde😔!

date: 2024-04-02 01:00:00 +0100
categories: [Lessen]
tags: []
pin: true
math: true
mermaid: true
---



## Eindopdracht
We zijn nu aangekomen bij de eindopdracht!
In de eindopdracht zullen we alle kennis van de 3 hoofdstukken combineren.
Om de eindopdracht een beetje leuk te maken, zijn er ook 3 verschillende opties.
Elke opdracht is op een ander niveau, 1 is het makkelijkste terwijl 3 de moeilijkste is.
**Mijn advies: daag jezelf uit! Je zult veel kennis leren terwijl je bezig bent en ik garandeer je dat je alle niveau's aankan.**


## Niveau 1: Monument
Bouw een monument na!
Insteek: Als je meer visueel bent ingesteld!


De Eiffeltoren is een gebouw in Parijs dat bekend is over de hele wereld. 
De toren is 330 meter lang en is meer dan 10 miljoen kilo. Het kost een fortuin om deze toren na te maken … tenzij je het in voxel game doet!

![Desktop View](/assets/img/eiffeltoren.jpg){: width="auto" height="auto" }


Het is aan jullie de beurt om een gebouw uit te kiezen en deze na te maken in Minetest. Er is echter 1 extra uitdaging... je mag geen blokjes met de hand plaatsen! 

### Stappenplan
De opdracht bestaat uit 4 stappen:

1. Kies een monument uit. Hier zijn twee criteria aan verbonden:
Het moet een gebouw zijn, dus geen landschappen, tuinen of meubels.
Het gebouw mag niet uit een enkele simpele vorm bestaan. Het mag dus niet een gebouw zijn dat alleen een kubus, piramide of een eenvoudig rechthoek is. Een voorbeeld zou de piramide van Gizeh zijn, omdat het om een enkele simpele vorm gaat. De Eiffeltoren mag weer wel omdat het bestaat uit verschillende vormen. De bedoeling is dat de keuze een uitdaging moet bieden.
2. In Miney, klik op start en maak een flat world aan.
3. Bouw je monument na. Hier zijn de volgende regels aan verbonden:
Je mag geen blokjes met de hand plaatsen. Na het inleveren zal ik de code op mijn computer draaien, dus deze zullen dan überhaupt niet meekomen.
Het is niet de bedoeling dat je een gebouw maakt door zelf handmatig x, y, z locaties mee te geven, je bent dan heel lang bezig. Denk na hoe je dit kan doen door middel van loops en lijsten.
Je maakt bovenaan je programma een lijst aan met alle type blokjes die komen. Bijvoorbeeld als je alleen steen, glas en zand gaat gebruiken, verwacht ik bovenaan dus `blokken = ["stone", "glass", "sand"]`. Als je een blokje wilt ophalen, moet je deze uit de lijst halen o.b.v. de index. Zie de les over lijsten als je even vergeten bent hoe dit moet.
Je gebouw moet uit minimaal 250 blokjes bestaan.
4. Schijf het verslag. Zie hieronder wat de criteria daaraan zijn.

### Verslag:
- Voorpagina met je naam, klas, naam van het monument en de datum waarop het document is aangemaakt.
- Toelichting van je keuze voor monument (max. 200 woorden)
- Foto van het monument zoals het in de echte wereld eruit ziet.
- Foto van je creatie
- Uitleg hoe het programma in elkaar licht hierin toe hoe je kenmerken van het monument hebt gemaakt en wat voor constructies (for loops, if statements en lijsten) je hierin ziet (max. 500 woorden).
- Toelichting hoe het ontwikkelproces verliep, hierin verwacht ik te zien wat je uitdagingen waren, wat makkelijk was en wat je hebt geleerd (max. 400 woorden).


## Niveau 2: Huis
Kies een plek en bouw een huis.
Insteek: Een algoritmische invalshoek

De uitdaging bij deze opdracht is om een huisje te plaatsen, helaas kan je niet altijd dezelfde plek kiezen, dus zul je een algoritme maken die het kan. Het eindresultaat is dus een huisje gebouwd op een ideale locatie.

#### Voorbeeldalgoritme
Een voorbeeldalgoritme ziet er als volgt uit:
- Ik wil een huisje naast het water hebben, dus maximaal 5 blokken verwijdert van een water blok.
- Ik wil een huisje hebben in de buurt van bos, dus maximaal 10 blokken verwijdert van meerdere hout blokken.
- Ik wil een huisje hebben dat zich bevind in een vlak terrein, dus met een bereik van 5 blokjes wil ik dat alle blokjes dezelfde hoogte hebben.
- Ik wil dat mijn huisje op zand wordt gebouwd.
- Ik wil dat er genoeg plek is voor mijn huisje.

Om zo een zoekalgoritme te bouwen, moet je de volgende stappen ondernemen:
- Pak alle blokjes die je kan vinden
- Filter alle blokjes die niet zand zijn.
- Kijk bij elk blokje zand of de omgeving voldoet aan de criteria.

Maak nu je eigen zoekalgoritme! Bepaal zelf de criteria dus neem niet de bovenstaande over.

### Stappenplan
1. Maak een simpel huis in Minetest door middel van Python code. Het huis moet uit minder 100 blokjes bestaan.
2. Bedenk wat voor criteria je stelt aan de omgeving
3. Bouw je zoekalgoritme om de criteria te vinden.
4. Schrijf het verslag, hieronder de criteria.


### Verslag
- Voorpagina met je naam, klas en de datum waarop het document is aangemaakt.
- Toelichting wat voor criteria je aan je zoekalgoritme stelt (max. 200 woorden)
- Foto van je huisje in een ideal scenario.
- Uitleg hoe het programma in elkaar licht hierin toe hoe je kenmerken van het monument hebt gemaakt en wat voor constructies (for loops, if statements en lijsten) je hierin ziet (max. 500 woorden).
- Toelichting hoe het ontwikkelproces verliep, hierin verwacht ik te zien wat je uitdagingen waren, wat makkelijk was en wat je hebt geleerd (max. 400 woorden).



## Niveau 3: Stad
Deze opgave zit iets anders in elkaar dan de andere 2.
Bij deze opdracht ga je de [__The City Renaissance Challenge for Minecraft__](https://grzi.github.io/city-renaissance-challenge-minecraft/) volgen. Hierin zal je leren hoe je een stad moet bouwen, als opdracht zul je de taken uitvoeren alleen doormiddel van Python code. De opdracht is als volgt:
- In plaats van blokjes bouwen is je doel om dit te doen doormiddel van Python code.
- Bouw tot en met stap 11. Stap 9 mag je overslaan.
- Minetest en Minecraft zijn iets anders, hierdoor zullen sommige taken niet mogelijk zijn, deze mag je dan ook overslaan.
- Treasure chest taken mag je overslaan.
- Dieren plaatsen mag je overslaan.
- Schrijf het bijbehorende verslag.

### Verslag
- Voorpagina met je naam, klas en de datum waarop het document is aangemaakt.
- Foto van je stad
- Uitleg hoe het programma in elkaar licht hierin toe hoe je kenmerken van het monument hebt gemaakt en wat voor constructies (for loops, if statements en lijsten) je hierin ziet (max. 500 woorden).
- Toelichting hoe het ontwikkelproces verliep, hierin verwacht ik te zien wat je uitdagingen waren, wat makkelijk was en wat je hebt geleerd (max. 400 woorden).
