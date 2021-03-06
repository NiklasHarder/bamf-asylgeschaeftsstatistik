# bamf-asylgeschaeftsstatistik - Report

## Zu den Daten

Das BAMF (Bundesamt für Migration und Flüchtlinge) veröffentlicht [monatlich die Asylgeschäftsstatistik](http://www.bamf.de/DE/Infothek/Statistiken/Asylzahlen/Asylgesch%C3%A4ftsstatistik/asylgeschaeftsstatistik-node.html). Das ist eine wichtige und aktuelle Datenquelle.

Eine Kennzahl ist die "Schutzquote", die die Frage beantwortet, wie viel Prozent der Asylantragssteller bleiben dürfen. Die in den BAMF-Berichten erscheinende "Gesamtschutzquote" errechnet sie als Summe aller positiven Entscheide geteilt durch alle Anträge. In dieser "Summe aller Anträge" sind allerdings auch die enthalten, die sich anderweitig erledigt haben - durch Wegzug, Heirat, Weiterreise oder anderen Gründen. Das ist irritierend. Wenn von 1000 Anträgen 800 positiv entschieden wurden, bedeutet das nicht, dass 200 negativ entschieden wurden - sondern dass sich vielleicht 150 anderweitig erledigt haben und 50 negativ entschieden wurden. Deshalb rechnen Eurostat und andere Stellen diese nicht inhaltlich geprüften Asylanträge heraus und geben die "bereinigte Schutzquote" an als die positiven Entscheidungen geteilt durch alle inhaltlich behandelten Anträge. (https://de.wikipedia.org/wiki/Gesamtschutzquote, http://www.bamf.de/DE/Infothek/Statistiken/Asylzahlen/asylzahlen-node.html)

Wir wollen:

1. Die Daten aus den Berichten als CSV herausziehen und damit weiterverarbeitbar machen
2. Die bereinigte Schutzquote errechnen
3. Das Ergebnis grafisch darstellen
4. und online stellen.

## Zur Technik
Daten kommen von https://www.bamf.de/SharedDocs/Anlagen/DE/Downloads/Infothek/Statistik/Asyl/201603-statistik-anlage-asyl-geschaeftsbericht.html

0. Bei Upload des neuen Berichts wird ein email verschickt
1. In docker mit php Script:
2. Download des PDF, Weiterverarbeitung per tabula , http://tabula.technology, zu csv, bereinigt und auf github geschoben
3. Erklärt gemäss Datapackage http://dataprotocols.org/data-packages , mit Datapackage bauen: http://datapackagist.okfnlabs.org
4. In Spreadsheet: Berechnung, Visualisierung

## Zum Projekt
Entstanden auf einem Datathon in Muenchen am 07.05.2016

