# Bolt Security Prompts - Deutsch

## RLS-Richtlinien (Row Level Security)

### Allgemeine Überprüfung
```
Überprüfe die RLS-Richtlinien in meiner Bolt-App, um sicherzustellen, dass Benutzer nur auf ihre eigenen Daten zugreifen können und geteilte Daten ordnungsgemäß geschützt sind
```

### Benutzer und Beiträge
```
Prüfe die RLS-Richtlinien für Benutzer- und Beitrags-Tabellen - Benutzer sollten nur ihr eigenes Profil sehen, aber alle öffentlichen Beiträge lesen können
```

### Einstellungen
```
Füge RLS-Richtlinien zur Einstellungs-Tabelle hinzu, damit Benutzer nur auf ihre eigenen Einstellungen zugreifen können
```

### Zugriffsrechte korrigieren
```
Behebe zu weitreichende Zugriffsrechte - Benutzer sehen derzeit alle Beiträge von allen Benutzern, beschränke auf eigene Beiträge und nur öffentliche Beiträge
```

### Teams und Projekte
```
Richte RLS für Teams- und Projekt-Tabellen ein, damit Teammitglieder nur Projekte ihres eigenen Teams sehen
```

### Multi-Tenant Apps
```
Stelle sicher, dass Benutzer nur auf Daten ihrer eigenen Organisation in meiner Multi-Tenant-App zugreifen können
```

### Sicherheitsaudit
```
Prüfe RLS-Richtlinien auf Sicherheitslücken, durch die Benutzer auf nicht autorisierte Daten zugreifen könnten
```

### Vereinfachung
```
Vereinfache komplexe RLS-Richtlinien unter Beibehaltung der Sicherheit - aktuelle Richtlinien sind zu kompliziert
```

---

## Edge Functions

### Benutzerregistrierung
```
Erstelle eine Edge Function für die Benutzerregistrierung mit ordnungsgemäßer Validierung und Sicherheitsprüfungen. Benutzer sollten E-Mail, Passwort und optional ein Profilbild bei der Anmeldung angeben
```

### Zahlungsabwicklung
```
Verlagere die Zahlungsabwicklungslogik vom Frontend in eine sichere Edge Function. Ich habe eine Checkout-Komponente, die derzeit Stripe-Zahlungen direkt im Browser verarbeitet
```

### Datei-Uploads
```
Erstelle eine Edge Function für Datei-Uploads mit Typ- und Größenvalidierung. Benutzer können Profilbilder (max. 5MB) und Dokumente (nur PDF, max. 10MB) hochladen
```

### E-Mail-Versand
```
Richte eine Edge Function ein, um Willkommens-E-Mails sicher zu versenden, wenn sich Benutzer anmelden. Verwende die Anbieter-API, um personalisierte Willkommens-E-Mails mit dem Namen und den Kontodaten des Benutzers zu senden
```

### Webhook-Verarbeitung
```
Implementiere eine Edge Function zur Verarbeitung von Webhook-Events von externen Diensten
```

---

## Sicherheit & API-Schlüssel

### Stripe API-Schlüssel
```
Füge einen API-Schlüssel für Stripe-Zahlungen sicher hinzu, ohne ihn im Frontend-Code offenzulegen
```

### Validierung verlagern
```
Verlagere die Validierungslogik von React-Komponenten zu Edge Functions für bessere Sicherheit
```

### Code-Überprüfung
```
Überprüfe den Frontend-Code auf offengelegte Geheimnisse, API-Schlüssel oder sensible Informationen. Ich habe eine Einstellungsseite, die Benutzerpräferenzen anzeigt, und möchte sicherstellen, dass keine sensiblen Daten sichtbar sind
```

### Validierung identifizieren
```
Identifiziere clientseitige Validierung, die zu Backend-Edge-Functions verlagert werden sollte
```