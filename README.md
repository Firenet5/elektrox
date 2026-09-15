# ElektroX – Elektro Hauska – V6

iPhone-taugliche Angebots- und Rechnungs-App als statische Web-App/PWA-Grundlage.

## Neu in V6: DATANORM
- Import-Assistent für DATANORM-Artikeldateien über **Artikel → DATANORM**.
- Erkennung von DATANORM-A-Artikelsätzen und Vorschau der Felder.
- Vor dem Import können Artikelnummer, Bezeichnung, Einkaufspreis und Mengeneinheit zugeordnet werden.
- Einkaufspreis (EK) und Verkaufspreis (VK) werden getrennt gespeichert.
- Standard-Kalkulation im Artikelstamm: 23 % Aufschlag, frei änderbar.
- Bereits vorhandene Artikel mit gleicher Artikelnummer werden beim Import aktualisiert.
- Importierte Artikel werden als Quelle DATANORM gekennzeichnet.
- Artikel können weiterhin manuell bearbeitet werden.

### Wichtig
DATANORM 4 und 5 sind standardisierte, semikolonbasierte Austauschformate. Die tatsächlichen Felder können je nach Datenlieferant unterschiedlich befüllt sein. Deshalb zeigt ElektroX vor dem Import eine Feldvorschau und lässt die Zuordnung prüfen.

Der nächste Ausbau kann ergänzen:
- DATPREIS-Preisänderungsdateien
- Rabattgruppen und Lieferanten
- Hersteller-/Typnummern
- Warengruppen
- Rohstoff-/Zuschläge
- automatische Lieferanten- und Preishistorie
- automatische VK-Neukalkulation nach Preisänderungen

## Dropbox
Die App verwendet OAuth 2.0 mit PKCE. Es wird kein Dropbox App Secret in der Browser-App verwendet.

Zielordner:
`/ElektroX – Elektro Hauska`

## Start
Die `index.html` kann nach dem Hosting über eine HTTPS-Adresse geöffnet werden. Für die Dropbox-OAuth-Weiterleitung muss diese exakte Adresse in der Dropbox App Console als Redirect URI hinterlegt werden.
