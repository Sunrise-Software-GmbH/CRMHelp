---
title: Bestellungen
has_children: false
grand_parent: Verkauf, Einkauf und Lager
parent: Einkauf
nav_order: 20
---

# Bestellungen

Die Bestellung ist die Basis der weiteren Belege, wie E-Lieferschein, E-Rechnung und E-Gutschrift für Lager, Menge, Rabatt und Preis. Eine Bestellung kann durch eine Anfrage übergeleitet oder manuell erstellt werden. Man kann diese auch direkt aus einem Verkaufs Angebot oder Auftrags Beleg überleiten.

**Bestellung Status:**

- **In Bearbeitung:** Die Bestellung wird noch bearbeitet und wurde noch nicht versendet.
- **Versendet:** Die Bestellung wurde an den Lieferanten weitergeleitet.
- **Abgeschlossen**

**Button *"Versenden"*:** Bei der Aktion *"Versenden"* wird der Status der Bestellung auf Versendet gewechselt und eine E-Mail geöffnet mit dem Bestellbeleg als PDF Datei im Anhang. Siehe Bestellungs Status **Versendet**.

Belegs Überleitung mit Button *"Lieferschein erzeugen"* oder über das Menü *"Aktivität neu > Einkauf > Lieferschein oder Retourschein"* überleiten in einen Einkaufs Lieferschein oder Retourschein [Siehe E-Lieferscheine und E-Retourscheine](./E-Lieferscheine%20und%20E-Retourscheine.md).

Bei der Übernahme der Bestell Positionen in einen E-Lieferschein wird immer geprüft, ob es einen E-Lieferschein oder mehrere Teil- E-Lieferscheine gibt. Es wird eine Dialog mit folgenden Optionen geöffnet:

- **Positionszeilen übernehmen:** Kann aktiviert werden, damit die Positionen aus der Bestellung in den E-Lieferschein übernommen werden. Wird diese Option nicht aktiviert, können die Positionen manuell im E-Lieferschein eingegeben werden.
- **nur Zeilen mit lagergeführten Artikel übernehmen:** Es werden nur Positionen übernommen, die auch im Lager geführt werden.
**nur noch nicht gelieferte Zeilen übernehmen:** Existieren mehrere Teil- E-Lieferscheine, werden nur die Mengen übernommen, die noch nicht ausgeliefert wurden (Restmenge der Auftragspositionen zu den bereits gelieferten E-Lieferscheinpositionen)

Beleg über das Menü *"Aktivität neu > Einkauf > E-Rechnung"* überleiten in eine Einkaufs E-Rechnung: Siehe E-Rechnungen und E-Gutschriften.
Es wird eine Dialog mit folgenden Optionen geöffnet:

Verrechnung / Fakturierung:

- **auf Basis E-Lieferschein:** Gibt es zu einer Bestellung einen E-Lieferschein, oder mehrere Teil-E-Lieferscheine, wird die E-Rechnung immer auf Basis des E-Lieferscheins erstellt. Man kann zu den jeweiligen Teil-E-Lieferscheinen auch Teil-E-Rechnungen erstellen. Ob man in eine E-Rechnung mehrere Teil-E-Lieferscheine übernimmt oder pro E-Lieferschein eine E-Rechnung erstellt, ist Sache der Vereinbarung mit dem jeweiligen Lieferanten. Bei der Übernahme der Lieferschein Positionen in eine Rechnung wird immer die tatsächliche Menge übernommen.
- **auf Basis Bestellung:** Wenn kein E-Lieferschein zu einer Bestellung existiert, wird die E-Rechnung immer auf Basis der Bestellung erstellt. Auch hier kann man die Bestellung auf mehrere Teilrechnungen splitten. Bei der Übernahme der Bestell Positionen in eine E-Rechnung wird immer geprüft, ob es eine E-Rechnung oder mehrere Teil-E-Rechnungen gibt. Existieren mehrere Teil-E-Rechnungen wird nur die Differenzmenge übernommen.

**Belegs Überleitung in Verkauf:**

Aus einer Bestellung kann man über das Menü *„Aktivität neu > Verkauf > Auftrag"* die Positionen in einen Verkaufs Auftrag überleiten, um einen weiterführenden Verkaufsprozess einzuleiten. [Siehe Aufträge](../Verkauf/Aufträge.md).

Belegs Überleitung aus Verkauf:
Aus den Belege Verkauf Angebot oder Auftrag kann man direkt überleiten in eine Einkaufs Bestellung. [Siehe Verkauf](../Verkauf/index.md).

**Lieferstatus in der Bestellliste für lagergeführte Artikel:**

- **leer:** Es ist eine Bestellung ohne lagergeführte Artikel.
- **noch nichts geliefert:** Es ist eine Bestellung mit lagergeführten Artikel. Noch kein E-Lieferschein wurde erstellt.
- **teilweise geliefert:** Lieferung erfolgt in Teilschritten bis die gesamte Menge der Bestellung abgewickelt ist. Ein Teil-E-Lieferschein wurde bereits erstellt.
- **alles geliefert:** Lieferung ist vollständig abgearbeitet. Es ist die gesamte Bestellmenge in einem oder mehreren E-Lieferscheinen vorhanden.
