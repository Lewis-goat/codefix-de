---
title: Breville/Sage Oracle – Dampffehler und ER-Codes richtig einordnen
description: Dampf- und ER-Codes der Breville/Sage Oracle – welche Spülroutine zuerst hilft, wann Kalk die eigentliche Ursache ist und was die Teile kosten.
---

Kein Bereich einer Breville Oracle arbeitet härter als die Dampfseite: ein Dampfkessel aus Edelstahl, ein Stab, der Milch automatisch texturiert, Füllstandsonden und eine Nachfüllpumpe, alle täglich auf Temperatur. Dort entsteht auch ein großer Teil der Fehlercodes. Die Oracle-Familie nutzt eine Servicetabelle mit 32 Einträgen, die Breville nicht veröffentlicht; im Vereinigten Königreich trägt dieselbe Hardware das **Sage**-Logo, und die Codes sind identisch. Bevor Sie auf ein defektes Teil schließen, arbeiten Sie die günstigen Prüfungen ab: Die meisten Abschaltungen auf der Dampfseite sind eine verstopfte Dampfdüse, eine unterlassene Spülung oder Kalk auf einer Sonde. Die [Übersicht der Breville- und Sage-Modelle](https://de.codefixcoffee.com/breville/) hilft bei der Einordnung.

## Wo die Dampf-Codes in der Oracle-Tabelle liegen

Oracle (BES980) und Oracle Touch (BES990) teilen sich eine Tabelle; die BES980 zeigt die Einträge als „Error 1" bis „Error 32", die BES990 stellt ein ER davor. Die dampfseitigen Einträge sammeln sich an fünf Stellen:

- **Error 1 bis 4** – den Temperatursensor des Dampfkessels, durchlaufend als offener Stromkreis beim Start, Verlust im Betrieb und Kurzschluss in beiden Situationen. Ein Sensor, vier Meldewege.
- **Error 13 bis 16** – dasselbe Quartett für den Temperatursensor des Dampfstabs, jene Sonde, die das Auto-Texturieren bei der richtigen Milchtemperatur stoppt. Sie sitzt am nassesten Ort der Maschine.
- **Error 18** – der Dampfkessel heizt nicht ordnungsgemäß auf.
- **Error 20 und 21** – Wasserstand des Dampfkessels oder Probleme der Nachfüllpumpe sowie eine Füllstandsmessung, die nicht zum erwarteten Bild der Platine passt.
- **Error 26** – der Dampfkessel wurde über die Zieltemperatur hinaus heiß; **Error 32** – ein Dampfkessel-Leck oder ein gescheitertes Nachfüllen.

Nicht alles in Stabnähe gehört zur Dampfseite: Die Codes 5 bis 8 zählen zum Temperatursensor des Kaffeekessels, [Error 8](https://de.codefixcoffee.com/breville/oracle-bes980/error-8/) ist dessen Eintrag für den Kurzschluss im Betrieb. Das gespeicherte Protokoll hilft, die Familien zu trennen – an der BES980 öffnen Sie bei ausgeschalteter Maschine mit den gemeinsam gehaltenen Tasten 1 TASSE, 2 TASSEN und POWER den Error Storage und blättern durch alle 32 Codes samt Zählerständen.

## Die erste Prüfung – die Spülroutine

Schwacher oder stotternder Dampf oder ein Code unmittelbar nach einem Milchgetränk verweist eher auf die Düse als auf den Kessel:

1. Ziehen Sie den Netzstecker und lassen Sie den Dampfstab abkühlen.
2. Schrauben Sie die Dampfdüse ab und weichen Sie sie in heißem Wasser mit einem Schuss Entkalker ein; befreien Sie jede Öffnung mit der Nadel des Reinigungswerkzeugs.
3. Führen Sie die Dampfspülung durch – rund zehn Sekunden Dampf in die Tropfschale ohne aufgeschraubte Düse, danach noch einmal mit.
4. Spülen Sie den Stab künftig nach jeder Milchrunde aus; getrocknete Milch in der Düse ist der Auslöser der meisten dieser Abschaltungen.

Überwacht die Maschine den Dampfdruck – wie die Oracle Jet mit ihrem Code E16 –, kann eine verkrustete Düse den Fehler werfen, bevor Sie den nachlassenden Dampf überhaupt bemerken.

## Härtegrad, Kalk und die Füllstandsonden

Wo das Wasser hart ist, schreibt der Kalk eigene Fehlercodes. Die Füllstandsonden des Dampfkessels sitzen ständig in heißem Wasser, und eine Kalkschicht isoliert sie so weit, dass die Platine „kein Wasser" liest, obwohl der Kessel voll ist – der klassische Weg zu Error 20 oder 21 und zum Nachfüllversagen von Error 32. Kalk lagert sich auch im Dampfweg und am Eingang der Nachfüllpumpe ab. Eine vollständige Entkalkung einschließlich des Dampfkessel-Zyklus ist die günstigste Diagnose, die Sie fahren können, und sie beseitigt erstaunlich viele dieser Codes im Alleingang.

Das Schwestermodell der Reihe bestätigt den Punkt: Die Dual Boiler versteckt ihre Codes 00 bis 12 in einem Selbsttest-Menü, und [Code 00](https://de.codefixcoffee.com/breville/dual-boiler-bes920/00/) – der Dampfkessel-Sensor wird nicht erkannt – steht dort an der Spitze einer Tabelle, deren Füllstands- und Nachfüll-Einträge unter hartem Wasser exakt dasselbe Verhalten zeigen.

### Wasserhärte in Deutschland, Österreich und der Schweiz

In Deutschland wird die Wasserhärte in Grad deutscher Härte (°dH) angegeben, und ab etwa 14 °dH gilt Wasser als hart – große Teile Bayerns, Baden-Württembergs und des westlichen Deutschlands liegen darüber, sodass ein Dampfkessel dort ohne regelmäßige Entkalkung zügig verkrustet. Auch in Österreich ist das Leitungswasser vielerorts kalkhaltig, während es in weiten Teilen der Schweiz deutlich weicher ausfällt. Ihren genauen Härtegrad nennt Ihnen der örtliche Wasserversorger; daraus leiten Sie das Entkalkungsintervall und, falls vorhanden, die Härteeinstellung der Maschine ab. Die offiziellen Entkalkungsanleitungen von Sage finden Sie im Support-Bereich von [sageappliances.co.uk](https://www.sageappliances.co.uk/).

## Entkalken statt Zerlegen – und wo die Grenze liegt

Erst entkalken, dann zerlegen – aber kennen Sie die Grenze der Entkalkung:

- **Zuerst entkalken** bei Füllstands-, Sonden- und Nachfüll-Codes (20, 21, 32), bei schwachem Dampf ohne Code und bei jeder Maschine, deren letzte Entkalkung mehr als drei Monate zurückliegt. Kosten: eine Flasche Entkalker.
- **Entkalkung hilft nicht**, wenn ein Sensor-Code auf frisch entkalkter, warmer Maschine sofort zurückkommt – ob als Dampfkessel-Eintrag der Codes 1 bis 4 oder als [Error 8](https://de.codefixcoffee.com/breville/oracle-bes980/error-8/) auf der Kaffee-Seite. Ein Code, der die Entkalkung übersteht, verweist auf den Sensor, sein Kabel oder einen Stecker.
- **Anhalten und Dichtungen prüfen**, wenn Error 26 wiederkehrt: Ein undichter Dampfsonden-O-Ring lässt heißen Dampf an das Sensorkabel gelangen und ahmt einen durchgehenden Kessel nach. Neue Sonden-O-Ringe sind billig; eine Triac-Platine, die die Heizung nicht mehr abschaltet, ist es nicht.
- **Error 18** an einer Maschine, die überhaupt keinen Dampf mehr erzeugt, liegt meist an der Heizseite – Thermosicherung, Heizelement oder Platine – und nicht am Kalk; führen Sie ihn als Reparatur, nicht als Reinigung.

Für das Zerlegen halten Portale wie [ifixit.com](https://www.ifixit.com/) Teardowns und Schritt-für-Schritt-Anleitungen für Espressomaschinen bereit.

## Was die Teile kosten

Originale Temperatursensor-Baugruppen kosten je nach Sensor etwa 25 bis 95 €; Dampfstab-Baugruppen, die ihren Sensor einschließen, liegen bei rund 60 bis 95 €; ein Satz aus Sonde und O-Ringen bei etwa 85 € und eine Nachfüllpumpe bei 30 bis 60 €. Dem stehen Herstellerangebote für interne Fehler außerhalb der Garantie von üblicherweise 300 bis 500 € gegenüber – die bessere Rechnung lautet daher fast immer: zuerst die Entkalkerflasche, danach die Reparatur auf Sensor-Ebene.
