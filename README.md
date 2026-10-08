# Patientenchecker Werneck

Einzeldatei-Anwendung, veröffentlicht über GitHub Pages:
**https://jobraetz99.github.io/Patientenchecker-werneck/**

| Datei | wofür |
|---|---|
| `index.html` | das Dashboard selbst |
| `blank.html` | Landeseite des Anmelde-Popups — **muss mit hoch**, sonst bricht das Abrufen der Teamliste |
| `.nojekyll` | schaltet die Jekyll-Verarbeitung ab, die sonst die Seite umbaut |

## Arbeitskopie

Bearbeitet wird **nicht hier**, sondern in OneDrive unter
`BM Group/12_Code/Patientenchecker/werneck.html`. Von dort wird kopiert und
hochgeladen — ein `.git`-Ordner in einem synchronisierten OneDrive-Ordner geht
früher oder später kaputt.

## Anmeldung

Die Seite lädt ihre Daten mit dem Microsoft-Konto des Besuchers aus SharePoint.
Damit die Anmeldung funktioniert, müssen **beide** URLs in der
App-Registrierung `9fe9cda7-79c3-4d06-82dc-372715bb8086` unter
*Authentifizierung → Single-Page-Anwendung* stehen:

```
https://jobraetz99.github.io/Patientenchecker-werneck/
https://jobraetz99.github.io/Patientenchecker-werneck/blank.html
```

Fehlt eine davon, meldet Microsoft `AADSTS50011`.

## Was öffentlich ist

Das Repository ist öffentlich, also auch der Quelltext: Preise, Bewertungslogik,
SharePoint-Pfade. **Patientendaten sind nicht darin** — die kommen erst nach der
Anmeldung aus SharePoint und nur für Konten mit Rechten auf der Site.
