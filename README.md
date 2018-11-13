# PlantUML Info Support Stijl
Plant UML Info Support Stijl voor PlantUML Diagrammen. 

# Gebruikershandleiding
Dit design is op twee manier te gebruiken. Het is mogelijk om een lokale kopie te gebruiken of een url aan te spreken.

## Lokale kopie
Om een lokale kopie te gebruiken moet allereerst het design.puml bestand gedownload worden. Vervolgens is het handig als dit bestand in dezelfde folder komt te staan als de rest van je PlantUML diagrammen. Vervolgens kan het design gebruikt worden door `!include design.puml` aan het begin van het bestand te zetten. Hieronder een voorbeeld:
```
@startuml
!include design.puml
// Rest van de code
@enduml
```

Naast dit design wordt ook een verzameling handige methoden aangeboden, deze methoden helpen een beter overzicht te houden. Deze methoden zijn te gebruiken door methods.puml te gebruiken, deze kan op de zelfde manier toegevoegd worden aan een project als het design.puml bestand: `!include methods.puml`.

Door het gebruik van deze methoden kan bijvoorbeeld voor een sequence diagram de acties op de volgende manier aangemaakt worden.

```
request(service1, service2, description)
return(service2, service1, description)
self(service1, description)
```
De methode `request()` kent 3 argumenten, als eerst een participant of actor welke verantwoordelijk is voor het request. Als tweede een participant of actor waarnaar het verzoek gedaan wordt. Tot slot een bescrijving van het verzoek. Hiermee wordt een vaste pijl getekend van de participant of actor meegegeven als eerste argument naar de participant of actor meegegeven als tweede argument. De `return()` methode werkt op de zelfde manier maar tekent een gestreepte pijl wat aantoont dat het om een return waarde gaat. De `self()` methode tekend een pijl van de participant of actor meegegeven als eerste argument naar zichzelf.

Indien het design en de methoden beide nodig zijn kunnen deze beide toegevoegd worden aan een diagram door `!include localindex.puml` bovenaan het diagram toe te voegen.

## Via een url
Om via een url te werken kan `!includeurl` gebruikt worden. Als er met een url gewerkt wordt heb je altijd de laatste versie. Hieronder een voorbeeld:
```
@startuml
#Design:
!includeurl https://raw.githubusercontent.com/luudvkeulen/PlantUMLISStijl/master/design.puml
#Methods:
https://raw.githubusercontent.com/luudvkeulen/PlantUMLISStijl/master/methods.puml
#Beide:
https://raw.githubusercontent.com/luudvkeulen/PlantUMLISStijl/master/remoteindex.puml
// Rest van de code
@enduml
```

# Voorbeelden
### Activity diagram
![alt text](https://i.imgur.com/JYLcZyn.png "Activity diagram")
### Sequence diagram
![alt text](https://raw.githubusercontent.com/luudvkeulen/PlantUMLISStijl/master/out/voorbeelden/sequencediagram/Sequence%20diagram.png "Sequence diagram")
