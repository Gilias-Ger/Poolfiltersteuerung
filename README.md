# Poolfiltersteuerung
ioBroker Blockly Poolfilter Steuerung

https://forum.iobroker.net/topic/23093/vorlage-poolfilterpumpensteuerung

# Funktionen:

*Alle Datenpunkte können automatisch erzeugt werden, einfach den Block über den Variablen-Stamm aktivieren und das Script neu Starten.

*Es gibt zwei Einschaltzeiten (00:00-23:59) sowie zwei Laufzeiten (60) in Minuten die frei wählbar sind.

*Wird die Filterpumpe per Hand eingeschalten nicht durch das Script schaltet die Pumpe nach z.B. 60min aus, diese Zeit kann auch geändert werden.

*Es gibt eine Handeinschalt Funktion die die Pumpe einschaltet aber nicht mehr ausschaltet es wird nur stündlich gemeldet das die Pumpe x Stunden an ist.

*Eine Zeitauswahl die die Pumpe für x Minuten (auswählbar) einschaltet und danach wieder ausschaltet.



# To-Do-List

*Erweiterung für pH und Chlor Dosierung

*Urlaubsmodus einfügen

*Sessonmodus einfügen


# Blockly Importieren

Unter Scripts erstellt ihr euch ein neues Blockly Script und öffnet dieses, oben rechts gibt es mehrere Icons klickt nun auf das zweite Icon "Blöcke importieren" fügt dort das Script ein und Importiert die Blöcke.

Links oben im script befinden sich die OB-Variablen diese müssen angepasst werde. Man kann auch die Objekte automatisch erzeugen lassen, dafür den deaktivierten Block aktivieren und das Script ein mal starten. Danach sind die Objekte unter Objekte -> javascript.0.Pool zu finden.


# VIS Importieren

die ZIP Datei einfach über Skripts -> oben links auf die 3 Punkte klicken -> Skripts importieren und ZIP Datei in das Fenster hineinziehen. Schon wird das Script unter "common -> Pool -> Filterpumpe" eingetragen.


# Versionen

*0.3 - Script erkennt ob Steuerung erreichbar ist. Wenn nicht wird eine Meldung ausgegeben. Filterung wird nicht aktiviert.

*0.2 - Bugfix, Meldung "Zeitauswahl abgebrochen" bei automatischer ausschaltung entfernt.

*0.1.3 - Bugfix der ObjektID erstellung, ObjektIDs erhalten nun die richtige Formatierung.

*0.1 -mehrere kleine Bugsfixs, VIS Import, Einbau von Statustext im VIS, Bei einschaltung durch die Zeitauswahl wird die Uhrzeit der ausschaltung im Status des VIS angezeigt

*0.0.8 - Bugfix, Einschalt mit Zeitauswahl eingebaut, Ein-/Ausschalten der Benachrichtung per Telegram, Pushover usw. (Baustein muss angepasst werden)

*0.0.2 - Handein-Autoausschaltung eingebaut

*0.0.1 - erstes Script

