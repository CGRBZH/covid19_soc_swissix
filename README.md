
# Gesellschaftsmonitoring COVID19, Daten SwissIX

Daten zum täglichen Datenvolumen über [SwissIX Swiss Internet Exchange](https://www.swissix.ch/) im Rahmen des Projekts [Gesellschaftsmonitoring COVID19](https://statistikzh.github.io/covid19monitoring/)

## Datenlieferant

[source] SwissIX Swiss Internet Exchange

## Beteiligte

Corinna Grobe <corinna.grobe@statistik.ji.zh.ch>, Statistisches Amt Kanton Zürich


## Indikatorbeschreibung

[topic] Soziales

[variable_short] daily_volume

[variable_long] Tägliches Internet-Traffic-Volumen

[location] Schweiz (default)

[unit] Terabit pro Tag

[update] täglich

[description] https://github.com/CGRBZH/covid19_soc_swissix (to change)

## Open data

Kann die Variable OGD gestellt werden?

[public] Ja

## Struktur der Basisdaten:

Datei `https://ixpmanager.swissix.ch/swissix_daily_volume.txt`

* `date`: Datum, Format yyyy-mm-dd
* `value`: Anzahl, nur Ganzzahlen verwenden

## Vorgehen

* Automatisches Update des Datenfiles `swissix_daily_volume.txt` durch SwissIX, in der Regel täglich.
* R-Skript `prepareDate.R` zum Generieren der erforderlichen Datenstruktur.
