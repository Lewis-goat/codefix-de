---
title: Sage/Breville ER-Codes – die verborgene Servicetabelle verstehen
description: ER-Codes an Sage- und Breville-Maschinen stammen aus einer nie veröffentlichten Servicetabelle – so sind ER01–ER18 aufgebaut und die Oracle zählt anders.
---

Bleibt eine Breville-Espressomaschine abrupt stehen und zeigt ER05 im Display, werden Sie in der Bedienungsanleitung keine Erklärung finden. Das ist kein Versäumnis: Brevilles Fehlercodes stammen aus den internen Servicetabellen, mit denen das Unternehmen seine Reparaturen abwickelt, und diese werden bewusst nicht an Besitzer herausgegeben. Im Vereinigten Königreich vertreibt derselbe Konzern die identische Hardware unter der Marke **Sage** – baugleiche Geräte, nur der Schriftzug unterscheidet sich –, weshalb ein ER-Code an einer Sage Barista Touch exakt dasselbe bedeutet wie an einer Breville. Unsere [Breville-/Sage-Rubrik](https://de.codefixcoffee.com/breville/) deckt die aktuelle Modellpalette ab; dieser Beitrag erklärt die Ordnung hinter der Nummerierung, damit auch ein nie gesehener Code etwas Nützliches verrät.

## Warum Breville die Codes nicht veröffentlicht

Das Nutzerhandbuch behandelt Reinigung und Entkalkung, keine Diagnose. Die vollständigen Tabellen stecken hinter dem Servicemodus jedes Geräts: passwortgeschützte Bildschirme für Techniker mit gespeicherten Fehlerzählern und Live-Werten der Sensoren. Da die Codes ein Reparaturwerkzeug und kein Verbraucherfeature sind, hat Breville sie nie in einem öffentlichen Dokument zusammengetragen, und die meisten Besitzer sehen zeitlebens nur den einzelnen Code, der eine Abschaltung verursacht hat. Größer kann der Kontrast kaum sein: Miele druckt die Bedeutung seiner F-Codes in die Anleitung, weshalb die [Miele-Code-Seiten](https://de.codefixcoffee.com/miele/) das Handbuch direkt zitieren können.

## Die Barista-Touch-Tabelle von ER01 bis ER18

Die Barista Touch (BES880) und die Barista Touch Impress (BES881) – letztere teilt sich die Familie der Steuerplatinen und die Codetabelle – nutzen eine Tabelle mit 18 Einträgen. Kennt man das Schema, liest sie sich beinahe von selbst: Die Sensorcodes treten in **Vierergruppen** auf, eine Gruppe je Sensor, durchlaufend als offener Stromkreis beim Start, offener Stromkreis im Betrieb, Kurzschluss beim Start und Kurzschluss im Betrieb.

- **ER01 bis ER04** – den Temperatursensor der ThermoJet-Heizung („ferro") in seinen vier Varianten aus Offen- und Kurzschluss. [ER01](https://de.codefixcoffee.com/breville/barista-touch-bes880/er01/) ist der Eintrag für den offenen Stromkreis beim Start.
- **ER05 bis ER08** – den Temperatursensor des Milchkrugs, die kleine Sonde im Bereich der Tropfschale, die den Krug überwacht, während der Dampfstab die Milch texturiert. ER05, der offene Stromkreis beim Start, ist der am häufigsten gemeldete Barista-Touch-Code, und alle vier Einträge teilen sich eine Lösung.
- **ER09 bis ER12** – den Durchlauftemperatursensor des Brühwassers, nach demselben Vierer-Muster.
- **ER13 und ER14** – Zählfehler des Durchflussmessers, beim Start und im Betrieb: Die Pumpe lief, doch die Maschine konnte das durchströmende Wasser nicht erfassen.
- **ER15** – eine Kommunikationsstörung zwischen internen Elektronikmodulen; häufig ein gelockertes Flachbandkabel oder ein feuchter Stecker statt einer defekten Platine.
- **ER16 und ER17** – das Mahlwerk: Der Motor hat sich überhitzt und zum Selbstschutz abgeschaltet, danach lief er in den Timeout, ohne seine Aufgabe abzuschließen.
- **ER18** – die E-Fast-Schutzabschaltung, ein elektrischer oder sicherheitsrelevanter Fehler etwa durch Ableitstrom; dieser Code kann zusätzlich den FI-Schutzschalter Ihrer Steckdose auslösen.

## Die Oracle-Familie nummeriert anders

Beim Kauf einer Oracle wächst dieselbe Idee zu einer längeren Tabelle. Oracle (BES980) und Oracle Touch (BES990) teilen sich eine Liste mit 32 Einträgen, wobei die BES980 sie als „Error 1" bis „Error 32" anzeigt und die BES990 ein ER voranstellt. Die ersten sechzehn Einträge folgen der Quartett-Logik über vier Sensoren – Dampfkessel auf 1 bis 4, Kaffeekessel auf 5 bis 8, wobei [Error 8](https://de.codefixcoffee.com/breville/oracle-bes980/error-8/) den im Betrieb kurzschließenden Kaffeekessel-Sensor markiert, dann die beheizte Brühgruppe auf 9 bis 12 und der Dampfstab auf 13 bis 16. Der Rest der Tabelle: nicht heizende Kessel (17 bis 19), Füllstands- und Nachfüllfehler des Dampfkessels (20 und 21), Probleme des Durchflussmessers (22 und 23), Füllstandsonden und Überhitzung (24 bis 27), ein Platinen-Kommunikationsfehler auf 28, das Mahlwerk auf 29 und 30, der Tampermotor auf 31 und ein Dampfkessel-Leck beziehungsweise gescheitertes Nachfüllen auf 32.

Zwei kleinere Tabellen ergänzen die Familie. Die Oracle Jet (BES985) besitzt eine kürzere, eigene Tabelle von E1 bis E19, und die Dual Boiler (BES920) hält zweistellige Codes von 00 bis 12 in einem Selbsttest-Menü verborgen statt im normalen Display – eine Dual Boiler kann also auf einem Fehler stehen, den Sie nie auf dem Bildschirm sehen.

## Das Fehlerprotokoll selbst auslesen

Weil die Tabellen Servicedaten sind, führt der Weg zur Gerätehistorie über dieselben Service-Menüs. Die Zugänge klingen nach Werkstatt, sind aber unter Reparaturbetrieben gut dokumentiert:

- **Barista Touch und Oracle Touch** – an der Steckdose ausschalten, die Power-Taste vorn gedrückt halten, während Sie die Stromversorgung wieder einschalten, beim Erscheinen des Logos loslassen, das Service-Passwort 00000 eingeben und dann entweder den Error Counter für gespeicherte Fehler öffnen oder Live Debug für aktuelle Temperaturen und Füllstände.
- **Barista Touch Impress** – dieselbe Tastenfolge, nur lautet das Service-Passwort hier 02015.
- **Oracle BES980** – bei eingestecktem, ausgeschaltetem Gerät die Tasten 1 TASSE, 2 TASSEN und POWER mindestens eine Sekunde gemeinsam halten; nach dem langen Signalton das SELECT-Rad drücken, um den Error Storage zu öffnen, und die Fehler 1 bis 32 mit ihren gespeicherten Zählern durchblättern.

Betrachten Sie diese Menüs als reine Leseansicht: Protokollieren Sie, was gespeichert ist, lassen Sie Einstellungen unangetastet und löschen Sie das Log erst nach einer abgeschlossenen Reparatur – nur so erkennen Sie, ob ein Code zurückkommt. Für die anschließende Zerlegung bieten Portale wie [ifixit.com](https://www.ifixit.com/) Teardowns und Schritt-für-Schritt-Anleitungen rund um Espressomaschinen.

## Was die Reparaturen typischerweise kosten

Selbst gegen eine unveröffentlichte Tabelle bleibt die Wirtschaftsrechnung vorhersehbar. Temperatursensor-Baugruppen kosten je nach Sensor etwa 25 bis 95 €, wobei Dampfstab- und Milchkrug-Sensoren die teuren sind; O-Ring-Sets liegen bei 10 bis 20 €, ein Milchsensor-Reparaturset bei rund 30 bis 50 € gegenüber 80 bis 95 € für die Original-Baugruppe. Herstellerangebote außerhalb der Garantie bewegen sich bei internen Fehlern üblicherweise zwischen 300 und 500 €, sodass der Sensor-Tausch zum Satz eines unabhängigen Betriebs fast immer der bessere Weg ist.

### Für Deutschland, Österreich und die Schweiz

Auch im deutschsprachigen Raum kommen diese Maschinen als Sage in den Handel; Anleitungen, Entkalkungsvideos und Support erreichen Sie über die Herstellerseite [sageappliances.co.uk](https://www.sageappliances.co.uk/). Behalten Sie ER18 im Hinterkopf: In vielen neueren Elektroinstallationen in Deutschland, Österreich und der Schweiz hängen Steckdosenkreise an einem FI-Schutzschalter mit 30 mA, und genau ein Ableitstromfehler, wie ihn ER18 meldet, kann diese Absicherung auslösen. Fällt in Ihrer Küche also der FI, während die Maschine läuft, lesen Sie das als Symptom und nicht als Zufall.
