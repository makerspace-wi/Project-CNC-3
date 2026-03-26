# Nullpunkte festlegen

Die Achsennullpunkte bestimmen, wo der CNC-Job startet.  
Falsch gesetzte Nullpunkte führen schnell zu Massfehlern, Luftfräen oder Kollisionen.  
Im folgenden wird zunächst die manülle Vorgehensweise erklärt.

## Ziel

* X0 / Y0: Bezugspunkt auf dem Werkstück gemäss CAM-Setup
* Z0: Höhenbezug auf Werkstückoberfläche (wie bei der CNC-3 im Setup definiert)

## Vorbedingungen

* Fräser ist korrekt montiert und festgezogen
* Werkstück ist final gespannt (danach nicht mehr verschieben)
* CAM-Datei ist geladen und der gewünschte Nullpunkt ist bekannt
* Spindel steht still

## Schritt-für-Schritt: Achsennullpunkte einstellen

1. **Nahe an den Zielpunkt fahren**  
	Mit Fernsteuerung, Tastatur oder Maus die Achsen in langsamer Geschwindigkeit in die Nähe des geplanten Nullpunkts bewegen.
2. **X und Y exakt ausrichten**  
	Fräsermittelpunkt auf die gewünschte Ecke oder Markierung positionieren.  
	Zum Schluss nur noch mit kleinen Schritten (Feinverstellung) korrigieren.
3. **X/Y nullen**  
	Im CNC-Controller die aktuelle Position als X0 und Y0 setzen.
4. **Z-Höhe anfahren**  
	Fräser vorsichtig in Z nach unten fahren, bis der Bezugspunkt fast erreicht ist.
5. **Z exakt setzen**  
	Je nach Vorgehen in der Einweisung:
	* Direkt auf Oberfläche tasten (sehr kleine Schritte), oder
	* Papiermethode verwenden (Papier klemmt leicht zwischen Werkzeug und Fläche)
6. **Z nullen**  
	Aktuelle Z-Position als Z0 setzen.
7. **Sicherheitsabstand anfahren**  
	Werkzeug einige Millimeter in Z nach oben fahren.

## Wichtige Hinweise

* Nullpunkte immer **nach** dem finalen Spannen setzen
* Nach Fräserwechsel Z-Nullpunkt zwingend neu setzen
* Wenn X/Y-Bezug verschoben wurde: X und Y neu setzen
* Bei Unsicherheit lieber erneut antasten statt mit falschem Nullpunkt starten

## Typische Fehler

* CAM-Nullpunkt (z. B. linke vordere Ecke) passt nicht zum real gesetzten Nullpunkt
* Z-Nullpunkt auf falscher Fläche gesetzt (Werkstück statt Opfermaterial oder umgekehrt)
* Nach dem Nullen wurde das Werkstück nochmals verschoben
* Z zu schnell angefahren und Werkzeug/Fläche berührt

## 20-Sekunden-Check vor Start

* X0/Y0/Z0 sind gesetzt und plausibel
* Werkzeug ist auf sicheren Z-Abstand gefahren
* Simulation/Vorschau passt zur realen Position
* Erst jetzt Fräsjob starten

[Zurück zum Start](https://makerspace-wi.github.io/Project-CNC-3/)
