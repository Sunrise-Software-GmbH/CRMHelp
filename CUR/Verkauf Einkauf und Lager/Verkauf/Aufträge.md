---
title: Aufträge
has_children: false
grand_parent: Verkauf, Einkauf und Lager
parent: Verkauf
nav_order: 30
---
# Aufträge

Ein Auftrag gilt im CRM als eine Bestellung eines Kunden. Dieses kann ein angenommenes Angebot sein oder eine Bestellung ohne Angebot. Wenn im CRM bereits ein Angebot für den Kunden erstellt wurde, kann ein Auftrag aus dem Angebot per Button „Auftrag erstellen" erzeugt werden. Im Auftrag können die kopierten Angebots Eigenschaften und Positionen beliebig verändert werden. Der Auftrag ist die Basis der weiteren Belege wie Lieferschein, Rechnung und Gutschrift. **Einen Lieferschein, eine Rechnung oder eine Gutschrift kann man ohne Auftrag nicht erstellen!**  
Alle Aktivitäten, wie E-Mails, Besuchsberichte, Aufgaben, Termine, Dokumente, Lieferschein und Rechnungen werden darin abgelegt.

**Auftrag Typen:**

- **Kauf:** Es werden ausschließlich Artikel vom Eigenlager verwendet. Beim "Lieferschein abschließen" wird die jeweilige Lagerbewegung durchgeführt.
- **Strecke:** Artikel werden vom Lieferant direkt zum Kunden geliefert. Diese laufen nicht über das Eigenlager. Beim "Lieferschein abschließen" wird keine Lagerbewegung durchgeführt.
- **Miete:** Artikel, die mit der aktiven Artikel Option „Mietbar" gekennzeichnet sind, müssen immer als „Mietbar" aktiviert sein.
- **Laufzeitvertrag:** Es können auch zyklische Laufzeitverträge abgebildet werden. Die jeweiligen Anforderungen sind bei den Kunden so unterschiedlich, dass wir diesen Auftragstyp nur über das Customizing freischalten.

**Auftrag Status:**

- **In Bearbeitung**: Der Auftrag ist noch in Bearbeitung. Es wird die Bestellung des Kunden in den Auftrag übernommen.
- **Kommissionierung:** Der Auftrag steht für die Lager Abteilung zur Auslieferung bereit. Jetzt kann ein Lieferschein oder mehrere Teillieferscheine erstellt werden.
- **Verrechnung:** Für die Fakturierung kann nun für den Auftrag benutzt werden und dadurch ist es möglich eine Rechnung oder mehrere Teilrechnungen zu erzeugen.
- **Abgeschlossen:** Es wurde der Auftrag abgeschlossen. Beim Wechsel auf diesen Status wird geprüft, ob auch alle Positionen abgerechnet wurden.

**Button** *"Kommissionierung"*: Bei der Aktion *"Kommissionierung"* wird der Status des Auftrages auf **Kommissionierung** gewechselt. Siehe Auftrags Status **Kommissionierung**.

**Belegs Überleitung mit Button** *"Lieferschein erzeugen"* oder über das **Menü** *"Aktivität neu > Verkauf > Lieferschein oder Retourschein"* überleiten in einen **Verkaufs Lieferschein oder Retourschein**: [Siehe Lieferscheine und Retourscheine](./Lieferscheine%20und%20Retourscheine.md).

Bei der Übernahme der Auftrags Positionen in einem Lieferschein oder Retourschein wird ein Dialog mit folgenden Optionen geöffnet:

- **Positionszeilen übernehmen:** Kann aktiviert werden, damit die Positionen aus dem Auftrag in den Lieferschein oder Retourschein übernommen werden. Wird diese Option nicht aktiviert, können die Positionen manuell im Lieferschein oder Retourschein eingefügt werden.
- **nur Zeilen mit lagergeführten Artikel übernehmen:** Es werden nur Positionen übernommen, die auch im Lager geführt werden, unabhängig davon, ob diese auch tatsächlich derzeit im Lager verfügbar sind.
- **nur noch nicht gelieferte Zeilen übernehmen:** Existieren mehrere Lieferscheine, werden nur die Mengen übernommen, die noch nicht ausgeliefert wurden (Restmenge der Auftragspositionen zu den bereits gelieferten Lieferscheinpositionen).
- **nur noch nicht zurückgelieferte Zeilen übernehmen:** Existieren mehrere Retourlieferscheine, werden nur die Mengen übernommen, die noch nicht zurückgeliefert wurden (Restmenge der Auftragspositionen zu den bereits zurückgelieferten Retourlieferscheinpositionen).

**Belegs Überleitung mit Button** *"Rechnung erzeugen"* oder über das **Menü** *"Aktivität neu > Verkauf > Rechnung"* überleiten in eine Verkaufs Rechnung: [Siehe Rechnungen und Gutschriften](./Rechnungen%20und%20Gutschriften.md).

Es wird eine Dialog mit folgenden Optionen geöffnet:

- **auf Basis Lieferschein:** Gibt es zu einem Auftrag einen oder mehrere Lieferschein, wird die Rechnung immer auf Basis des Lieferscheins erstellt. Man kann zu den jeweiligen Lieferscheinen auch Teilrechnungen erstellen. Ob man in eine Rechnung mehrere Lieferscheine übernimmt oder pro Lieferschein eine Rechnung erstellt, hängt von der Vereinbarung mit dem jeweiligen Kunden ab. Bei der Übernahme der Lieferschein Positionen in eine Rechnung wird immer die tatsächliche Menge übernommen.
- **auf Basis Auftrag:** Gibt es zu einem Auftrag keinen Lieferschein wird die Rechnung immer auf Basis des Auftrags erstellt. Auch hier kann man den Auftrag auf mehrere Teilrechnungen splitten. Bei der Übernahme der Auftrags Positionen in eine Rechnung wird immer geprüft, ob es eine Rechnung mehrere Teilrechnungen gibt. Existieren mehrere Teilrechnungen wird nur die Differenzmenge übernommen.

**Belegs Überleitung in Einkauf:**

Ein **Auftrag** kann man direkt über das **Menü** *"Aktivität neu > Einkauf > Anfrage oder Bestellung"* überleiten in eine **Einkaufs Anfrage oder Bestellung**, um einen weiterführenden Einkaufsprozess einzuleiten. [Siehe Einkauf](../Einkauf/index.md).

**Lieferstatus in der Auftragsliste für lagergeführte Artikel:**

- **leer:** Es ist ein Auftrag ohne lagergeführte Artikel.
- **noch nichts geliefert:** Es ist ein Auftrag mit lagergeführte Artikel. Es wurde noch kein Lieferschein erstellt.
- **teilweise geliefert:** Lieferung erfolgt in Teilschritten bis die gesamte Menge des Auftrages abgearbeitet ist. Teillieferscheine wurden bereits erstellt.
- **alles geliefert:** Die Lieferung ist vollständig abgearbeitet. Die gesamte Auftragsmenge ist in einem oder mehreren Lieferscheinen vorhanden.
