# uni-project-chess
Im Rahmen unserer Software-Engineering Vorlesung entwerfen wir eine **Modellierung** des Spiels Schach.<br>
Die **Projektanforderungen** sehen wie folgt aus:
- Jeder Spieler eigener/s PC / Tablet / Smartphone, Spiel läuft auf einem Server
- Anwendung stellt graphisch dar und checkt Validität von Benutzeraktionen
- Nicht: Computer als Spieler

Dafür werden folgende **UML-Diagramme** ausgearbeitet:
- Use-Case Diagramm
- Klassendiagramm
- Sequenzdiagramm


## 📖 Schachregeln

Schach ist ein strategisches Brettspiel für zwei Spieler. Hier sind die grundlegenden Regeln:
### Spielbrett und Aufstellung

Das Schachbrett besteht aus 64 Feldern (8x8) in abwechselnd hellen und dunklen Farben.
Jeder Spieler beginnt mit 16 Figuren: 1 König, 1 Dame, 2 Türme, 2 Läufer, 2 Springer und 8 Bauern.
Die Figuren werden in einer spezifischen Anordnung auf den beiden dem Spieler nächstgelegenen Reihen aufgestellt.

### Grundlegende Spielmechanik

Weiß macht den ersten Zug, danach ziehen die Spieler abwechselnd.
Ein Zug besteht aus dem Bewegen einer eigenen Figur auf ein freies Feld oder dem Schlagen einer gegnerischen Figur.
Jede Figurenart hat ihre eigenen Bewegungsregeln.

### `Figuren`

<table>
<tr>
<td>

**♚ König**<br>
Kann ein Feld in jede Richtung ziehen.

</td>
<td>
<img src="img/king_movement.png" alt="König Bewegung" width="200"/>
</td>
</tr>

<tr>
<td>

**♛ Dame**<br>
Bewegt sich beliebig viele Felder horizontal, vertikal oder diagonal.

</td>
<td>
<img src="img/queen_movement.png" alt="Dame Bewegung" width="200"/>
</td>
</tr>

<tr>
<td>

**♜ Turm**<br>
Zieht beliebig viele Felder horizontal oder vertikal. 

</td>
<td>
<img src="img/rook_movement.png" alt="Turm Bewegung" width="200"/>
</td>
</tr>

<tr>
<td>

**♝ Läufer**<br>
Bewegt sich beliebig viele Felder diagonal.

</td>
<td>
<img src="img/bishop_movement.png" alt="Läufer Bewegung" width="200"/>
</td>
</tr>

<tr>
<td>

**♞ Springer**<br>
Zieht in einem "L"-Muster: zwei Felder in eine Richtung und dann ein Feld im 90-Grad-Winkel.

</td>
<td>
<img src="img/knight_movement.png" alt="Springer Bewegung" width="200"/>
</td>
</tr>

<tr>
<td>

**♟ Bauer**<br>
Zieht ein Feld vorwärts (beim ersten Zug optional zwei Felder).  
Schlägt diagonal ein Feld vorwärts.

</td>
<td>
<img src="img/pawn_movement.png" alt="Bauer Bewegung" width="200"/>
</td>
</tr>
</table>

### `Spezielle Regeln`

**Schach:** Wenn der König bedroht ist, muss der Spieler diese Bedrohung im nächsten Zug abwenden.  

**Schachmatt:** Das Spiel endet, wenn ein König im Schach steht und keine legale Möglichkeit hat, diesem zu entkommen.  

**Patt:** Das Spiel endet unentschieden, wenn ein Spieler am Zug ist, aber keinen legalen Zug machen kann, ohne seinen König ins Schach zu setzen.  


**Rochade:** Ein spezieller Zug, bei dem König und Turm gleichzeitig bewegt werden.

<img src="img/castling.png" alt="Rochade" width="550"/>

**En Passant:** Eine spezielle Fangmethode für Bauern.

<img src="img/en_passant.png" alt="En Passant" width="550"/>

**Bauernumwandlung:** Ein Bauer, der die gegnerische Grundlinie erreicht, wird in eine andere Figur (üblicherweise eine Dame) umgewandelt.

<img src="img/pawn_promotion.png" alt="Bauernumwandlung" width="550"/>

## 👨🏽‍💻 Unsere Vorgehensweise
<table>
<tr>
<td>

### 🛠️ Tools:

- Github Repository
- Github Projects
- [PlantUML](https://plantuml.com)

</td>
<td>

<img src="https://media.giphy.com/media/du3J3cXyzhj75IOgvA/giphy.gif?cid=790b7611k5o7mvfr270ww0tu2q4dhea4vv65bavl95vlvvk9&ep=v1_gifs_search&rid=giphy.gif&ct=g" alt="Github Gif" width="200"/>

</td>
</tr>
</table>

## ⛓️‍💥 UML-Diagramme

### `Use-Case Diagramm`
![Use-Case Diagramm](/img/UML/use-case-diagram.png)

#### Detaillierte Use-Case Beschreibungen:
- [Use Case 1: Figur umwandeln](/Use%20Cases/use-case-figurumwandeln.md)
- [Use Case 2: Zug machen](/Use%20Cases/use-case-zugmachen.md)
- [Use Case 3: Spiel anlegen](/Use%20Cases/use-case-spielanlegen.md)
- [Use Case 4: Aufgeben](/Use%20Cases/use-case-aufgeben.md)
- [Use Case 5: Einstellungen ändern](/Use%20Cases/use-case-einstellungaendern.md)
- [Use Case 6: Zug validieren](/Use%20Cases/use-case-zugvalidieren.md)

### `Klassendiagramm`
![Klassendiagramm](img/UML/class-diagram.png)

Zusätzlich haben wir ein [Data Dictionary](/Classes/dataDictionary.md) und eine [Übersicht der Assoziationen](/Classes/associations.md) zwischen den Klassen erstellt.

### `Sequenzdiagramm`
<p>Wir haben für den Zug eines Bauern (mit all seinen Möglichkeiten: En Passant, Umwandlung) ein UML Sequenzdiagramm erstellt: </p>

![Sequenzdiagramm Bauernzug](/img/UML/sequence-diagram-pawn_move.png)

## 💡 Unsere Learnings
- [PlantUML](https://plantuml.com) ein sehr cooles Tool!
- Umgang mit Github (Versionskontrolle, Zusammenarbeit mit dem Team, etc.)
- Best Practices des Software-Engineerings, bzw. der Softwaremodellierung

## ℹ️ Quellen
Garber, Thomas. (2009). *Schach - Die Spielregeln*. [PDF](/Schachregeln.pdf)
