# BSEasy Sync

WordPress Plugin zur Synchronisation von Mitglieder- und Kontaktdaten aus EasyVerein (API v2.0) mit WordPress.

## Beschreibung

BSEasy Sync synchronisiert Mitglieder- und Kontaktdaten aus EasyVerein über die Consent-API v2.0 mit WordPress. Das Plugin bietet eine umfassende Admin-Oberfläche zur Verwaltung der Synchronisation und zeigt die Daten im Frontend als interaktive Mitgliederlisten, Karten und Kalender an.

## Hauptfunktionen

- **API-Synchronisation**: Automatische Synchronisation mit EasyVerein Consent-API v2.0
- **Admin-Interface**: Umfassende Verwaltungsoberfläche für Sync-Einstellungen, Felderkonfiguration und Datenverwaltung
- **Frontend-Darstellung**: 
  - Interaktive Mitgliederlisten mit Filterfunktionen
  - Interaktive Kartenansicht (Leaflet.js) mit Clustering
  - Kalenderansicht für Veranstaltungen
- **Caching**: Intelligentes Caching-System für optimale Performance
- **Sicherheit**: Umfassende Sicherheitsmaßnahmen (Nonces, Rate-Limiting, Input-Validierung, SQL-Injection-Schutz)

## Anforderungen

- WordPress: 5.8 oder höher
- PHP: 7.4 oder höher
- EasyVerein API v2.0 Zugriff

## Installation

1. Plugin-Verzeichnis in `/wp-content/plugins/` hochladen
2. Plugin im WordPress Admin aktivieren
3. Unter "BSEasy Sync" die API-Zugangsdaten konfigurieren
4. Erste Synchronisation durchführen

## Verwendung

### Shortcodes

**Mitgliederliste:**
```
[bes_members]
```

**Kartenansicht:**
```
[bes_map]
```

**Kalender:**
```
[bes_calendar]
```

### Admin-Bereich

Nach der Aktivierung findest du das Plugin im WordPress Admin-Menü unter "BSEasy Sync" mit folgenden Bereichen:

- **Sync**: Synchronisation starten und verwalten
- **Felder**: Custom-Field-Konfiguration und Verwaltung
- **Karte**: Karten-Einstellungen
- **Kalender**: Kalender-Konfiguration

## Technische Details

- **Version**: 3.0.0
- **Text Domain**: besync
- **Lizenz**: GPL v2 or later
- **Entwickelt nach**: WordPress Coding Standards (WPCS)

## Sicherheit

Das Plugin implementiert umfassende Sicherheitsmaßnahmen:

- AES-256-CBC Verschlüsselung für API-Tokens
- Nonce-Validierung für alle AJAX-Requests
- SQL-Injection-Schutz durch `$wpdb->prepare()`
- XSS-Schutz durch Output-Escaping
- Rate-Limiting für API-Endpunkte
- Input-Validierung und Sanitization

## Support & Links

- **GitHub**: [https://github.com/eversthomas/bseasy-sync](https://github.com/eversthomas/bseasy-sync)
- **Website**: [https://bezugssysteme.de](https://bezugssysteme.de)
- **Autor**: Tom Evers

## Lizenz

Dieses Plugin ist lizenziert unter der GPL v2 or later.

Copyright (c) Tom Evers

Dieses Programm ist freie Software. Sie können es unter den Bedingungen der GNU General Public License, wie von der Free Software Foundation veröffentlicht, weitergeben und/oder modifizieren, entweder gemäß Version 2 der Lizenz oder (nach Ihrer Option) jeder späteren Version.

Dieses Programm wird in der Hoffnung verteilt, dass es nützlich sein wird, aber OHNE JEDE GEWÄHRLEISTUNG; sogar ohne die implizite Gewährleistung der MARKTFÄHIGKEIT oder der EIGNUNG FÜR EINEN BESTIMMTEN ZWECK. Siehe die GNU General Public License für weitere Details.

