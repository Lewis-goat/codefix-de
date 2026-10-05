---
title: Breville Dual Boiler 00–12: die zweistelligen Codes
description: Breville Dual Boiler BES920 meldet Fehler als Codes 00 bis 12 in einem versteckten Selbsttest-Menü: Bedeutung der Blöcke, Dampf- vs. Brühseite, Lösungen.
---

Die meisten Espressomaschinen von Breville melden ihre Störungen auf dem normalen Display: Die Barista Touch zeigt ER-Codes, die Oracle meldet Error-Codes, die Oracle Jet arbeitet mit E-Nummern. Der **Dual Boiler BES920** macht es anders. Seine Fehlertabelle besteht aus nüchternen zweistelligen Codes, **00 bis 12**, und sie liegt in einem versteckten Selbsttest-Menü, nicht auf dem Alltagsbildschirm. Wer die Tastenkombination nicht kennt, sieht diese Codes nie — auch nicht nach tagelangem Beobachten der Frontblende.

Es lohnt sich, das Nummernschema zu verstehen, denn es ist ordentlich gebaut: Der Block, in dem ein Code liegt, verrät die Art der Störung, und innerhalb des Blocks benennt der Code das Bauteil, das sich meldet.

## Das Fehlerprotokoll auslesen

1. Schalten Sie die Maschine an der Steckdose aus.
2. Halten Sie **EXIT** und **MANUAL** gedrückt, während Sie die Spannung wieder zuschalten; das Selbsttest-Menü erscheint.
3. Gehen Sie mit **MENU** zu Punkt 3, dem Fehlerprotokoll. Punkt 4 zeigt den Füllstand der Kessel, angezeigt als LLL (niedrig) oder HHH (hoch).
4. Blättern Sie im Protokoll mit **MENU** durch die Codes 00 bis 12, jeweils mit gespeichertem Zählerstand.
5. Bei ErSt halten Sie **MANUAL** gedrückt, bis die Maschine piept, um die gespeicherten Codes zu löschen; der Tassenzähler bleibt dabei unberührt.

Die Zählerstände sind so wichtig wie die Codes selbst: Eine Störung mit dem Zählerstand 1 aus dem Vorjahr ist Geschichte; eine Störung, deren Zähler jede Woche steigt, ist ein akutes Problem im Wachsen.

## Was die 00er-Familie abdeckt

Die Codes **00 bis 05** bilden den Block der Temperatursensoren, angelegt als drei Paare. Innerhalb jedes Paars bedeutet die niedrigere Zahl, dass der Sensor **nicht erkannt** wird — die Platine liest einen offenen Stromkreis —, die höhere Zahl, dass er als **Kurzschluss** gelesen wird:

- **00 und 01** — Temperaturfühler Dampfkessel, erst nicht erkannt, dann Kurzschluss.
- **02 und 03** — Temperaturfühler Brühkessel, erst nicht erkannt, dann Kurzschluss.
- **04 und 05** — Temperaturfühler der Brühgruppenheizung, erst nicht erkannt, dann Kurzschluss.

Die BES920 bringt zwei Edelstahlkessel plus eine beheizte Brühgruppe mit — die drei Sensoren überwachen also genau die drei beheizten Zonen der Maschine. Die [Seite zu Code 00](https://de.codefixcoffee.com/breville/dual-boiler-bes920/00/) behandelt den Sensor des Dampfkessels, und ihre praktischen Ratschläge gelten für die anderen fünf genauso: Setzen Sie den Sensor-Stecker neu auf und inspizieren Sie ihn, bevor Sie Teile kaufen, und achten Sie auf Feuchtigkeit — Wasser an einem Verbinder liest sich je nach Position als offener Kreis oder als Kurzschluss. Original-NTC-Sensor-Sätze kosten je nachdem, um welchen der drei es geht, etwa 25 bis 90 €; O-Ring-Sets gibt es für 10 bis 20 € und sind ohnehin oft der wahre Übeltäter.

## Dampfseite gegen Brühseite

Der Rest der Tabelle teilt sich entlang derselben Baugrenze wie die Sensorpaare:

- **Dampfkessel:** 06 (Pumpenproblem beim Start), 07 (Füllstands- oder Pumpenstörung) und 11 (erkannte Überhitzung).
- **Brühkessel — die Brühseite:** 08 (Pumpen- oder Durchflussstörung), 09 (Füllstandsstörung) und 10 (erkannte Überhitzung).
- **Brühgruppe:** 12 (erkannte Überhitzung).

### Codes, die gemeinsam auftreten

Diese Störungen greifen ineinander — deshalb schlägt das Lesen des gesamten Protokolls das Lesen eines einzelnen Codes. Code 08 bedeutet: Die Pumpe lief, aber der Durchflussmesser sah nichts — meistens Kalk auf dem Flügelrad des Durchflussmessers oder eine kleine Pumpe, die brummt, ohne Wasser zu bewegen; in beiden Fällen ist die Entkalkung der erste Schritt. Code 11, eine Überhitzung des Dampfkessels, folgt meist auf einen Kessel, der nicht nachgefüllt wird — prüfen Sie, ob auch 07 oder 08 einen Zählerstand haben —, weil das Heizelement einen niedrigen Kessel weiterheizt; die andere Ursache ist eine undichte Fühlerdichtung. Lesen Sie vor jeder Bestellung Punkt 4 im Selbsttest-Menü: Ein Füllstand, der nicht zu dem passt, was Sie beim Füllen der Maschine hören, verrät, auf welcher Seite die Störung wirklich liegt.

Code 12, die überhitzende Brühgruppe, ist das seltenere Ende der Tabelle — und der Code, bei dem wiederholtes Auftreten am schwersten wiegt: Eine Überhitzung, die immer wiederkehrt, deutet darauf, dass die Leistungsplatine einen Heizer eingerastet lässt, nicht auf einen driftenden Sensor. Die [Seite zu Code 12](https://de.codefixcoffee.com/breville/dual-boiler-bes920/12/) geht den Fall durch.

## Was die Teile kosten

- Entkalker für die Durchfluss- und Füllstandscodes: rund 10 € — und er behebt einen echten Anteil von ihnen.
- Füllpumpe: 30 bis 60 €.
- Fühler mit O-Ring-Set für den Dampfkessel: etwa 85 €; O-Ring-Sets allein 10 bis 20 €.
- Thermosicherung: 10 bis 20 € — aber klären Sie zuerst, warum sie ausgelöst hat.
- Triac oder Leistungsplatine: 80 bis 150 €.

Für interne Defekte liegen Reparaturangebote außerhalb der Garantie häufig bei 300 bis 500 € und mehr — eine Pumpe oder ein Sensor lohnt sich also als Eigenleistung; bei einer Platine in einer älteren Maschine holen Sie vorher ein Angebot ein. Wasser und Netzstrom teilen sich den oberen Bereich des Kessels: Ziehen Sie den Stecker, bevor Sie Fühler anfassen.

### Praxis-Tipp für den DACH-Raum

Im deutschsprachigen Raum firmieren die Geräte unter dem Namen Breville, während dieselben Maschinen in Großbritannien als Sage by Heston Blumenthal verkauft werden — technisch sind sie identisch, nur Marke und Support unterscheiden sich. Anleitungen und Ersatzteilinformationen der Schwestergeräte finden Sie deshalb auch auf [sageappliances.co.uk](https://www.sageappliances.co.uk); Schritt-für-Schritt-Reparaturleitfäden mit Fotos gibt es zusätzlich auf [ifixit.com](https://www.ifixit.com). In Regionen mit hartem Leitungswasser — weite Teile Süddeutschlands, Österreichs und der Schweiz — verkürzt sich zudem das Entkalkungsintervall spürbar, und die Codes 08 und 09 sind hierzulande häufig reine Kalkfolgen.

Wie die übrigen Maschinen des Programms ihre Störungen formulieren, steht im [Breville-Bereich](https://de.codefixcoffee.com/breville/) — die Maschinen der ER-Familie teilen viele Diagnoseideen, aber nicht die Nummerierung.
