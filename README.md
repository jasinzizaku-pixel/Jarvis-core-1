# JARVIS CORE 1.0 — kostenloser Hybrid-PWA-Prototyp

## Was ist enthalten?
- Responsive Web-App für Desktop und Smartphone
- Installierbare PWA-Grundlage (Manifest + Service Worker)
- Lokale Speicherung im Browser (`localStorage`)
- Dashboard, Chat-Demo, Agentenübersicht
- Aufgaben und Projekte mit CRUD-Funktionen
- Research-Briefs
- Finance-Watchlist und Paper-Trading-Ideen (nur illustrative Daten)
- Reservierungsanfrage-Entwurf mit lokalem Freigabeprozess
- Freigabezentrum, Integrationsübersicht und Einstellungen
- JSON-Datenexport und Workspace-Reset

## Starten
1. ZIP entpacken.
2. Dateien über einen lokalen Webserver bereitstellen. Beispiel mit Python:
   `python -m http.server 8000`
3. Im Browser `http://localhost:8000` öffnen.

Alternativ die Dateien auf einen statischen HTTPS-Host legen. Für die PWA-Installation und Offline-Funktion ist HTTPS erforderlich (localhost ist für lokale Entwicklung ausgenommen).

## Wichtige Grenzen
- Dies ist ein Frontend-Prototyp, keine echte autonome KI.
- Chat-Antworten sind lokal und regelbasiert; kein KI-Modell wird aufgerufen.
- Daten bleiben im jeweiligen Browserprofil. Es gibt keine Cloud-Synchronisierung, Anmeldung oder Mehrgeräte-Datenbank.
- Es gibt keine Websuche, echten Restaurantbuchungen, E-Mails, Kalenderaktionen, Brokerverbindung oder Livekurse.
- Finance ist ausschließlich Simulation. Keine echten Orders oder Anlageberatung.
- Freigaben protokollieren nur die lokale Entscheidung; sie führen keine externe Aktion aus.
- Voice/Wake Word ist als späteres Modul vorgesehen, aber noch nicht aktiviert.
- Keine API-Schlüssel in Frontend-Code eintragen.

## Nächste technische Ausbaustufen
1. Versionskontrolle und automatisierte Tests
2. Sichere Authentifizierung und Cloud-Backend für geräteübergreifende Synchronisierung
3. Serverseitige KI-Provider-Anbindung mit Secret-Management und Kostenlimits
4. Websuche und kontrollierte Tool-Aufrufe
5. Freigabe-Gateway mit unveränderlichem Audit-Log
6. Kalender-/Reservierungsanbieter und E-Mail mit OAuth
7. Voice: Speech-to-text, Dialogsteuerung, Text-to-speech
8. Paper-Trading-Datenquelle; Echtgeld-Broker erst nach separater Sicherheits- und Rechtsprüfung

## Datenschutz
Alle Eingaben in dieser Demo werden im Browser gespeichert. Auf gemeinsam genutzten Geräten keine sensiblen Daten eingeben. Nutze den JSON-Export für eine Sicherung und den Reset, um lokale Daten zu löschen.
