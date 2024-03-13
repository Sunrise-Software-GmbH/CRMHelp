---
title: Rechnungen und Gutschriften
has_children: false
grand_parent: Verkauf, Einkauf und Lager
parent: Verkauf
nav_order: 50
---

# Rechnungen und Gutschriften
{:toc}

Eine Rechnung ist ein Dokument für meine Kunden, in der die ausgelieferte Ware oder auch Dienstleistung enthalten ist. Eine Gutschrift ist das Storno einer gesamten Rechnung oder nur ein Teil der Positionsmenge in einer Rechnung.

Es kann eine Gutschrift aus einer Rechnung erzeugt werden oder aus einem Auftrag. Alle Aktivitäten, wie E-Mails, Besuchsberichte, Aufgaben, Termine und Dokumente werden darin abgelegt.

**Typen:** Nach diesen Typen kann gefiltert werden.
- **Rechnung**
- **Gutschrift**

**Rechnung/Gutschrift Status:**
- **In Bearbeitung:** Der Beleg ist noch in Bearbeitung.
- **Versendet:** Der Beleg wurde per Brief oder E-Mail versendet.
- **Abgeschlossen:** Es wurde der Beleg abgeschlossen und der Betrag über "Bezahlt am" ausgebucht.

**Beleg Aktionen:** Es wurde bei der Rechnungsfirma (Debitor) als Rechnungsversand in den Firmenstammdaten eingestellt.
- **Versenden - Brief**
- **Versenden - E-Mail**

**Über das Kontext [Menü](Menü)<!-- TODO --> der Rechnungsliste erreichbare Funktion:**
- **Rechnung abschließen:** Die ausgewählten Rechnungen, deren Status *"versendet"* ist, werden nach der Eingabe eines Datums abgeschlossen. Dabei wird der Rechnungsbetrag als bezahlter Betrag, das *"bezahlt am"* Datum durch das eingegebene Datum und der Status auf *"abgeschlossen"* gesetzt.  
Rechnungen, für die keine Schreibberechtigung existiert,werden nicht geändert.

**Gutschrift erstellen:**  

Es kann eine Gutschrift aus einer **Rechnung** über das **Menü** *"Aktivität > Verkauf> Gutschrift"* erstellt werden. Es werden alle Positionen der Rechnung in die Gutschrift übernommen.

Es kann eine Gutschrift aus einem **Auftrag**, über das **Menü** *"Aktivität > Verkauf > Gutschrift"* erstellt werden, wenn es einen **Retourschein** gibt.


## Elektronischer Rechnungsexport (E-Rechnung für Italien)
{:toc}

Mit 01.01.2019 wurde vom italienischen Finanzamt ein elektronischer Rechnungsablauf definiert. Über das Rechnungsformular im CRM kann aus einer Rechnung eine XML Datei erzeugt werden, die für einen Import im Finanzamt verwendet werden kann. Dazu steht der Button *"Versenden - XML"* zur Verfügung.

Dazu sind folgende Eingaben notwendig:
- **Buchhaltungseinheit:**  
eInvoicing aktiv (ActiveEInvoicing): aktiviert  
eInvoicing URL (UrlEInvoicing): hier wird ein Pfad für die Ablage der zu erzeugenden XML Datei hinterlegt
- **Firma:**  
Mail-Rechnungsversand (LinkMailInvoice): Eintragung einer gültigen E-Mail Adresse  
eInvoicing Empfängercode (RecipientCodeEInvoicing): neben den Standard Feldern wie FN-Nr, UID und Steuernummer ist auch der Empfängercode zu hinterlegen.

## Schnittstellen Finanzbuchhaltung (Export FIBU) (RZL, BMD, DATEV,...)
{:toc}

Für die Module Rechnungen, Gutschriften und Kunden (Debitoren) gibt es die Möglichkeit für einen FIBU Export für verschiedene Buchhaltungssysteme wie RZL, BMD oder DATEV.

**Hier kann eingestellt werden, welche Daten für die Finanzbuchhaltung exportiert werden sollen:**
- **Buchhaltungseinheit:** ermöglicht die Auswahl der Buchhaltungseinheit, deren Rechnungen exportiert werden sollen. Auch die Option "Ausgewählte" bezieht sich auf die hier eingestellte Buchhaltungseinheit.
- **Verzeichnis:** Angabe eines Ordners, in dem die Dateien abgelegt werden.
- **Senden als E-Mail:** Die erzeugten Dateien werden in einem E-Mail als Anhang abgelegt.
- **Datei Kennung:** Hier sollte eine Datei-Kennung eingegeben werden, um den exportierten Dateien einen Namen zu geben (Beispiel: die Datei-Kennung *"2017-01"* erzeugt die Dateien *"2017-01-Account.csv"* und *"2017-01-Invoice.csv"*).
- **Debitorenliste:** Wenn diese Option aktiviert ist, dann werden auch die Debitoren der Buchhaltungseinheit exportiert. Diese werden in einer Datei mit der Dateikennung und der Ergänzung "-Account" abgelegt (Beispiel: *2017-01-Account.csv*).
- **Ausgangsrechnungen:** Wenn diese Option aktiviert ist, dann werden die Rechnungen der Buchhaltungseinheit exportiert. Diese werden in einer Datei mit der Dateikennung und der Ergänzung "-Invoice" abgelegt (Beispiel: *2017-01-Invoice.csv*).

**Für den Rechnungsexport stehen noch folgende Optionen zur Verfügung:**
- **PDF Datei pro Beleg erzeugen:** Erzeugt für jede exportierte Rechnung auch eine PDF Datei im Unterverzeichnis mit der Jahreszahl der darin enthaltenen Rechnungen. Ist *"Senden als E-Mail"* aktiviert, werden diese Rechnungs-PDF Dateien in einer ZIP Datei mit der Dateikennung Invoices.zip zusammengepackt (Beispiel: *2017-01-Invoices.zip*)
- **Nicht gebuchte:** Unabhängig der aktuellen Rechnungsliste werden alle noch nicht gebuchten Rechnungen exportiert.
- **Ausgewählte:** Exportiert die in der aktuellen Rechnungsliste ausgewählten Rechnungen unter Berücksichtigung der gewünschten Buchhaltungseinheit.

**Neben den Standard-Funktionen der Belege bietet das Rechnungsmodul noch zusätzliche Funktionen an:**
- **Export FIBU:** Ist für den angemeldeten Benutzer über die Administration das Recht für diesen Export hinterlegt, dann enthält das [Menü](Menü)<!-- TODO --> *"Senden an - Export"* einen zusätzlichen Menüpunkt *"Export FIBU"*. Diese Funktion bietet einen Dialog für die Auswahl der zu exportierenden Daten an und erzeugt anschließend die für das Finanz-Buchhaltungs-Programm erforderlichen Daten.

## Registrierkassensicherheitsverordnung (RKSV für Österreich)
{:toc}

Die Anwendung der in Österreich 2017 eingeführten RKSV wird in nachfolgendem Link beschrieben: [RKSV Betrieb](https://www.relations-crm.com/documents/Downloads/rksv/Dokumentation%20RKSV%20-%20Betrieb.pdf)
