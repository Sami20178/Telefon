# Telefon — Node.js Server

Node.js + Express API-Grundlage für die Telefon-App. Benötigt Node.js 20 oder neuer.

## Lokal starten
```bash
npm install
cp .env.example .env
npm start
```
Standard-Port: 3000.

## API-Endpunkte
- `GET /` — Service-Info
- `GET /api/health` — Healthcheck
- `GET /api/chats`, `POST /api/chats` — Demo-Chats
- `POST /api/chats/:id/messages` — Demo-Nachricht
- `GET /api/contacts`, `POST /api/contacts` — Demo-Kontakte
- `GET /api/calls`, `POST /api/calls` — Anrufprotokoll, startet keinen echten Anruf
- `GET /api/ads/placement` — Platzierung für den Werbung-Tab; Live-Anzeigen deaktiviert

## Wichtiger Status
Das ist noch kein produktionsreifer Chat- oder Telefonie-Dienst. Daten liegen vorläufig im Arbeitsspeicher und verschwinden beim Neustart. Authentifizierung, Datenbank, Echtzeit-Zustellung, Push-Mitteilungen, Datei-/Medienversand, Ende-zu-Ende-Verschlüsselung, SMS-Anbieter und echte Mobilfunk-/VoIP-Anrufe fehlen. Keine privaten Nachrichten oder echten Zugangsdaten in dieser Demo verwenden.

Microsoft-Werbung ist ein Platzhalter. Live-Werbung erfordert eine zugelassene Integration sowie passende Datenschutz- und Einwilligungsinformationen. Niemals Schlüssel oder Zugangsdaten ins Repository committen.

Für Produktion HTTPS, persistente Datenbank, Authentifizierung, Zugriffskontrollen, Rate-Limits und Sicherheitsprüfung ergänzen.
