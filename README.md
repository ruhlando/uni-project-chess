# uni-project-chess
Im Rahmen unserer Software-Engineering Vorlesung entwerfen wir eine **Modellierung** des Spiels Schach.<br>
Die **Projektanforderungen** sehen wie folgt aus:
- Jeder Spieler eigener/s PC / Tablet / Smartphone, Spiel läuft auf einem Server
- Anwendung stellt graphisch dar und checkt Validität von Benutzeraktionen
- Nicht: Computer als Spieler

Dafür werden folgende **UML-Diagrame** ausgearbeitet:
- Use-Case Diagramm
- Klassendiagramm
- Sequenzdiagramm


## Schachregeln


Schach ist ein strategisches Brettspiel für zwei Spieler. Hier sind die grundlegenden Regeln:
### Spielbrett und Aufstellung

Das Schachbrett besteht aus 64 Feldern (8x8) in abwechselnd hellen und dunklen Farben.
Jeder Spieler beginnt mit 16 Figuren: 1 König, 1 Dame, 2 Türme, 2 Läufer, 2 Springer und 8 Bauern.
Die Figuren werden in einer spezifischen Anordnung auf den beiden dem Spieler nächstgelegenen Reihen aufgestellt.

### Grundlegende Spielmechanik

Weiß macht den ersten Zug, danach ziehen die Spieler abwechselnd.
Ein Zug besteht aus dem Bewegen einer eigenen Figur auf ein freies Feld oder dem Schlagen einer gegnerischen Figur.
Jede Figurenart hat ihre eigenen Bewegungsregeln.

### Figurenbewegungen
#### König 

Kann ein Feld in jede Richtung ziehen. 
#### Dame 
Bewegt sich beliebig viele Felder horizontal, vertikal oder diagonal. 
#### Turm 
Zieht beliebig viele Felder horizontal oder vertikal. 
#### Läufer 
Bewegt sich beliebig viele Felder diagonal. 
#### Springer 
Zieht in einem "L"-Muster: zwei Felder in eine Richtung und dann ein Feld im 90-Grad-Winkel. 
#### Bauer

Zieht ein Feld vorwärts (beim ersten Zug optional zwei Felder).  
Schlägt diagonal ein Feld vorwärts.

### Spezielle Regeln

**Schach:** Wenn der König bedroht ist, muss der Spieler diese Bedrohung im nächsten Zug abwenden.  

**Schachmatt:** Das Spiel endet, wenn ein König im Schach steht und keine legale Möglichkeit hat, diesem zu entkommen.  

**Patt:** Das Spiel endet unentschieden, wenn ein Spieler am Zug ist, aber keinen legalen Zug machen kann, ohne seinen König ins Schach zu setzen.  

**Rochade:** Ein spezieller Zug, bei dem König und Turm gleichzeitig bewegt werden.  

**En Passant:** Eine spezielle Fangmethode für Bauern.  

**Bauernumwandlung:** Ein Bauer, der die gegnerische Grundlinie erreicht, wird in eine andere Figur (üblicherweise eine Dame) umgewandelt.  



Use Case Diagramm: <br>
![Use Case Diagramm](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.githubusercontent.com/ruhlando/uni-project-chess/refs/heads/main/usecases.iuml?token=GHSAT0AAAAAACZIWQ3HIMJZRLUKBDAA6OD2ZY2C47A)
