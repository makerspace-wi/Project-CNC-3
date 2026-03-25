# Nullpunkte festlegen

Die Achsennullpunkte bestimmen, wo der CNC-Job startet.  
Falsch gesetzte Nullpunkte fuehren schnell zu Massfehlern, Luftfraesen oder Kollisionen.

## Ziel

* X0 / Y0: Bezugspunkt auf dem Werkstueck gemaess CAM-Setup
* Z0: Hoehenbezug auf Werkstueckoberflaeche oder Opfermaterial (wie im CAM-Job definiert)

## Vorbedingungen

* Fraeser ist korrekt montiert und festgezogen
* Werkstueck ist final gespannt (danach nicht mehr verschieben)
* CAM-Datei ist geladen und der gewuenschte Nullpunkt ist bekannt
* Spindel steht still

## Schritt-fuer-Schritt: Achsennullpunkte einstellen

1. **Nahe an den Zielpunkt fahren**  
	Mit Fernsteuerung oder Maus die Achsen in langsamer Geschwindigkeit in die Naehe des geplanten Nullpunkts bewegen.
2. **X und Y exakt ausrichten**  
	Fräsermittelpunkt auf die gewuenschte Ecke oder Markierung positionieren.  
	Zum Schluss nur noch mit kleinen Schritten (Feinverstellung) korrigieren.
3. **X/Y nullen**  
	Im CNC-Controller die aktuelle Position als X0 und Y0 setzen.
4. **Z-Hoehe anfahren**  
	Fraeser vorsichtig in Z nach unten fahren, bis der Bezugspunkt fast erreicht ist.
5. **Z exakt setzen**  
	Je nach Vorgehen in der Einweisung:
	* Direkt auf Oberflaeche tasten (sehr kleine Schritte), oder
	* Papiermethode verwenden (Papier klemmt leicht zwischen Werkzeug und Flaeche)
6. **Z nullen**  
	Aktuelle Z-Position als Z0 setzen.
7. **Sicherheitsabstand anfahren**  
	Werkzeug einige Millimeter in Z nach oben fahren.

## Wichtige Hinweise

* Nullpunkte immer **nach** dem finalen Spannen setzen
* Nach Fraeserwechsel Z-Nullpunkt zwingend neu setzen
* Wenn X/Y-Bezug verschoben wurde: X und Y neu setzen
* Bei Unsicherheit lieber erneut antasten statt mit falschem Nullpunkt starten

## Typische Fehler

* CAM-Nullpunkt (z. B. linke vordere Ecke) passt nicht zum real gesetzten Nullpunkt
* Z-Nullpunkt auf falscher Flaeche gesetzt (Werkstueck statt Opfermaterial oder umgekehrt)
* Nach dem Nullen wurde das Werkstueck nochmals verschoben
* Z zu schnell angefahren und Werkzeug/Flaeche beruehrt

## 20-Sekunden-Check vor Start

* X0/Y0/Z0 sind gesetzt und plausibel
* Werkzeug ist auf sicheren Z-Abstand gefahren
* Simulation/Vorschau passt zur realen Position
* Erst jetzt Fräsjob starten

[Zurück zum Start](https://makerspace-wi.github.io/Project-CNC-3/)
