# Git-Anleitung für Anfänger

## Was ist Git?

Git ist wie eine **Zeitmaschine für deine Projekte**. Es verfolgt jede Änderung, die du an deinem Code machst, damit du:

- Sehen kannst, was du geändert hast und wann
- Zu früheren Versionen zurückkehren kannst, wenn etwas kaputt geht
- Deine Arbeit sicher und gesichert halten kannst
- An neuen Ideen arbeiten kannst, ohne das zu zerstören, was bereits funktioniert

Stell es dir wie "Änderungen verfolgen" in Microsoft Word vor, aber viel mächtiger und speziell für Software-Projekte entwickelt.

## Warum solltest du dich darum kümmern?

Wenn du Tools wie Lovable oder Bolt verwendest, können sie deine Arbeit automatisch in Git speichern. Das bedeutet:

- **Sicherheit**: Deine Arbeit ist in der Cloud gesichert (auf GitHub)
- **Verlauf**: Du kannst sehen, wie sich dein Projekt entwickelt hat
- **Rückgängig**: Einen Fehler gemacht? Du kannst zu dem Zeitpunkt zurückkehren, als alles funktioniert hat
- **Teilen**: Andere können deine Arbeit sehen und du kannst zusammenarbeiten

## Wichtige Konzepte

### Repository (Repo)

Ein **Repository** ist der Ordner deines Projekts, den Git überwacht. Es enthält:
- Alle deine Projektdateien
- Die komplette Historie der Änderungen
- Informationen darüber, wer welche Änderungen wann gemacht hat

Wenn du ein Projekt in Lovable oder Bolt erstellst und es mit GitHub verbindest, erstellst du ein Repository.

### Commit

Ein **Commit** ist wie ein Schnappschuss deines Projekts zu einem bestimmten Zeitpunkt. Jeder Commit speichert:
- Welche Änderungen du gemacht hast
- Eine Nachricht, die die Änderungen beschreibt
- Wann du sie gemacht hast

Stell dir Commits als Speicherpunkte in einem Videospiel vor - du kannst immer zu ihnen zurückkehren.

### Branch (Zweig)

Ein **Branch** ist wie eine parallele Version deines Projekts. Die Hauptversion heißt normalerweise `main` oder `master`.

**Für diesen Workshop**: Du wirst hauptsächlich mit dem main Branch arbeiten. Branches sind für fortgeschrittenere Workflows, aber es ist gut zu wissen, dass sie existieren!

### GitHub

**GitHub** ist eine Website, die deine Git-Repositories online speichert. Es ist wie Google Drive oder Dropbox, aber speziell für Code-Projekte mit Git entwickelt.

## Was du tatsächlich tun wirst

Bei der Verwendung von Lovable oder Bolt passiert folgendes mit Git:

### 1. Verbinde dein Tool mit GitHub

Dein KI-Tool (Lovable/Bolt) wird dich bitten, es mit deinem GitHub-Konto zu verbinden. Das ermöglicht es, deine Arbeit automatisch zu speichern.

### 2. Automatische Commits

Jedes Mal, wenn du Änderungen machst und die KI dein Projekt aktualisiert, erstellt sie einen Commit. Du wirst Nachrichten wie diese sehen:
- "Homepage-Design hinzugefügt"
- "Button-Stile aktualisiert"
- "Navigationsmenü repariert"

### 3. Sieh dir dein Projekt auf GitHub an

Du kannst zu GitHub.com gehen und sehen:
- Deine Projektdateien
- Historie aller Änderungen
- Wann jede Änderung gemacht wurde

## Grundlegende Aufgaben, die du machen kannst

### Repository anzeigen

1. Gehe zu [github.com](https://github.com)
2. Melde dich an
3. Klicke auf dein Profilbild (oben rechts)
4. Klicke auf "Your repositories"
5. Klicke auf deinen Projektnamen

### Projektverlauf anzeigen

Sobald du dein Repository betrachtest:

1. Suche nach dem "commits" Link (normalerweise oben, zeigt eine Zahl wie "24 commits")
2. Klicke darauf, um alle Änderungen über die Zeit zu sehen
3. Klicke auf jeden Commit, um genau zu sehen, was sich geändert hat

### Dateien anzeigen

Deine Repository-Seite zeigt alle deine Projektdateien. Du kannst:
- Auf jede Datei klicken, um ihren Inhalt zu lesen
- Sehen, wann sie zuletzt aktualisiert wurde
- Dateien herunterladen, falls nötig

### Projekt synchronisieren

Bei der Verwendung von Lovable oder Bolt:
- **Sie synchronisieren automatisch**, wenn du Änderungen machst
- Du musst nicht manuell "speichern" oder "hochladen"
- Änderungen erscheinen innerhalb von Sekunden/Minuten auf GitHub

## Häufige Begriffe, die du sehen wirst

| Begriff | Was es bedeutet |
|---------|-----------------|
| **Push** | Deine Änderungen von deinem lokalen Computer zu GitHub senden |
| **Pull** | Die neuesten Änderungen von GitHub zu deinem Computer holen |
| **Clone** | Eine Kopie eines Repositories erstellen |
| **Main/Master** | Die Hauptversion deines Projekts |
| **SHA/Hash** | Eine eindeutige ID für jeden Commit (sieht aus wie: `a3f2b9c`) |

**Hinweis**: Mit Lovable und Bolt passieren Push und Pull automatisch!

## Wenn etwas schief geht

### "Meine Änderungen erscheinen nicht auf GitHub"

- Warte eine Minute - die Synchronisation kann einen Moment dauern
- Prüfe, ob dein Tool noch mit GitHub verbunden ist
- Suche nach Fehlermeldungen in deinem Tool

### "Ich habe einen Fehler gemacht und möchte zurückgehen"

- Sage deinem KI-Tool: "Kannst du zu einer früheren Version zurückkehren?"
- Oder auf GitHub kannst du alte Commits anzeigen und Code von dort kopieren

### "Ich sehe mein Repository nicht auf GitHub"

- Stelle sicher, dass du in das richtige GitHub-Konto eingeloggt bist
- Prüfe, ob das Repository privat ist (du kannst nur deine eigenen privaten Repos sehen)
- Vergewissere dich, dass du den Verbindungsprozess mit deinem KI-Tool abgeschlossen hast

## Worum du dich nicht kümmern musst

Für diesen Workshop sind diese Themen über das hinaus, was du brauchst:

- **Merging** - Verschiedene Versionen kombinieren (fortgeschritten)
- **Rebasing** - Historie neu organisieren (fortgeschritten)
- **Pull Requests** - Formeller Weg, Änderungen vorzuschlagen (für Team-Workflows)
- **Merge Conflicts** - Wenn zwei Änderungen kollidieren (fortgeschritten)
- **Git-Befehle** - Terminal/Command Line Verwendung (deine Tools handhaben das)

Deine KI-Tools kümmern sich um die komplexen Sachen!

## Tipps für den Erfolg

1. **Lass es automatisch passieren** - Deine Tools handhaben Git für dich
2. **Schaue gelegentlich auf GitHub** - Es ist befriedigend, deinen Fortschritt zu sehen!
3. **Lies Commit-Nachrichten** - Sie erzählen die Geschichte, wie sich dein Projekt entwickelt hat
4. **Mach dir keinen Stress** - Git ist da, um dir zu helfen, nicht um dich zu verwirren
5. **Frag um Hilfe** - Wenn etwas falsch zu sein scheint, frag im Workshop oder schau es nach

## Möchtest du mehr lernen?

Sobald du mit den Grundlagen vertraut bist, sind diese Ressourcen großartig:

- [GitHub's Hello World Guide](https://guides.github.com/activities/hello-world/)
- [Git Handbook](https://guides.github.com/introduction/git-handbook/)
- [GitHub Learning Lab](https://lab.github.com/)

## Denk daran

Git ist ein mächtiges Tool, aber **du musst es nicht beherrschen**, um erstaunliche Dinge mit KI-Tools zu bauen. Deine Tools handhaben die komplizierten Teile, und dieses Wissen hilft dir nur zu verstehen, was hinter den Kulissen passiert.

Konzentriere dich auf das Bauen und Erstellen - Git ist da, um dich automatisch und leise zu unterstützen!

---

**Fragen während des Workshops?** Zögere nicht zu fragen! Git kann zunächst mysteriös erscheinen, aber es wird mit ein wenig Übung klar.
