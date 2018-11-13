# PlantUML Info Support Stijl
Plant UML Info Support Stijl voor PlantUML Diagrammen. 

# Gebruikershandleiding
Dit design is op twee manier te gebruiken. Het is mogelijk om een lokale kopie te gebruiken of een url aan te spreken.

## Lokale kopie
Om een lokale kopie te gebruiken moet allereerst het design.puml bestande gedownload worden. Vervolgens is het handig als dit bestand in dezelfde folder komt te staan als de rest van je PlantUML diagrammen. Vervolgens kan het design gebruikt worden door `!include design.puml` aan het begin van het bestand te zetten. Hieronder een voorbeeld:
```
@startuml
!include design.puml
// Rest van de code
@enduml
```

## Via een url
Om via een url te werken kan `!includeurl` gebruikt worden. Als er met een url gewerkt wordt heb je altijd de laatste versie. Hieronder een voorbeeld:
```
@startuml
!includeurl https://raw.githubusercontent.com/luudvkeulen/PlantUMLISStijl/master/design.puml
// Rest van de code
@enduml
```

# Voorbeelden
![alt text](https://i.imgur.com/JYLcZyn.png "Activity diagram")
