# Normalisierung

Normalisierungen von relationalen Datenschemas werden verwendet, um Redundanzen zu verringern und Anomalien (in Kontext: ungewollte Veränderungen an Daten) zu bekämpfen. 

In der Praxis hat sich das Normalisieren bis auf die 3. Normalform als Performancesteigernd erwiesen, während darauffolgende Normalisierungen die Zugriffsgeschwindigkeit negativ beeinflussen.

## 0. Normalform - Tabellisierung!

* Alle Datenelemente sind in einer Tabelle zusammengefasst und aufgelistet.

## 1. Normalform - Atomarisierung!

* Jeder Information der Tabelle wird eine eigene Spalte zugewiesen.

> in Einfach: Listen aufbrechen, Listenelemente zu neuen Tabellenspalten.

## 2. Normalform - Relationierung!

* In 1. Normalform
* Jedes Attribut bezieht sich vollfunktional auf den Primärschlüssel der Tabelle

> in Einfach: Neue thematische Untertabellen mit jeweiligem Primärschlüssel erstellen, jeweilige Felder aus alter Tabelle lösen und die Beziehungen mit jeweiligen Fremdschlüsseln kennzeichnen.

## 3. Normalform

* In 2. Normalform
* Jedes Attribut ist ausschließlich vom jeweiligen Primärschlüssel abhängig.

> in Einfach: Überprüfung der Abhängigkeit von Nicht-Primärschlüssel vornehmen und weitere Untertabellen erstellen.

## Boyce-Codd-Normalform (BCNF)
Benannt nach den Erfindern der relationalen Datenbanken.

* gleichzeitig in 3. Normalform
* Jeder Fremdschlüssel bezieht sich alleine auf den Primärschlüssel.

## 4. Normalform

* in BC Normalform
* Jede Tabelle beinhaltet nur thematisch passende Felder.

## 5. Normalform

* In 4. Normalform
* Jede Trivialität wird aufgelöst.