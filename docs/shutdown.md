# CNC-Fräse sicher herunterfahren

Der Shutdown-Prozess muss immer in der gleichen Reihenfolge erfolgen, damit keine Achse unerwartet fährt und die Maschine sauber für den nächsten Nutzer übergeben wird.

## Reihenfolge: Shutdown nach dem Fräsen

1. **Fräsjob beenden**  
	Warten, bis alle Achsen stehen und die Spindel komplett aus ist.
1. **MMS/Kühlung ausschalten**  
 Links unten - Falls genutzt: [MMS stoppen](mms.md)
1. **Makro [*Mitte*](macros.md) aufrufen (2. Button von links)**  
    Die Z-Achse wird in sichere Höhe und Fräser weg vom Werkstück bewegt, damit Werkstück und Spannmittel gut zugänglich sind.
1. **CNC-Controller stoppen**  
	In Estlcam CNC den Betrieb sauber beenden, bevor irgendetwas an Hardware ausgeschaltet wird.
1. **Spindel/Frequenzumrichter ausschalten (falls separat geschaltet)**  
	Nur nach sicherem Stillstand.
1. **Werkstück entnehmen und Spannmittel lösen**  
	Vorsichtig ausspannen, scharfe Kanten beachten.
1. **Maschine reinigen**  
	Späne an Tisch, Führungen und im Arbeitsraum entfernen; Werkzeugaufnahme sauber halten.
1. **Sichtprüfung auf Beschädigungen**  
	Fräser, Spannzange, Kabel und Not-Aus Bereich kurz kontrollieren.
1. **PC/Software sauber schliessen**  
	Dateien sichern, Projekte speichern, Programme geordnet beenden.
1. **Ausloggen**  
    abc    
1. **Hauptschalter/Versorgung ausschalten (wenn vorgesehen)**  
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
