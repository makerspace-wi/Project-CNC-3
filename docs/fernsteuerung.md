# Funktionen Handrad Fernsteuerung

<img src="images/ESTLCAM Handrad.png" width="400">

Der Joystick der Fernsteuerung hat folgende Funktionen:

- hoch/runter: Bewegung der Y-Achse nach hinten/vorne - je größer die Auslenkung, desto schneller die Achsenbewegung.
- links/rechts: Bewegung der X-Achse nach links/rechts - je größer die Auslenkung, desto schneller die Achsenbewegung.
- Drehung des Joysticks nach rechts/links: Bewegung der Z-Achse nach open/unten - je weiter die Drehung, desto schneller die Achsenbewegung.

Der Drehgeber bewegt immer die Achse, die zuletzt mit dem Joystick verfahren wurde - also automatisch die richtige. 

Leuchtender Taster (blau) in der Mitte: Abnullen -> kurz drücken nullt die ausgewählte Achse, lang drücken nullt alle ab.

## Programmablauf steuern

- Ein Druck auf den mit "S" beschrifteten Knopf startet oder Stopt die Spindel manuell
- Ein Druck auf den mit "F" beschrifteten Knopf startet das geladene CNC Programm
- Durch drehen am "F" Knopf kann die Vorschubgeschwindigkeit von 0 bis 100% angepasst werden
- Durch drehen am "S" Knopf kann die Spindeldrehzahl von 0 bis 200% variiert werden
- Drücken bei laufendem Programm einen der beiden Knöpfe pausiert das Programm

[Zurück zum Start](https://makerspace-wi.github.io/Project-CNC-3/#hilfestellungen-zum-fr%C3%A4sjob)  ---  [Weiter]()
