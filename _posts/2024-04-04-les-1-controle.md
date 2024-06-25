---
title: '1.2: Condities!'
description: Wanneer iets mag en wanneer niet.

date: 2024-04-08 06:00:00 +0100
categories: [Lessen]
tags: [ ]
pin: true
math: true
mermaid: true
---

## Controle
Controle structuur passen we toe als we taken willen uitvoeren die conditioneel zijn.
Conditioneel betekent, als er een regel gebonden is aan de operatie. Denk bijvoorbeeld aan de regels die we hebben op school. Je mag met elkaar praten tijdens de pauze, maar niet tijdens de toets.
Het is dus conditioneel of je met elkaar mag praten.

## Voorbeeld teken app
In de teken app hebben we al gewerkt met conditionele operaties. Bijvoorbeeld de opdracht over de pennen.
De opdracht was als volgt: De prijs van pennen met opdruk is €0,97 per stuk, maar bij aankoop van 500 pennen of meer daalt de prijs naar €0,89.
In de teken app zag dat er als volgt uit:

![Desktop View](/assets/img/les1/Pennen.png){: width="auto" height="auto" }

Laten we dit even vertalen naar een python code.

```python
prijs = 0
aantal_pennen = 10
if aantal_pennen > 500:
    prijs = 0.89 * aantal_pennen
else:
    prijs = 0.97 *aantal_pennen
print(prijs)
```

Wat valt je op als je naar deze code kijkt? Noteer het even!

Een aantal van mijn observaties zijn:
- ``Als`` wordt vervangen door ``if``, dat is niet heel gek, want dat is de vertaling.
- ``Anders`` wordt vervangen door ``else``, wederom is dat de vertaling.
- De code is georganiseerd door inspringing, dit is om aan te geven dat de code binnen iets hoort.
- De code beschikt over een dubbele punt, dit is om aan te geven dat er een conditie klaar is.
\
Verder is de code grotendeels gelijk, dit betekent dus dat de kennis die je al hebt, goed vertaalbaar is naar Python!

# If en Else
Deze kernwoorden, if en else, zijn de basis van de controle structuur in Python.
Wederom zie je dat we gebruiken maken van de dubbele punt en de inspringing. Dit is om aan te geven dat de code binnen de if of else hoort.
Laten we even wat nauwkeuriger kijken naar een ``if`` en ``else`` conditie kijken.

```python
if aantal_pennen > 500:
```
De regel is op te splitsen in de volgende delen:
- ``if``: Dit is de start van de conditie, dit betekent letterlijk als.
- ``aantal_pennen > 500``: Dit is de conditie, als deze conditie waar is, dan wordt de code binnen de if uitgevoerd.
- ``:``: Dit is de afsluiting van de conditie, dit betekent dat de conditie af is.

Laten we nu even kijken naar de ``else``.

```python
else:
```

We zien hier dat de regel op te splitsen is in 2 delen:
- ``else``: Dit is de start van de else conditie, dit betekent letterlijk anders.
- ``:``: Dit is de afsluiting van de else conditie en dat de bijbehorende code begint.

Wat nou als we meerdere condities willen doen?

# Elif
Laten we even een voorbeeld situatie pakken.
2 kaasstengels bij de Hoogvliet zijn €0,58, maar als je er 2 koopt, dan is de prijs 50 cent per stuk.
De Hoogvliet wilt echter niet dat mensen meer dan twee kopen, want dan is er niet genoeg voor iedereen, ze besluiten daarom om de korting niet meer toe te passen na 2 kaasstengels.
Laten we dit even vertalen naar Python.

```python
if aantal_kaasstengels == 1:
  prijs = 0.58
elif aantal_kaasstengels == 2:
  prijs = 1
else:
  prijs = (0.58 * aantal_kaasstengels-2) + 1
```

Met deze code kunnen we de prijs berekenen van de kaasstengels.
De elif geeft ons dus nog een situatie of scenario om af te vangen in onze code.

Genoeg gepraat! Laten we even wat opdrachten maken!


## Deel 2 - Controle
Deze opdrachten gaan over het maken van basis condities.
Je kunt deze opdrachten maken op de [online omgeving van Python](https://www.mycompiler.io/nl/new/python){:target="_blank"}

```python

# Opdracht 1: Bepaal of een getal positief of negatief is.
# Maak een functie die achterhaald of een getal positief of negatief is.
# Noem de functie positief_negatief
# De functie heeft 1 paramater, het getal.
# Als het getal positief is mag je de waarde 1 terug geven, als het getal negatief is mag je de waarde -1 terug geven.

# Opdracht 2: Bepaal of een getal positief, negatief of nul is.
# Maak een functie die achterhaald of een getal positief, negatief of nul is.
# Noem de functie positief_negatief_nul
# De functie heeft 1 paramater, het getal.
# Als het getal positief is mag je de waarde 1 terug geven, als het getal negatief is mag je de waarde -1 terug geven.
# Als het getal nul is mag je de waarde 0 terug geven.

# Opdracht 3: Grootste getal.
# Maak een functie die achterhaald welke van de 2 getallen groter is.
# Noem de functie groter
# De functie heeft 2 paramaters, a en b.
# Geef het grootste getal terug. Als de getallen dezelfde waarde hebben mag je 1 van de 2 kiezen.
# Je mag er vanuit gaan dat beide getallen boven de nul zijn.

# Opdracht 4: Bereik
# Maak een functie die achterhaald of een getal binnen het bereik is van 2 andere getallen.
# Noem de functie bereik
# De functie heeft 3 paramaters, minimum, maximum, getal
# Als het getal binnen het bereik is mag je de waarde 1 terug geven, als het buiten het bereik ik mag je een 0 terug geven.

# Opdracht 5: Beide getallen in het bereik
# Maak een functie die achterhaald of twee getallen binnen het bereik is van 2 andere getallen.
# Noem de functie dubbel_bereik
# De functie heeft 4 paramaters, minimum, maximum, getal_a en getal_b
# Als beide getallen binnen het bereik zijn mag je de waarde 2 terug geven.
# Als 1 van ze in het bereik is mag je 1 terug geven.
# Als geen van ze binnen het bereik is geef je 0 terug.

# EXTRA
# Opdracht 6: Van score naar getal
# Maak een functie die een score binnen krijgt en deze moet omrekenen naar een aantal punten.
# Noem de functie score_naar_getal
# De functie krijgt 1 paramater, score.
# Een score tussen 90 en 100 krijgt 10 punten
# Een score tussen 80 en 89 krijgt 8 punten
# Een score tussen 70 en 79 krijgt 6 punten
# Een score tussen 60 en 69 krijgt 4 punten
# Een score onder 60 of boven de 100 krijgt 0 punten

# EXTRA
# Opdracht 7: Ledenkorting
# We hebben een winkel en we willen graag onze loyale leden, Ledenkorting geven.
# We hebben 4 niveaus voor ledenkorting:
# Niveau 0: 0% ledenkorting
# Niveau 1: 10% ledenkorting
# Niveau 2: 20% ledenkorting
# Niveau 3: 30% ledenkorting
# Maak een functie, leden_prijs_berekenen
# De functie krijgt 2 paramaters mee, het niveau (0,1,2,3) en de prijs van het artikel.
# Bereken dan de uiteindelijke prijs (prijs-korting) die het lid moet betalen.

# EXTRA
# Opdracht 8: Beperkte ledenkorting
# Ons ledenkortingsysteem van hiervoor werkte geweldig! Alleen nu is er een nieuwe regel. Je ledenkorting gaat pas in als de prijs van het artikel voor de 100 euro is.
# Maak een nieuwe functie aan genaamd beperkte_leden_prijs_berekenen, kopieer je code van de vorige opgave hierin en voeg de limitatie van 100 euro er aan toe.
# Bereken dan de uiteindelijke prijs (prijs-korting) die het lid moet betalen.

```
Als dit is gelukt dan ben je klaar met de controle opdrachten.
Ga nu verder met het een-na-laatste deel van de python lesstof, de [variabelen](https://brandonkroes.com/python/posts/les-1-variabelen/).

