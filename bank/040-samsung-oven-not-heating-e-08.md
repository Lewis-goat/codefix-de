---
title: Samsung Herd heizt nicht: E-08 und Verwandte
description: Samsung-Backofen heizt nicht und zeigt E-08? Erst der Reset, dann Heizelement, Temperaturfühler und Relais prüfen — plus die Türschloss-Variante.
---

Ein Backofen, der läuft und trotzdem kalt bleibt, versagt auf traurig vorhersagbare Weise: Die Platine hat eine Temperatur vorgegeben, der Garraum ist nicht gestiegen, und die Maschine hat den Grund protokolliert. Bei Samsung-Herden und Einbaubacköfen ist [E-08](https://de.codefixcoffee.com/samsung/range-wall-oven/e-08/) der Hauptcode für dieses Bild — Ofen heizt nicht, mit Ober- bzw. Unterhitze-Heizelement, Temperaturfühler oder einem Relais auf der Platine als Verdächtigen. Darum herum liegt eine kleine Familie verwandter Codes, die den Fehler weiter eingrenzt. Dieser Beitrag geht sie in der Reihenfolge durch, in der sich die Prüfung lohnt — beginnend mit dem Schritt, den alle überspringen.

## Zuerst: der Reset am Schutzschalter

Bevor Sie irgendetwas folgern: Trennen Sie die Spannung am Leitungsschutzschalter für drei Minuten und schalten Sie sie wieder zu. Das ist kein Aberglaube — eine Herd-Platine, die in einen schlechten Zustand geraten ist, kann einen Heizfehler protokollieren, den sie sonst nicht hätte, und ein sauberer Stromzyklus löscht ihn. Kehrt E-08 beim nächsten Backversuch zurück, ist der Fehler echt, und Sie gehen weiter. Derselbe Dreiminuten-Reset eröffnet zudem die Diagnose für nahezu jeden Code in der [Samsung-Ofen-Codeliste](https://de.codefixcoffee.com/samsung-oven-error-codes/) — eine Gewohnheit, die sich lohnt.

### Besonderheit im DACH-Raum: Festanschluss und 400 Volt

In Deutschland und Österreich hängen viele Herde im Festanschluss — ein Netzstecker zum Ziehen gibt es dann nicht, der Dreiminuten-Reset läuft stattdessen über die Leitungsschutzschalter bzw. den Herd-Automaten im Sicherungskasten. Herde werden hierzulande üblicherweise mit Drehstrom 400 V versorgt, und das Heizelement liegt zwischen zwei Außenleitern: Fällt eine Phase aus, etwa durch einen ausgelösten Automaten, bleibt der Ofen kalt, obwohl alles andere normal wirkt. Auch in der Schweiz werden Herde mit 400 V betrieben — prüfen Sie deshalb zuerst, ob alle zum Herd gehörenden Automaten eingeschaltet sind, bevor Sie an Bauteilen denken.

## Das Heizelement

Das Unterhitze-Heizelement ist das Arbeitstier am Boden des Garraums, und es versagt sichtbar. Bei laufendem Ofen sollte das Element auf seiner ganzen Länge gleichmäßig glühen. Ein sichtbarer Bruch, eine Blase oder eine Brandstelle ist eine Diagnose, die Sie mit bloßem Auge treffen: ersetzen. Ein Heizelement kostet 30 bis 60 € und gehört zu den lohnendsten Ofenreparaturen überhaupt. Glüht es einwandfrei, hält der Ofen die Temperatur aber trotzdem nicht, ist das Element entlastet und der Fühler ist als Nächstes dran — der komplette Entscheidungsweg steht auf der [E-08-Diagnoseseite](https://de.codefixcoffee.com/samsung/range-wall-oven/e-08/).

## Der Temperaturfühler

Die Spitze des Fühlers misst die Garraumtemperatur und meldet sie der Platine als Widerstandswert. Bei Raumtemperatur liest ein gesunder NTC-Sensor rund 1080 Ohm — und diese Zahl ist die gesamte Prüfung:

1. Strom am Leitungsschutzschalter abschalten.
2. Den Fühler aus der Rückwand des Garraums schrauben (zwei Schrauben) und abziehen.
3. Durchmessen: rund 1080 Ohm bei Raumtemperatur ist gesund.
4. Passt der Wert, den Stecker neu aufsetzen; weicht er deutlich ab, den Fühler ersetzen.

Zwei verwandte Codes verraten ohne Messgerät, in welche Richtung der Fühler ausgefallen ist. E-27 heißt, der Fühler liest offen — Widerstand zu hoch, über etwa 2950 Ohm —, also ein defekter Fühler oder ein loser Stecker. E-28 heißt Kurzschluss, unter etwa 930 Ohm — ein kurzgeschlossener Fühler oder ein gequetschter Kabelbaum hinter dem Ofen. Der Fühler selbst kostet 20 bis 40 € und wird von innen in den Garraum geschraubt.

## Das Relais auf der Platine

Glüht das Element und misst der Fühler korrekt, bleibt die Relaisplatine übrig: Die Platine schaltet die Spannung zum Element nicht durch. Ein Relais, das nie schließt, sieht von innen genau so aus wie ein totes Element. Das ist das Ergebnis mit 100 bis 200 € Kosten, und bei einem älteren Herd ist das der Punkt, an dem der Vergleich zwischen Reparaturangebot und Gerätewert vernünftig wird.

## Die Türschloss-Variante

Ein Vorbehalt, bevor Sie Teile kaufen: Bei einigen Modellen listet der Hersteller E-08 als Türschloss-Fehler statt als Heizfehler — das motorisierte Schloss der Selbstreinigung statt des Backkreislaufs. Sehen Sie im Handbuch Ihres Modells nach — die offiziellen Anleitungen und Hilfestellungen finden Sie im [Support-Bereich von samsung.com](https://www.samsung.com) —, bevor Sie ein Element bestellen. Der zugehörige Code für Schlossprobleme ist E-0E (angezeigt als E-0E oder FL); er erscheint meist nach einem Selbstreinigungs-Lauf, wenn der Schalter klemmt oder der Schlossmotor versagt — die Baugruppe kostet 40 bis 90 €. Öffnen Sie die Tür in keinem dieser Fälle mit Gewalt: Lassen Sie den Ofen vollständig abkühlen, heiß entriegelt er nicht.

## Der Code für das umgekehrte Problem

Während Sie in dieser Fehlerfamilie unterwegs sind, sollten Sie [E-0A](https://de.codefixcoffee.com/samsung/range-wall-oven/e-0a/) kennen: den überhitzenden Ofen. Es wirkt wie eine andere Beschwerde, teilt aber zwei Verdächtige mit E-08 — einen falsch messenden Fühler (diesmal zu niedrig) oder ein klebendes Relais, das das Element nicht abschaltet. Behandeln Sie E-0A mit mehr Dringlichkeit als einen Kalt-Ausfall: Ein klebendes Relais heißt, das Element bleibt eingeschaltet — also sofort die Spannung am Schutzschalter trennen und den Ofen bis zur Reparatur nicht benutzen.

## Was die Reparaturen kosten

Unterhitze-Element 30 bis 60 €, Fühler 20 bis 40 €, Türschloss-Baugruppe 40 bis 90 €, Relaisplatine 100 bis 200 €. Element und Fühler sind bei jedem vernünftigen Gerätealter ein klares Ja; die Platine ist eine Abwägung. Ein Techniker-Heimbesuch kostet 120 bis 250 € für die Diagnose zzgl. des Teils — fair für die Bestätigung, welche der drei Sie wirklich brauchen.
