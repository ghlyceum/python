---
title: '1.1: Functies!'
description: Code die andere code laat werken!

date: 2024-04-09 06:00:00 +0100
categories: [Lessen]
tags: [ ]
pin: true
math: true
mermaid: true
---

# Les 1:  Functies, controle en variabelen
## Introductie
Vandaag starten we met de eerste les van Python! Het is daardoor iets anders dan normaal.
De eerste les is vooral even een opfrisser van informatie die je al een keer hebt gehoord, vandoor ook even de volgende melding.

> Deze lesmodule is aanzienlijk langer dan andere modules! We zullen veel onderwerpen behandelen die al een keer langs zijn gekomen, maar het is mogelijk dat je er niet alles van herinnert. Neem de tijd om alles door te nemen en te oefenen. Als je vragen hebt, stel ze gerust!
{: .prompt-warning }

Mocht je sommige punten zijn vergeten? Geen probleem, we zullen het even kort herhalen en er zijn een tal van extra opdrachten.

## Leerdoel
Bij deze les hoort het volgende leerdoel: \\
**_Voor de start van de volgende les kan ik mijn teken app kennis op het gebied van functies, condities en variabele overzetten naar Python en hiermee kan ik simpele python functies bouwen._**

Hieruit kan je al ophalen dat we de kennis van de teken app gaan overzetten naar Python. Laten we beginnen met functies!


## Functies
> **Omschrijving**\
Het doel van functies in Python is om je code georganiseerd en herbruikbaar te maken.
Stel je voor dat je een opdracht vaak moet uitvoeren, zoals het omrekenen van seconde naar dagen. In plaats van elke
keer dezelfde code te schrijven, kun je een functie maken die deze taak uitvoert. Dan kun je die functie steeds opnieuw
gebruiken zonder de code te herhalen. Het helpt je om fouten te verminderen en je programma's makkelijker te begrijpen.
 
**Een functie aanroep bestaat uit drie onderdelen:**
1. De functienaam. Deze staat als eerste en wordt gebruikt om functies van elkaar te onderscheiden. Net zoals je eigen
  naam, wordt deze gebruikt om de functie aan te roepen of te gebruiken.
2. De Haakjes, (). De haakjes worden gebruikt om aan te geven dat wat er hierna komt parameters zijn.
3. De Parameter, hiermee geef je gegevens mee aan de functie om deze te gebruiken.
  {: .prompt-info }

### Voorbeeld in de teken app
Laten we even een voorbeeld functie pakken van de teken app. Stel dat ik een rechte lijn van 10 pixels op het scherm wil tekenen:

![Desktop View](/assets/img/les1/rechte%20kleine%20lijn.png){: width="auto" height="auto" }
_Rechte lijn uit de teken app_

Kan je je nog herinneren hoe dit moet?
1. ```penAan()``` om te beginnen met het tekenen van een lijn
2. ```vooruit(10)``` om de pen met 10 pixels naar voren te bewegen.

Als we dit in de teken app maken komt er het volgende uit:

![Desktop View](/assets/img/les1/tekenapp-rechtelijn.png){: width="auto" height="auto" }
_Tekenen van een lijn van 10 pixels_

#### Koppelen aan de definitie
Als we dit nu vergelijken met de functie definitie van hierboven, kunnen we de volgende overeenkomsten zien:
1. We beginnen met de functienaam, in dit geval ```penAan``` of ```vooruit```.
2. We hebben haakjes, ```()```, om aan te geven dat we een functie aanroepen.
3. We hebben een parameter, in dit geval ```10```, om aan te geven hoeveel pixels we vooruit willen.

Laten we nu eens kijken hoe dit eruit ziet in Python.


### Voorbeeld in Python
Laten we beginnen met een eenvoudig voorbeeld, namelijk het plaatsen van een blokje in Miney.
Denk weer even terug aan de opgaven van wiskunde en het hoe het assenstelsel. 
Als we een object in een 3D wereld willen plaatsen, hebben we 3 assen nodig.
- X is horizontaal, van links naar rechts. In de afbeelding is dit de rode lijn. 
- Y is verticaal, van beneden naar boven. In de afbeelding is dit de groene lijn.
- Z is diepte, van voor naar achter. In de afbeelding is dit de blauwe lijn.

![Desktop View](/assets/img/les1/3d%20ruimte%20axis.png){: width="auto" height="auto" }
_Kubus in een 3D ruimte_


#### Functie voor het plaatsen van een blok.
De functie voor het plaatsen van een blok ziet er als volgt uit:
```python
plaats_blok(x, y, z, blok_type)
```

We zien hier een aantal dingen staan:
1. ```plaats_blok``` is de naam van de functie.
2. ``()``, de haakjes waarin we de parameters plaatsen.
3. ```x, y, z, blok_type``` zijn de parameters die we meegeven aan de functie.

We hebben dus 4 paramaters nodig voor het plaatsen van een blokje.
De x, y en z zijn dus de locatie van het blokje, maar blok_type hebben we nog niet besproken.
De vierde parameter is het type blokje dat je wilt plaatsen. Dit kan bijvoorbeeld zand zijn, of een blokje hout.
Om het type blokje aan te geven moeten we de juiste naam weten, deze zijn online te achterhalen en zullen we later bespreken.

#### Gebruiken van de functie
Nu we weten wat de functie wil, kunnen we deze gebruiken. Laten we kiezen voor de volgende parameters:
- Het blokje moet op de X-as op plek 400 worden geplaatst. 
- Het blokje moet op de Y-as op plek 200 worden geplaatst.
- Het blokje moet op de Z-as op plek 100 worden geplaatst.
- Het blokje moet een blokje hout ("default:wood") zijn.

Als we dit voorbeeld vervolgens invullen komt er het volgende uit:

```python
plaats_blok(400, 200, 100, "default:wood")
```
---

## Functie constructie
Tot zover de uitleg van de **werking** van functies.
Laten we nu even nadenken over de **opbouw** van een functie!

Hierbij even een voorbeeld van een functie die we kunnen aanmaken in Python:
```python
def vermenigvuldig(a, b):
    return a * b
```

Laten we dit even ontleden:
1. ```def``` is een keyword die aangeeft dat we een functie gaan definiëren.
2. ```vermenigvuldig``` is de naam van de functie, deze naam is gekozen omdat dit precies is wat de functie doet.
3. ```(a, b)``` zijn de parameters die we meegeven aan de functie. Net zoals we hiervoor hebben besproken, worden de parameters in haakjes meegegeven.
4. ```:``` hiermee geven we aan dat we klaar zijn met de functie definiëren.
5. ```return``` is een keyword die aangeeft dat we iets terug geven.
6. ```a * b``` is de berekening die we uitvoeren. In dit geval vermenigvuldigen we a met b.

Als we deze functie dan gebruiken verwachten we het volgende:
```python
resultaat = vermenigvuldig(2, 3)
print(resultaat)
> 6
```

De functie print, doet zoals de naam al zegt, iets printen.

### Voorbeeld teken app
Denk weer even terug naar de teken app, hier heb je vaak eigen functies moeten maken, in de takenapp hadden we hier een andere naam voor.
In de teken app noemde we dit een **deeltaak**. Functies in Python zijn eigenlijk hetzelfde als deeltaken in de teken app.
Een voorbeeld deeltaak was het aanmaken van een vierkant, dit zag er zo uit:

![Desktop View](/assets/img/les1/vierkant%20tekenen.png){: width="auto" height="auto" }
_Vierkant tekenen_

In het voorbeeld is vierkant onze functie naam en de parameters zijn de lengte van de zijde van het vierkant.

### Verschil met Python
Het verschil is dus dat we zelf wat meer informatie moeten intikken in Python. Specifiek de volgende stappen:
- Wanneer we beginnen met het aanmaken van een functie gebruiken we ``def``.
- We geven de functie een naam, in dit geval ``vierkant``.
- We geven de parameters mee, wederom tussen haakjes, in dit geval ``(lengte)``.
- We sluiten de functie af met een dubbele punt, ``:``.
- Hierna vullen we de inhoud in van de functie, in dit geval het tekenen van een vierkant, maar hier gebeurt iets... geks.

Als je goed kijkt naar de vermenigvuldig functie, zie je dat we de regel eronder hebben geïndenteerd. Dit is een belangrijk onderdeel van Python, de indentatie.
Identatie betekent dat deze met een spatie of een tab naar binnen is gedrukt. Dit geeft aan dat de code binnen de functie valt. In de teken app konden we deze regels onder elkaar zetten, maar in Python moeten we dus een tab gebruiken.

Voor nu, genoeg gelezen. Programmeren leer je door te doen!


## Deel 1 - Functies
Deze opdrachten gaan over het maken van basis functies.
Je kunt deze opdrachten maken op de [online omgeving van Python](https://www.mycompiler.io/nl/new/python){:target="_blank"}
Kopieer de code en plak deze in de onlineomgeving.
Het maken van de extra opgaven hoeft niet per se, maar is zeker aan te bevelen.


```python

# Opdracht 1: Er mist iets..
# De volgende functies missen nog iets.. kan jij achterhalen wat er mist?

def min_tien(a)
    return a-10
plus_tien(a):
    return a-10
def maal_tien a:
    return a * 10
def delen_door_tien(a)
    a/10


# Opdracht 2: Vermenigvuldigen met honderd
# Maak een functie vermenigvuldig_met_honderd
# De functie krijgt 1 paramater, genaamd a.
# De functie vermenigvuldigd de waarde met honderd
# Het eindresultaat wordt teruggegeven.



# Opdracht 3: Centimeter naar Meter
# Maak een functie die berekent hoe je van centimeter naar meter gaat.
# De functie naam is centimeter_naar_meter
# De functie krijgt 1 paramater mee, namelijk de centimers
# De functie geeft het aantal meters terug.



# Opdracht 4: Berekenen verjaardag leeftijd
# Maak een functie die bepaalt hoe oud iemand wordt op basis van het geboortejaar.
# Bijvoorbeeld: als je in 2010 bent geboren wordt in je in 2024 14 jaar oud.
# Maak een functie genaamd bereken_verjaardag_leeftijd
# De functie krijgt 1 paramater mee, namelijk het jaartal van hun geboorte.
# Je mag er vanuit gaan dat we deze functie alleen testen op in het jaar 2024.


# EXTRA
# Opdracht 5: Optellen
# Maak een functie genaamd optellen.
# De functie krijgt 2 paramaters mee, a en b.
# De functie telt beide getallen bij elkaar op.
# De functie geeft de uitkomst terug.



# EXTRA
# Opdracht 6: Optellen en omrekenen
# Maak een functie genaamd centimeters_optellen_naar_meters
# De functie moet gebruik maken van je centimeter_naar_meter functie van opgave 4 en de optellen functie van opgave 6.
# De functie krijgt twee paramaters, a en b.
# De functie geeft de waarde terug in meters.
# Bijvoorbeeld centimeters_optellen_naar_meters(100, 100) is 2
```


Als je klaar bent met de opdrachten kan je ze nu controleren!
Kopieer de onderstaande code onderin om het controleren of het werkt!
```python

# test opdracht 2:
if 'vermenigvuldig_met_honderd' in globals():
    if(vermenigvuldig_met_honderd(1) == 100 and vermenigvuldig_met_honderd(2) == 200 ):
        print("Opdracht 2: Vermenigvuldigen met honderd is gelukt!")
    else:
        print("Opdracht 2: werkt nog niet helemaal, kijk er nog even een keer naar!")
        
# test opdracht 3:
if 'centimer_naar_meter' in globals():
    if(centimer_naar_meter(100) == 1 and centimer_naar_meter(150) == 1.5 ):
        print("Opdracht 3: De centimer naar meter berekening is gelukt!")
    else:
        print("Opdracht 3: werkt nog niet helemaal, kijk er nog even een keer naar!")

# test opdracht 4:
if 'bereken_verjaardag_leeftijd' in globals():
    if(bereken_verjaardag_leeftijd(1997) == 27 and bereken_verjaardag_leeftijd(2010) == 14 ):
        print("Opdracht 4: Het berekenen van de verjaardag leeftijd is gelukt!")
    else:
        print("Opdracht 4: werkt nog niet helemaal, kijk er nog even een keer naar!")

# test opdracht 5
if 'optellen' in globals():
    if(optellen(10, 10) == 20 and optellen(2, 6) == 8 ):
        print("Opdracht 5: Optellen is gelukt!")
    else:
        print("Opdracht 5: werkt nog niet helemaal, kijk er nog even een keer naar!")
        
# test opdracht 6
if 'centimeters_optellen_naar_meters' in globals():
    if(centimeters_optellen_naar_meters(150, 150) == 3 and centimeters_optellen_naar_meters(200, 200) == 4 ):
        print("Opdracht 6: Centimeters optellen naar meters is gelukt!")
    else:
        print("Opdracht 6: werkt nog niet helemaal, kijk er nog even een keer naar!")
```

Als je klaar bent, zie je dit onderin staan:

```
Opdracht 2: Vermenigvuldigen met honderd is gelukt!
Opdracht 3: De centimer naar meter berekening is gelukt!
Opdracht 4: Het berekenen van de verjaardag leeftijd is gelukt!
Opdracht 5: Optellen is gelukt!
Opdracht 6: Centimeters optellen naar meters is gelukt!


** Process exited - Return Code: 0 **
Press Enter to exit terminal
```

Als je dit ziet, dan heb je de opdrachten goed gemaakt! Gefeliciteerd! 🎉
Je kan nu verder gaan met het 2e deel van de lesstof, de [condities](https://brandonkroes.com/python/posts/les-1-controle/).



