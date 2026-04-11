# CNC-Fräse sicher herunterfahren

Der Shutdown-Prozess muss immer in der gleichen Reihenfolge erfolgen, damit keine Achse unerwartet fährt und die Maschine sauber für den nächsten Nutzer übergeben wird.

## Reihenfolge: Shutdown nach dem Fräsen

1. **Fräsjob beenden**  
	Warten, bis alle Achsen stehen und die Spindel komplett aus ist.
2. **Z-Achse in sichere Höhe fahren**  
	Werkzeug vom Werkstück wegfahren, damit beim weiteren Handling keine Kollision entsteht.
3. **X/Y in Parkposition fahren**  
	Arbeitsbereich so anfahren, dass Werkstück und Spannmittel gut zugänglich sind.
4. **MMS/Kühlung ausschalten**  
	Falls genutzt: Zufuhr stoppen, Restdruck abbauen, Tropfenbildung vermeiden.
5. **CNC-Controller stoppen**  
	In Estlcam CNC den Betrieb sauber beenden, bevor irgendetwas an Hardware ausgeschaltet wird.
6. **Spindel/Frequenzumrichter ausschalten (falls separat geschaltet)**  
	Nur nach sicherem Stillstand.
7. **Werkstück entnehmen und Spannmittel lösen**  
	Vorsichtig ausspannen, scharfe Kanten beachten.
8. **Maschine reinigen**  
	Späne an Tisch, Führungen und im Arbeitsraum entfernen; Werkzeugaufnahme sauber halten.
9. **Sichtprüfung auf Beschädigungen**  
	Fräser, Spannzange, Kabel und Not-Aus Bereich kurz kontrollieren.
10. **PC/Software sauber schliessen**  
	Dateien sichern, Projekte speichern, Programme geordnet beenden.
11. **Hauptschalter/Versorgung ausschalten (wenn vorgesehen)**  
	Erst ganz am Ende die Gesamtversorgung trennen.

## Sonderfall: Werkzeugwechsel während eines Jobs

* Maschine anhalten und Spindelstillstand abwarten.
* Fräser wechseln wie in der Fräser-Anleitung beschrieben.
* **Z-Nullpunkt zwingend neu setzen**, danach erst Job fortsetzen.

## Übergabe-Check

* Arbeitsfläche sauber
* Werkzeuge und Schlüssel aufgeräumt
* Keine Warnmeldung aktiv
* Maschine in sicherem Endzustand

[Reinigung](reinigung.md)

[Zurück zum Start](https://makerspace-wi.github.io/Project-CNC-3/)
