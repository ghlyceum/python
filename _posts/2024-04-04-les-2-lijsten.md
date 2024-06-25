---
title: "2: Lijsten"
description: Meer! Meer! Meer!

date: 2024-04-04 05:00:00 +0100
categories: [ Lessen ]
tags: [ ]
pin: true
math: true
mermaid: true
---
## Introductie
Deze les staat in het teken van het aanleren van lijsten in Python. Lijsten zijn een van de belangrijkste concepten in Python en hoe we meer dan 1 waarde kunnen opslaan in een variabele.
Het leerdoel voor vandaag is:

**Aan het einde van de les kan ik lijsten maken en op die lijsten kan ik waardes opvragen, waardes toevoegen, waardes verwijderen en waardes wijzigen.**

Lijsten zijn echter wel een compleet nieuw concept! Laten we beginnen met achterhalen waarom we lijsten gebruiken.
Als ik het woord lijst zeg, wat denk je dan? Een boodschappenlijstje!

Wat kunnen we vinden op een boodschappenlijstje? Een hoop producten, zoals:
- Appels
- Peren
- Bananen
- Brood
 
Dit is een lijst van producten die je wilt kopen in de supermarkt. Als we dan in de supermarkt zijn gaan we deze lijst af om te achterhalen of we alles hebben gevonden dat we nodig
hebben. Lijsten zijn dus een manier om meerdere dingen te onthouden en te gebruiken. In Python is dit niet anders, we kunnen een lijst maken van producten die we willen kopen.
Laten we een voorbeeld van een Python lijst pakken!

```python
boodschappenlijst = ["Appels", "Peren", "Bananen", "Brood"]
```

Laten we deze regel stap voor stap doornemen:

- We beginnen met de variabele naam, in dit geval is dat `boodschappenlijst`.
- We gebruiken het is gelijk teken `=` om aan te geven dat we een waarde gaan toekennen aan de variabele.
- We gebruiken de vierkante haken `[]` om aan te geven dat we een lijst gaan maken.
- In de vierkante haken zetten we de waardes waaruit de lijst gaat bestaan, als voorbeeld gaat het hier
  om ``Appels``, ``Peren``, ``Bananen`` en ``Brood``.
- Om elke waarde zetten we aanhalingstekens `""` om aan te geven dat het om een string gaat.
- Om elke waarde zetten we een komma `,` om aan te geven dat het om een nieuwe waarde gaat.

Laten we nog even een ander voorbeeld pakken:

```python
huisnummers = [1, 3, 5, 7, 9]
``` 

In dit geval hebben we een lijst van huisnummers, we hebben hier geen aanhalingstekens gebruikt omdat het om een getal
De constructie blijft echter wel grotendeels gelijk:

- We beginnen met de variabele naam, in dit geval is dat `huisnummers`.
- We gebruiken het is gelijk teken `=` om aan te geven dat we een waarde gaan toekennen aan de variabele.
- We gebruiken de vierkante haken `[]` om aan te geven dat we een lijst gaan maken.
- In de vierkante haken zetten we de waardes waaruit de lijst gaat bestaan, als voorbeeld gaat het hier
  om ``1``, ``3``, ``5``, ``7`` en ``9``.
- Om elke waarde zetten we een komma `,` om aan te geven dat het om een nieuwe waarde gaat.

Genoeg gelezen, laten we nu overgaan naar het uitvoeren!

### Opdrachten
Je kunt deze opdrachten maken op de [online omgeving van Python](https://www.mycompiler.io/nl/new/python){:target="_blank"}
**Sla je antwoorden goed op! We zullen deze gedurende alle opdrachten gebruiken!**

```python

# Opdracht 1: Maak een lijst met 5 verschillende. 
# Noem de lijst getallen_lijst en zet er 5 verschillende getallen in.

# Opdracht 2: Maak een lijst met 5 namen.
# Noem de lijst namen_lijst en zet er 5 verschillende namen in.

# Opdracht 3: Maak een lijst met 5 verschillende postcodes.
# Noem de lijst postcode_lijst en zet er 5 verschillende postcodes in.
# Een postcode bevat letters, cijfers en een spatie.

# Opdracht 4: Maak een lijst met 5 variable.
# Noem de lijst variable_lijst en zet er 5 verschillende variabelen in.
# Je mag zelf kiezen wat je in de lijst zet, maar zorg er wel voor dat je enkel variabele gebruikt en geen letters of getallen.

```

Okay we hebben nu een beetje kennis gemaakt met de lijsten, maar wat kunnen we er nu mee?

We zullen nu even de operaties van lijsten doornemen. De belangrijkste operaties die we kunnen uitvoeren zijn:

- Waardes opvragen uit een lijst.
- Toevoegen van een waarde aan een lijst.
- Verwijderen van een waarde uit een lijst.
- Wijzigen van een waarde in een lijst.

## Waardes opvragen uit een lijst

Laten we weer even een voorbeeld lijst nemen.

```python
boodschappenlijst = ["Appels", "Peren", "Bananen", "Brood"]
```

Stel dat ik nu wil weten wat de eerste waarde is van de lijst?
Dan kan ik dat doen door de volgende regel te gebruiken:

```python
eerste_waarde = boodschappenlijst[0]
```

In dit geval is de variable `eerste_waarde` gelijk aan de waarde `Appels` uit onze `boodschappenlijst`.
Hoe komen we aan deze waarde? We geven hierbij aan dat we de eerste waarde willen hebben door de `[0]` achter de lijst
te zetten.

**Let op!** Python begint te tellen vanaf 0, dus de eerste waarde is `[0]`, de tweede waarde is `[1]` enzovoort.
Het lijkt een beetje raar, maar dit is een conventie die in veel programmeertalen wordt gebruikt!
Je zult er naarmate je meer programmeert steeds meer aan wennen.

Deze waarde heet de index! De index is een manier om aan te geven welke waarde je wilt hebben uit een lijst.
Indexen beginnen altijd bij 0, dus de eerste waarde is `[0]`, de tweede waarde is `[1]` enzovoort.
Dus als je kijkt naar ons codevoorbeeld, dan zul je de bovenstaande getallen in je hoofd moeten neerzetten.

```python
                        0         1         2         3
boodschappenlijst = ["Appels", "Peren", "Bananen", "Brood"]
```

Als we dus de waardes willen opvragen komt dat er als volgt uit te zien:

```python
eerste_waarde = boodschappenlijst[0]  # "Appels"
tweede_waarde = boodschappenlijst[1]  # "Peren"
derde_waarde  = boodschappenlijst[2]  # "Bananen"
vierde_waarde = boodschappenlijst[3]  # "Brood"
```

Laten we nu eens kijken naar een ander voorbeeld:

```python
huisnummers = [1, 3, 5, 7, 9]
```

Stel dat ik nu wil weten wat de derde waarde is van de lijst? Kan je raden hoe dit moet?

```python
derde_waarde = huisnummers[2] # 5
```

Als laatste stap zullen we nog een handig trucje leren!
Stel dat we willen weten of een waarde in een lijst zit! Dit kunnen we doen door de volgende regel te gebruiken:

```python
waarde = "Appels"
boodschappenlijst = ["Appels", "Peren", "Bananen", "Brood"]
if waarde in boodschappenlijst:
    print("De waarde zit in de lijst!")
else:
    print("De waarde zit niet in de lijst!")
```

In dit geval zullen we de volgende output krijgen:

```python
De waarde zit in de lijst!
```
Laten we dit even ontleden:
- We beginnen met de variabele naam, in dit geval is dat `waarde`.
- We geven de waarde `Appels` aan de variabele `waarde`.
- We beginnen met de variabele naam, in dit geval is dat `boodschappenlijst`.
- We gebruiken de `in` keyword om aan te geven dat we willen weten of de waarde in de lijst zit. In dit geval kan je in zien als letterlijk "zit het er in?".
- We gebruiken de `if` keyword om aan te geven dat we een controle willen uitvoeren. Als de waarde in de lijst zit, dan voeren we de code uit die onder de `if` staat.
- We gebruiken de `else` keyword om aan te geven dat we een alternatief willen uitvoeren als de waarde niet in de lijst zit. In dit geval voeren we de code uit die onder de `else` staat.
Dit is een handige manier om te achterhalen of een waarde in een lijst zit!


Laten we even een aantal opgave maken om te zorgen dat je dit goed begrijpt!

### Opdrachten
Je kunt deze opdrachten maken op de [online omgeving van Python](https://www.mycompiler.io/nl/new/python){:target="_blank"}
```python
# Opdracht 1: Print het eerste element van de lijst getallen_lijst.
# Opdracht 2: Print het tweede element van de lijst namen_lijst.
# Opdracht 3: Print het derde element van de lijst postcode_lijst.
# Opdracht 4: Print het vierde element van de lijst variable_lijst.
# Opdracht 5: Controleer of de waarde 5 in de lijst getallen_lijst zit, print "De waarde zit in de lijst!" als dit het geval is, anders print "De waarde zit niet in de lijst!".
```

Tot zover het gedeelte over het opvragen van waardes uit een lijst, laten we nu eens kijken naar het toevoegen van een
element!

## Toevoegen van een waarde aan een lijst

Er zijn twee methode voor het toevoegen van een element aan een lijst:

1. append()
2. extend()

### Append()
We pakken weer ons vertrouwde bootschappenlijstje erbij:

```python
boodschappenlijst = ["Appels", "Peren", "Bananen", "Brood"]
```

Laten we nu zeggen dat we hier nog een product aan willen toevoegen, bijvoorbeeld `Melk`.
Dit kunnen we doen door de volgende regel te gebruiken:

```python
boodschappenlijst.append("Melk")
```

Het resultaat van deze regel is dat de lijst er nu als volgt uitziet:

```python
boodschappenlijst = ["Appels", "Peren", "Bananen", "Brood", "Melk"]
```

Er is nu een nieuw element toegevoegd aan de lijst!
Kijk eens goed naar de plek waar de waarde is toegevoegd. De waarde is toegevoegd aan het einde van de lijst, dit is een
standaard gedrag van de append() methode. Okay laten we nu even de werking aandachtig bekijken..

```python
boodschappenlijst.append("Melk")
```

- We beginnen met de variabele naam, in dit geval is dat `boodschappenlijst`.
- We gebruiken de punt `.` om aan te geven dat we een functie van de lijst gaan gebruiken.
- We gebruiken het keyword `append` om aan te geven dat we een waarde willen toevoegen aan de lijst. Append betekent
  toevoegen in het Engels.
- We gebruiken de haakjes `()` om aan te geven dat we een waarde meegeven aan de functie, zoals we eerder hebben
  besproken.
- In de haakjes zetten we de waarde die we willen toevoegen, in dit geval is dat `Melk`.
- Om de waarde zetten we aanhalingstekens `""` om aan te geven dat het om een reeks karakters gaat.

In conclusie: *Met append() geven we een enkele waarde mee, deze waarde wordt toegevoegd aan het einde van de lijst.*

### Extend()

Laten we nu eens kijken naar de extend() methode.

Stel dat we al een lijst hadden van boodschappen die we wilden kopen:

```python
boodschappenlijst = ["Appels", "Peren"]
```

We kregen toen het verzoek om een lijst van producten te kopen voor een pasta. De ingredienten voor de pasta zijn:

```python
pasta_ingredienten = ["Spaghetti", "Tomatensaus", "Kaas"]
```

Als we naar de supermarkt gaan wordt er 1 boodschappenlijstje gemaakt, we willen namelijk alle ingredienten in 1 keer
kopen.
Ons gewenst eindresultaat is dus:

```python
boodschappenlijst = ["Appels", "Peren", "Spaghetti", "Tomatensaus", "Kaas"]
```

Hoe kunnen we dit bereiken? Dit kunnen we doen door de extend() methode te gebruiken.

```python
pasta_ingredienten = ["Spaghetti", "Tomatensaus", "Kaas"]
boodschappenlijst = ["Appels", "Peren"]
boodschappenlijst.extend(pasta_ingredienten) # ["Appels", "Peren", "Spaghetti", "Tomatensaus", "Kaas"]
```

In dit geval hebben we de lijst `pasta_ingredienten` toegevoegd aan de lijst `boodschappenlijst`.
Het resultaat is dat de lijst `boodschappenlijst` nu bestaat uit de waardes van `boodschappenlijst`
en `pasta_ingredienten`.
Net zoals bij append is de waarde, in dit geval waardes, aan het einde van de lijst gekomen.

Tijd om hier mee te oefenen!

### Opdrachten
Je kunt deze opdrachten maken op de [online omgeving van Python](https://www.mycompiler.io/nl/new/python){:target="_blank"}
```python
# Opdracht 1: Voeg het getal 11000 toe aan de lijst getallen_lijst.
# Opdracht 2: Voeg de naam "Piet" toe aan de lijst namen_lijst.
# Opdracht 3: Voeg de postcode "1234 AB" toe aan de lijst postcode_lijst.
# Opdracht 4: Maak een lijst aan genaamd "lijst_1" met de waardes 1, 2, 3. Maak een lijst aan genaamd "lijst_2" met de
# waardes 4, 5, 6. Voeg de waardes van lijst_2 toe aan lijst_1.
```

Tot zover het gedeelte over het toevoegen van waardes aan een lijst, laten we nu eens kijken naar het verwijderen van
een waarde!

In conclusie, we gebruiken append voor het toevoegen van een **enkele** waarde en extend voor het toevoegen van *
*meerdere**.

## Verwijderen van een waarde uit een lijst

Er zijn twee methodes om een waarde te verwijderen uit een lijst:

1. Naam
2. Index

Laten we beginnen met de naam methode. We pakken weer onze boodschappenlijst erbij:

```python
boodschappenlijst = ["Appels", "Peren", "Bananen", "Brood"]
```

Stel dat we er net achter zijn gekomen dat we iemand anders al `Peren` had gekocht, hierdoor kunnen we deze verwijderen
uit de lijst.
Dit kunnen we doen door de volgende regel te gebruiken:

```python
boodschappenlijst.remove("Peren")
```

Laten we even bekijken wat hier gebeurt:

- We beginnen met de variabele naam, in dit geval is dat `boodschappenlijst`.
- We gebruiken de punt `.` om aan te geven dat we een functie van de lijst gaan gebruiken.
- We gebruiken het keyword `remove` om aan te geven dat we een waarde willen verwijderen uit de lijst. Remove betekent
  verwijderen in het Engels.
- We gebruiken de haakjes `()` om aan te geven dat we een waarde meegeven aan de functie, zoals we eerder hebben
  besproken.
- In de haakjes zetten we de waarde die we willen verwijderen, in dit geval is dat `Peren`.

- Het resultaat van deze regel is dat de lijst er nu als volgt uitziet:

```python
boodschappenlijst = ["Appels", "Bananen", "Brood"]
```

Er is nu een element verwijderd uit de lijst!

Met de remove() methode geven we een enkele waarde mee, deze waarde wordt dan opgezocht in de lijst en verwijderd.
Je kan je voorstellen dat dit handig is als je weet welke waarde je wilt verwijderen, maar wat als je de waarde niet?

Laten we nu eens kijken naar de index methode.

We pakken weer onze boodschappenlijst erbij:

```python
boodschappenlijst = ["Appels", "Peren", "Bananen", "Brood"]
```

We zijn nu in de winkel en pakken steeds het eerste product van de lijst en verwijderen deze als we het product hebben.

De lijst moet er dan als volgt uitzien:

```python
boodschappenlijst = ["Appels", "Peren", "Bananen", "Brood"]
boodschappenlijst = ["Peren", "Bananen", "Brood"]
boodschappenlijst = ["Bananen", "Brood"]
boodschappenlijst = ["Brood"]
```

Elke keer pakken we dus het eerste product en verwijderen we deze uit de lijst.
Gelukkig heeft Python hier een goede functie voor, genaamd `pop()`!

```python
boodschappenlijst = ["Appels", "Peren", "Bananen", "Brood"]
eerste_waarde = boodschappenlijst.pop(0) # "Appels"
print(boodschappenlijst) # ["Peren", "Bananen", "Brood"]
```

Laten we er even stap voor stap doorheen lopen:

- We beginnen met de variabele naam, in dit geval is dat `boodschappenlijst`.
- We gebruiken de punt `.` om aan te geven dat we een functie van de lijst gaan gebruiken.
- We gebruiken het keyword `pop` om aan te geven dat we een waarde willen verwijderen uit de lijst. Pop betekent
  verwijderen in het Engels.
- We gebruiken de haakjes `()` om aan te geven dat we een waarde meegeven aan de functie, zoals we eerder hebben
  besproken.
- In de haakjes zetten we de index van de waarde die we willen verwijderen, in dit geval is dat `0`. Denk hierbij weer
  even aan onze eerdere discussie over indexen.
- De waarde die we hebben verwijderd is teruggegeven door de pop() functie, hierdoor kunnen we deze waarde nog
  gebruiken. Dit is handig als je de waarde nog wilt gebruiken, maar ook als je wilt weten welke waarde je hebt
  verwijderd.

Welke van de twee functies (remove() en pop()) je gebruikt hangt af van de situatie. Als je de waarde weet die je wilt
verwijderen, dan is remove() handig. Als je de index weet, dan is pop() handig.
Het maakt dus eigenlijk niet uit welke je gebruikt, zolang je maar weet wanneer je welke moet gebruiken!

Laten we even oeferen met deze nieuwe kennis!

### Opdrachten
Je kunt deze opdrachten maken op de [online omgeving van Python](https://www.mycompiler.io/nl/new/python){:target="_blank"}
```python
# Opdracht 1: Verwijder het getal 11000 uit de lijst getallen_lijst.
# Opdracht 2: Verwijder de naam "Piet" uit de lijst namen_lijst.
# Opdracht 3: Verwijder de postcode "1234 AB" uit de lijst postcode_lijst.
# Opdracht 4: Van de lijst "lijst_1" verwijder je de eerste en de laatste waarde.
```

Tot zover het gedeelte over het verwijderen van waardes uit een lijst, laten we nu eens kijken naar het wijzigen van een
waarde.

## Wijzigen van een waarde in een lijst

Het wijzigen van een waarde in een lijst is een stuk eenvoudiger dan het verwijderen van een waarde, zo eenvoudig dat we
het in 1 regel kunnen doen!

We pakken weer onze boodschappenlijst erbij:

```python
boodschappenlijst = ["Appels", "Peren", "Bananen", "Brood"]
```

Stel dat we er net achter zijn gekomen dat `Sinaasappels` in de aanbieding zijn en we daarom geen `Peren` meer willen
hebben.
We kunnen er dan voor kiezen om de waarde `Peren` te verwijderen en `Sinaasappels` toe te voegen, maar we kunnen ook de
waarde `Peren` wijzigen naar `Sinaasappels`!

Dit kunnen we doen door de volgende regel te gebruiken:

```python
boodschappenlijst[1] = "Sinaasappels"
```

Laten we even bekijken wat hier gebeurt:

- We beginnen met de variabele naam, in dit geval is dat `boodschappenlijst`.
- We gebruiken de vierkante haken `[]` om aan te geven dat we een waarde willen wijzigen in de lijst.
- In de vierkante haken zetten we de index van de waarde die we willen wijzigen, in dit geval is dat `1`.
- We gebruiken het is gelijk teken `=` om aan te geven dat we een waarde gaan toekennen aan de variabele.
- We zetten de nieuwe waarde achter het is gelijk teken, in dit geval is dat `Sinaasappels`.
- Om de waarde zetten we aanhalingstekens `""` om aan te geven dat het om een reeks karakters gaat.
- De waarde op index `1` is nu gewijzigd naar `Sinaasappels`.

Laten we dit even oefenen!

### Opdrachten
Je kunt deze opdrachten maken op de [online omgeving van Python](https://www.mycompiler.io/nl/new/python){:target="_blank"}
```python
# Opdracht 1: Wijzig een van de getallen naar 12000 in de lijst getallen_lijst.
# Opdracht 2: Wijzig een van de namen naar "Klaas" in de lijst namen_lijst.
# Opdracht 3: Wijzig een van de postocodes "5678 CD" in de lijst postcode_lijst.
# Opdracht 4: Wijzig de eerste waarde van lijst_1 naar 10 en de laatste waarde naar 20.
```

In conclusie: *Met wijzigen van een waarde in een lijst geven we de index mee van de waarde die we willen wijzigen en de
nieuwe waarde.*

Tot zover het bewerken van lijsten in Python!
Laten we nu even verder gaan in Miney en zien hoe we dit kunnen verwerken!
[Klik hier voor de bijbehorende Miney opdrachten](https://brandonkroes.com/python/posts/les-2-miney/)
