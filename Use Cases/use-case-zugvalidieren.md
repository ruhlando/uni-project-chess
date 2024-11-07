Geschäftsprozess | Zug validieren
---|---
Ziel, Ergebnisse | Der Spielzug eines Spielers wird validiert
Akteure | Computer |
Vorbedingungen | Ein Spieler hat einen potentiellen Zug durchgeführt
Auslösendes Ereignis | Der Spieler der an der Reihe ist, wählt eine Schachfigur und ein Feld, auf das gezogen werden soll
Nachbedingung bei Erfolg | Der Zug des Spielers wird akzeptiert
Nachbedingung bei Fehlschlag | Der Spieler muss seinen Zug wiederholen
Eingehende Daten | Aktueller Spielstand, gewählte Schachfigur, gewähltes Feld
Ausgehende Daten | Neuer Spielstand
Ablauf | 1. Mögliche Züge der Figur laden <br> 2. Zug mit gewähltem Feld abgleichen <br> 3. positives Ergebnis speichern
Erweiterungen |---
Alternativen | 2a. Zug ist nicht möglich <br> 3. negatives Ergebnis speichern
