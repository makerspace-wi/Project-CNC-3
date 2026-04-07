# CNC-Fraese sicher herunterfahren

Der Shutdown-Prozess muss immer in der gleichen Reihenfolge erfolgen, damit keine Achse unerwartet faehrt und die Maschine sauber fuer den naechsten Nutzer uebergeben wird.

## Reihenfolge: Shutdown nach dem Fraesen

1. **Fraesjob beenden**  
	Warten, bis alle Achsen stehen und die Spindel komplett aus ist.
2. **Z-Achse in sichere Hoehe fahren**  
	Werkzeug vom Werkstueck wegfahren, damit beim weiteren Handling keine Kollision entsteht.
3. **X/Y in Parkposition fahren**  
	Arbeitsbereich so anfahren, dass Werkstueck und Spannmittel gut zugaenglich sind.
4. **MMS/Kuehlung ausschalten**  
	Falls genutzt: Zufuhr stoppen, Restdruck abbauen, Tropfenbildung vermeiden.
5. **CNC-Controller stoppen**  
	In Estlcam CNC den Betrieb sauber beenden, bevor irgendetwas an Hardware ausgeschaltet wird.
6. **Spindel/Frequenzumrichter ausschalten (falls separat geschaltet)**  
	Nur nach sicherem Stillstand.
7. **Werkstueck entnehmen und Spannmittel loesen**  
	Vorsichtig ausspannen, scharfe Kanten beachten.
8. **Maschine reinigen**  
	Spaene an Tisch, Fuehrungen und im Arbeitsraum entfernen; Werkzeugaufnahme sauber halten.
9. **Sichtpruefung auf Beschaedigungen**  
	Fraeser, Spannzange, Kabel und Not-Aus Bereich kurz kontrollieren.
10. **PC/Software sauber schliessen**  
	Dateien sichern, Projekte speichern, Programme geordnet beenden.
11. **Hauptschalter/Versorgung ausschalten (wenn vorgesehen)**  
	Erst ganz am Ende die Gesamtversorgung trennen.

## Sonderfall: Werkzeugwechsel waehrend eines Jobs

* Maschine anhalten und Spindelstillstand abwarten.
* Fraeser wechseln wie in der Fraeser-Anleitung beschrieben.
* **Z-Nullpunkt zwingend neu setzen**, danach erst Job fortsetzen.

## Uebergabe-Check

* Arbeitsflaeche sauber
* Werkzeuge und Schluessel aufgeraeumt
* Keine Warnmeldung aktiv
* Maschine in sicherem Endzustand

[Reinigung](reinigung.md)

[Zurück zum Start](https://makerspace-wi.github.io/Project-CNC-3/)
