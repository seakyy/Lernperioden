# Lern-Periode 10

25.4 bis 27.6

## Grob-Planung

1. Welche Programmiersprache möchten Sie verwenden? Was denken Sie, wo Ihre Zeit und Übung am sinnvollsten ist?

   Ich setze auf C# für das Backend (ASP .NET Core) und JavaScript (React) für das Frontend, da ich so sowohl serverseitige Logik als auch moderne Web-Interfaces üben kann.

   
2. Welche Datenbank-Technologie möchten Sie üben? Fühlen Sie sich sicher mit SQL und möchten etwas Neues ausprobieren; oder möchten Sie sich weiter mit SQL beschäftigen?

   Ich verwende SQLite mit Entity Framework Core, um meine SQL-Kenntnisse zu vertiefen und dennoch eine leichtgewichtige Lösung zu haben, die später auf dem Raspberry Pi 5 erweitert werden kann.

   
3. Was wäre ein geeignetes Abschluss-Projekt?

   Eine interaktive Event-Feedback-App, bei der Veranstalter Sitzungen und Fragen anlegen und Teilnehmer in Echtzeit Feedback geben können.

## 25.4

Welche 3 *features* sind die wichtigsten Ihres Projektes? Wie können Sie die Machbarkeit dieser in jeweils 45' am einfachsten beweisen?

| Make-or-Break Feature                  | Beschreibung                                                                                     | Proof of Concept                                               |
|----------------------------------------|-------------------------------------------------------------------------------------------------|-----------------------------------------------------------------|
| **Dynamische Fragen-Engine**           | Anlegen und Verwalten verschiedener Fragetypen (Multiple-Choice, Rating, Freitext) im Admin-UI. | Einfaches CRUD-Formular in Razor Pages implementieren.          |
| **Mobile UX & Session-Onboarding**     | Teilnehmer-Login per QR-Code oder Session-ID und Darstellung der Fragen auf dem Smartphone.      | Statische HTML-Seite mit QR-Code-Eingabe und Dummy-Fragen bauen.|
| **Echtzeit-Dashboard & Daten-Pipeline** | Live-Aktualisierung von Antworten in Balken- und Tortendiagrammen im Admin-Dashboard.           | Chart.js mit statischen Daten und einfachem Polling integrieren.|



✍️ Heute habe ich... (50-100 Wörter)

Heute habe ich das Projekt in Visual Studio angelegt, die Models für Sitzungen, Fragen, Optionen und Antworten erstellt und die drei wichtigsten Features aufgeschrieben. Ich habe auch die Datenbank eingerichtet. Als nächstes starte ich mit der ersten Razor-Page.

☝️ Vergessen Sie nicht, den Code von heute auf github hochzuladen. Ggf. bietet es sich an, für die Code-Schnipsel einen eigenen Ordner `exploration` zu erstellen.

## 2.5

Ausgehend von Ihren Erfahrungen vom 25.4, welche *features* brauchen noch mehr Recherche? (Sie können auch mehrere AP für ein *feature* aufwenden.)

- [ ] Papier & Stift: Mobil-Layout & User-Flow skizzieren (📵) 
- [ ] QR-Code: JS-Bibliothek zum Scannen & Generieren testen 
- [ ] Echtzeit: Polling vs. SignalR vergleichen  
- [ ] Charts: Dynamische Chart.js-Visualisierung prüfen 

✍️ Heute habe ich... (50-100 Wörter)

Heute habe ich die Mehrheit der zeit in Debuggen investiert. Ich hatte grosse Probleme beim Umsetzen des Echtzeit: Polling vs. SignalR vergleichen Arbeistpacket. Zuerst wurde die .db Datei garnicht anerkannt. Danach wurde sie zwar erkannt, aber der Code machte kein POST-Statement, dementsprechend wurde auch nicht gespeichert. Nachdem ich den Code nochmals aktualisisert habe, hat es endlich geklappt und die Daten werden in Echtzeit angezeigt und in einem Diagramm dargestellt. Da ich heute sehr unproduktiv war - das Debuggen war sehr zeitintensiv - verschiebe ich das Arbeitspacket mit den Charts auf nächstes mal.

☝️ Vergessen Sie nicht, den Code von heute auf github hochzuladen.

## 9.5

Planen Sie nun Ihr Projekt, sodass die *Kern-Funktionalität* in 3 Sitzungen realisiert ist. Schreiben Sie dazu zunächst 3 solche übergeordneten Kern-Funktionalitäten auf: 

1. Kern-Funktionalität: Admin-Oberfläche zum Anlegen von Sessions und Fragen
2. Kern-Funktionalität: Teilnehmer-Flow mit Antwort-Erfassung
3. Kern-Funktionalität: Live-Dashboard mit Ergebnis-Visualisierung 

Diese Kern-Funktionalitäten brechen Sie nun in etwa 4 AP je herunter. Versuchen Sie jetzt bereits, auch die Sitzung vom 16.5 und 23.5 zu planen (im Wissen, dass Sie kleine Anpassungen an Ihrer Planung vornehmen können).

- [ ] Sessions- und Fragen-CRUD im Admin-UI umsetzen
- [ ] JoinSession- und Questions-Page mit Antwortspeicherung implementieren 
- [ ] API-Endpunkt für Ergebnis-Aggregation erstellen
- [ ] Charts: Dynamische Chart.js-Visualisierung prüfen 

✍️ Heute habe ich... (50-100 Wörter)
Ich hatte am Anfang noch hartcodierte See-Daten und auch falsche bindungen, die zu ModelState-Fehler führten. Mit einem neuen, simplen ViewModel im Ordner Admin/ und mit dem korrekten einbinden der SeesionId speichert es jetzt endlich Fragen und Optionen in feedback.db und werden nach dem Speichern direkt zum Feedback Flow weitergeleitet. Ich habe heute, wie beim letzten Mal, sehr lange meine Zeit im Debugger verbracht, um die kleinen aber hartnäckigen Bindin Fehler zu beseiten (mit erfolg).

☝️  Vergessen Sie nicht, den Code von heute auf github hochzuladen.

## 16.5

- [ ] Admin/ResultsSignalR/1 aktualisieren
- [ ] Question-CRUD vervollständigen
- [ ] JoinSession-Flow & QR-Integration
- [ ] Live-Dashboard mit Chart.js integrieren

✍️ Heute habe ich... (50-100 Wörter)

☝️  Vergessen Sie nicht, den Code von heute auf github hochzuladen.

## 23.5

- [ ] ...
- [ ] ...
- [ ] ...
- [ ] ...

✍️ Heute habe ich... (50-100 Wörter)

☝️  Vergessen Sie nicht, den Code von heute auf github hochzuladen.

## 6.6

Ihr Projekt sollte nun alle Funktionalität haben, dass man es benutzen kann. Allerdings gibt es sicher noch Teile, welche "schöner" werden können: Layout, Code, Architektur... beschreiben Sie kurz den Stand Ihres Projekts, und leiten Sie daraus 6 solche "kosmetischen" AP für den 6.6 und den 13.6 ab.

- [ ] ...
- [ ] ...
- [ ] ...
- [ ] ...

✍️ Heute habe ich... (50-100 Wörter)

☝️  Vergessen Sie nicht, den Code von heute auf github hochzuladen.

## 13.6

- [ ] ...
- [ ] ...

✍️ Heute habe ich... (50-100 Wörter)

☝️  Vergessen Sie nicht, den Code von heute auf github hochzuladen.

## 20.6

Was fehlt Ihrem fertigen Projekt noch, um es auszuliefern? Reicht die Zeit für ein *nice-to-have feature*?

- [ ] ...

Bereiten Sie in den verbleibenden 2 AP Ihre Präsentation vor

- [ ] Materialien der Präsentation vorbereiten
- [ ] Präsentation üben

✍️ Heute habe ich... (50-100 Wörter)

☝️  Vergessen Sie nicht, die Unterlagen für Ihre Präsentation auf github hochzuladen.

## 27.6
