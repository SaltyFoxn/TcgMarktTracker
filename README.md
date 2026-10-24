# CardVault – TCG Market Tracker v0.1

Eine kostenlose, deutschsprachige, dunkle iPhone-taugliche PWA für eine lokale TCG-Sammlung.

## Enthalten

- Pokémon-, One-Piece- und Dragon-Ball-Demo-Karten
- Suche, Filter und Sortierung
- Kaufpreis, letzter Verkauf und aktueller Angebotspreis
- theoretischer Gewinn/Verlust gegenüber dem letzten Verkauf
- manuelle Preisbeobachtungen mit Quelle, Datum und Notiz
- lokale Speicherung im Browser
- JSON-Backup exportieren und importieren
- offlinefähige PWA-Grundstruktur mit Service Worker

## Wichtig

Alle eingebauten Demo-Karten und Preise sind frei erfunden. Es gibt keine Live-Preise und keine API-Anbindung. Manuell erfasste Werte werden nicht automatisch verifiziert. Die P/L-Rechnung ist vereinfacht und berücksichtigt noch keine Gebühren, Versandkosten oder Steuern.

## Kostenlos auf dem iPhone testen (GitHub Pages)

Du benötigst ein kostenloses GitHub-Konto und Safari auf dem iPhone. GitHub Pages stellt statische Dateien per HTTPS bereit und ist für diese kleine Demo ausreichend, vorbehaltlich der aktuellen Nutzungsbedingungen.

1. Öffne auf einem Computer `https://github.com` und erstelle ein kostenloses Konto, falls du noch keines hast.
2. Erstelle ein neues Repository, z. B. `tcg-market-tracker`. Für einen einfachen Einstieg kann es öffentlich sein; veröffentliche dort keine privaten Daten.
3. Lade `index.html`, `manifest.webmanifest`, `sw.js` und `icon.svg` in das oberste Verzeichnis des Repositorys hoch. `README.md` kannst du ebenfalls hochladen.
4. Öffne im Repository **Settings → Pages**.
5. Unter **Build and deployment** wählst du **Deploy from a branch**, anschließend den Branch `main` und den Ordner `/(root)`. Speichern.
6. Warte, bis GitHub Pages die Website veröffentlicht hat. Öffne die dort angezeigte URL.
7. Öffne dieselbe URL in Safari auf deinem iPhone. Tippe auf **Teilen → Zum Home-Bildschirm** (die Bezeichnung kann je nach iOS-Version leicht variieren) und bestätige.
8. Starte CardVault über das neue Home-Bildschirm-Symbol. Teste Suche, Karten hinzufügen, Preisbeobachtungen und Backup-Export.

### Ohne Computer?

Das Hochladen mehrerer Dateien lässt sich teilweise über die GitHub-Website im mobilen Browser versuchen, ist auf dem iPhone aber umständlicher. Wenn möglich, ist ein Computer für die Ersteinrichtung deutlich einfacher. Alternativ kannst du die `index.html` zunächst direkt in einem Browser öffnen, um die Oberfläche zu prüfen; PWA-Installation und Offline-Funktion brauchen normalerweise einen HTTPS-Host oder localhost.

## Daten speichern und sichern

- Die Sammlung wird mit `localStorage` auf dem jeweiligen Browser und der jeweiligen Website gespeichert.
- Browserdaten löschen, Website-Daten entfernen oder ein anderer Browser können dazu führen, dass die Sammlung nicht mehr verfügbar ist.
- Nutze regelmäßig **Backup & Daten → Backup exportieren (.json)**.
- Ein Backup enthält Karten und Preisbeobachtungen. Bewahre es an einem sicheren Ort auf.
- Import ersetzt die aktuell gespeicherten Daten.

## Grenzen von Version 0.1

- Kein automatischer Zugriff auf eBay oder Cardmarket
- Keine Anmeldung oder Cloud-Synchronisierung
- Keine verifizierten Live-Preise
- Kein automatisches Kartenbild- oder Kartendaten-Matching
- Kein steuerlicher oder gebührenbereinigter Gewinnrechner

## Nächste sinnvolle Schritte

1. Testen und Fehler beheben.
2. Kartendaten/Set-IDs strukturieren.
3. Gebühren und Versand als eigene Felder ergänzen.
4. Rechtmäßige und verfügbare Datenquellen für eBay-Verkäufe und Cardmarket-Angebote prüfen, bevor irgendeine automatische Integration geplant wird.
