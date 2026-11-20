# ImmoPlan – Immobilienfinanzierungs-Rechner

Eine statische Progressive Web App (PWA) für GitHub Pages. Sie berechnet Monatsrate, Zinskosten und Restschuld für 10, 20 und 30 Jahre. Das Restschuld-Diagramm aktualisiert sich live.

## Projektdateien

- `index.html` – Rechner und Oberfläche
- `manifest.webmanifest` – App-Name, Darstellung und Installations-Icons
- `service-worker.js` – Offline-Cache
- `assets/immoplan-logo.svg` – skalierbares Logo
- `assets/icon-192.png` und `assets/icon-512.png` – App-Icons
- `.github/workflows/deploy.yml` – automatisches GitHub-Pages-Deployment

## Veröffentlichung über GitHub Pages

1. Auf GitHub ein neues Repository erstellen, z. B. `immoplan`.
2. Den gesamten Inhalt dieses ZIP-Archivs in das Stammverzeichnis des Repositorys hochladen. `index.html` muss direkt im Stammverzeichnis liegen.
3. Im Repository **Settings → Pages** öffnen.
4. Unter **Build and deployment** als Source **GitHub Actions** auswählen.
5. Die Dateien auf den Branch `main` pushen. Der Workflow veröffentlicht die Website automatisch.
6. Die veröffentlichte Adresse findest du unter **Settings → Pages**. Sie sieht meist so aus: `https://DEIN-NUTZERNAME.github.io/immoplan/`.

GitHub Pages stellt HTTPS bereit. HTTPS ist für die PWA-Installation und den Offline-Modus erforderlich.

## Als Desktop-App installieren

1. Die veröffentlichte Website in Chrome oder Edge öffnen.
2. In der Adressleiste das Installationssymbol auswählen oder im Browsermenü **App installieren** anklicken.
3. ImmoPlan lässt sich danach wie eine eigenständige App über Startmenü, Dock oder Desktop öffnen.

## Auf iPhone oder iPad

1. Die Website in Safari öffnen.
2. Auf **Teilen** tippen.
3. **Zum Home-Bildschirm** auswählen.
4. Mit **Hinzufügen** bestätigen.

## Lokal testen

PWA-Installation und Service Worker funktionieren nicht beim direkten Öffnen über `file://`. Für einen lokalen Test die Dateien über einen lokalen Webserver bereitstellen oder GitHub Pages verwenden.

## Berechnungshinweis

Die Anwendung ist eine vereinfachte Modellrechnung. Sie berücksichtigt keine Kaufnebenkosten, Gebühren, Sondertilgungen, Tilgungssatzwechsel oder Anschlussfinanzierungs-Konditionen. Die angezeigten Zinsen beziehen sich auf den jeweiligen Simulationszeitraum.
