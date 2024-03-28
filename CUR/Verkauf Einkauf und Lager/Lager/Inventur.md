---
title: Inventur
has_children: false
grand_parent: Verkauf, Einkauf und Lager
parent: Lager
nav_order: 20
---

## Inventur

Eine Inventur wird durchgeführt, um die in der Datenbank hinterlegte Lagermenge mit dem tatsächlichen Lagerbestand zu korrigieren.

**Inventurtyp:**

- **Korrektur:** der Lagerstand eines bestimmten Artikels wird korrigiert.
- **Monatsabschluss:** gesamte Inventur der Buchhaltungseinheit für den Monatsabschluss.
- **Jahresabschluss:** gesamte Inventur der Buchhaltungseinheit für die Bilanz.

Über folgende Möglichkeiten können die Artikel in die Inventur übernommen werden:

- ![Lager](../../Pictures/Symbol_Store.svg)...**Gesamten Lagerstand übernehmen:** Es werden alle in den verschiedenen Lagern befindlichen Artikel in die Inventur übernommen. Dabei werden auch die jeweiligen Ausprägungen eines Artikels (zum Beispiel die Länge) berücksichtigt.
- ![Lager](../../Pictures/Symbol_InventoryInsertStore.svg )...**Lagerstand des Artikels einfügen:** Eines oder mehrerer Artikel werden nach Auswahl in der Inventur aufgenommen. Auch hier werden die verschiedenen Ausprägungen und Lager berücksichtigt.
- ![Lager](../../Pictures/Symbol_Article.svg)...**Artikel neu:** Nach Auswahl eines oder mehrerer Artikel und eines Lagers werden diese in die Inventur übernommen. Vorzugsweise handelt es sich dabei um Artikel, die noch nicht im Lager sind, oder deren Ausprägung noch nicht im Lager vorhanden ist.
Diese neu eingefügten Zeilen werden in Fettschrift dargestellt, da die Eingabe einer Ausprägung notwendig sein kann. Befindet sich der jeweilige Artikel bereits im ausgewählten Lager, dann wird dieser mit seinen Ausprägungen eingefügt.
- ![Lager](../../Pictures/Symbol_Copy.svg)...**Position kopieren**: die markierte Zeile wird kopiert, um zum Beispiel den Artikel mit einer anderen dynamischen Ausprägung in der Inventur aufzunehmen.

Beim Einfügen der Artikel in die Inventur bleibt die Inventurmenge leer. Diese sollte vom Benutzer eingetragen werden. Entspricht die Inventurmenge der aktuellen Lagermenge kann über die Funktion *"Lagermenge kopieren"* der aktuelle Lagerstand übernommen werden. Dabei werden die Werte nur in den Zeilen kopiert, in denen noch keine Inventur-Menge eingegeben wurde. Bereits vorgenommene Eingaben bleiben erhalten.

**Einzelbewertung:** bei Aktivierung der Einzelbewertung stehen zusätzliche *"Preis"* Spalten zur Verfügung. Der *"Inv. Ø EK Einzelpreis"* kann in der Liste auch geändert werden, um damit den Wert des Lagers zu korrigieren.
Diese Option steht nur bei abgeschlossenen Inventuren zur Verfügung.
Hinweis: über das Kontext-Menü *"Mehrfachbearbeitung Inv. Ø EK Einzelpreis"* kann der durchschnittliche Einzelpreis auch für mehrere Zeilen geändert werden.

**ACHTUNG:** Wenn Artikel mit verschiedenen Ausprägungen verwendet werden (zum Beispiel derselbe Artikel ist mit 4m und mit 6m Länge im Lager) oder bei Chargen/Seriennummern Artikel müssen in der Inventur alle Ausprägungen des Artikels enthalten sein. Dies gilt auch wenn sich die Anzahl nicht von der letzten Inventur unterscheidet, da in der Artikelliste der Lagerstand zu den in der Inventur enthaltenen Ausprägungen dargestellt wird.
Daher kann das Lager bei diesen Artikel nicht geändert werden.

**Solange sich ein Artikel in einer noch nicht abgeschlossenen Inventur befindet, ist er für die Verwendung in Lieferscheinen gesperrt.**
Beim *"Abschließen"* einer Inventur werden die Lagerstände korrigiert. Anschließend kann die Inventur nicht mehr geändert werden.
