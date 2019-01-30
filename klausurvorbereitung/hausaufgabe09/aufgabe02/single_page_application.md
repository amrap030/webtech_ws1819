# Was ist eine Single Page Application (SPA)?

- Webapplikation oder Website, welche die aktuelle Seite dynamisch mit neuem Inhalt befuellt oder Teile ersetzt, ohne die Seite nachzuladen
- dazu wird jeglicher benoetigter Code beim Oeffnen einer Seite geladen und kann somit verwendet werden um Inhalt zu ersetzen oder hinzuzufuegen
- falls wir doch noch Daten vom Server laden muessen, erhalten wir vom Server keine HTML Seiten mehr sondern strukturierte Daten im JSON Format womit Javascript umgehen kann (passiert im Hintergrund) -> keine Seiten werden geladen, sondern nur Daten

### Vorteile

- sehr reactive/responsive -> gute User Experience
- entkoppeltes Frontend, kein Serverseitiger Code muss geschrieben werden

### Challenges

- Initialer Page Load koennte Lange dauern, da mehr Ressourcen geladen werden muessen
- Analytics sind oft abhaengig vom Laden neuer Seiten im Browser
- es gibt keine wirkliche Browser History mehr, bis auf die Initiale Seite -> Vor und Zurueck nicht mehr moeglich -> verwirrend fuer User
- Viele Suchmaschienen fuehren Javascript Code nicht aus koennen Somit den Inhalt nicht erfassen
- Javascript kann im Browser ausgeschaltet werden
- eher fuer moderne Browser geeignet

### Geeignet fuer

- Webapplikationen

### nicht geeignet fuer

- Wikis (informative Seiten), Foren, News Pages

[SPA](https://www.youtube.com/watch?v=F_BYg2QGsC0)
