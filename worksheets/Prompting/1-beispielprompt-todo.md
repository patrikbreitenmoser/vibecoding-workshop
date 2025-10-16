# Beispiel-Prompt für To-Do App
Du bist mein Assistent. Erstelle eine To-do-App für eine Einzelperson. Implementiere ausschliesslich die folgenden Funktionen, Interaktionen und Regeln. 

Ziel und Nutzerbild:
- Einzelperson verwaltet persönliche Aufgaben, kurz und klar. Deutschsprachige Oberfläche.

Aufgabe anlegen:
- Pflichtfelder: Titel.
- Optionale Felder: Beschreibung, Fälligkeitsdatum, Priorität, Tags, Teilaufgaben.
- Validierung: Titel darf nicht leer sein. Fälligkeitsdatum darf bei Erstellung nicht in der Vergangenheit liegen.

Felder und Werte:
- Priorität: Hoch, Mittel, Tief. Standardwert ist Mittel.
- Status: Offen, In Arbeit, Erledigt. Standardwert ist Offen.
- Tags: freie Stichwörter, mehrere pro Aufgabe möglich.
- Teilaufgaben: Liste kurzer Punkte mit eigenem Abhakstatus.

Status- und Regelwerk:
- Eine Aufgabe kann genau einen Status haben.
- Setze Status automatisch auf Erledigt, wenn alle Teilaufgaben abgehakt sind.
- Beim Zurücksetzen einer Teilaufgabe wechsle die übergeordnete Aufgabe automatisch auf Offen.

Ansichten und Filter:
- Heute: alle offenen Aufgaben mit Fälligkeitsdatum heute, sortiert nach Fälligkeitsdatum dann Priorität.
- Überfällig: offene Aufgaben mit Fälligkeitsdatum vor heute, gleiche Sortierung.
- Nächste 7 Tage: offene Aufgaben mit Fälligkeitsdatum innerhalb der kommenden 7 Kalendertage.
- Erledigt: erledigte Aufgaben, zuletzt Erledigtes zuerst.
- Tag-Filter: filtere nach einem oder mehreren Tags.
- Textsuche: suche in Titel und Beschreibung, Teiltreffer zulässig.

Wiederkehrende Aufgaben:
- Wiederholung optional: täglich, wöchentlich, monatlich.
- Beim Abhaken einer wiederkehrenden Aufgabe wird automatisch die nächste Instanz erzeugt:
  - Täglich: Fälligkeitsdatum +1 Tag.
  - Wöchentlich: Fälligkeitsdatum +7 Tage.
  - Monatlich: gleiches Tagesdatum im Folgemonat, falls nicht vorhanden nächstmögliches Datum.

Bearbeitung und Konsistenz:
- Inline-Bearbeitung von Titel, Beschreibung, Fälligkeitsdatum, Priorität, Tags.
- Wenn das Fälligkeitsdatum auf ein früheres Datum gesetzt wird als heute, verschiebe die Aufgabe automatisch in die Ansicht Überfällig, Status bleibt unverändert.
- Löschen nur, wenn die Aufgabe nicht wiederkehrend ist oder die Wiederholung zuvor deaktiviert wurde. Alternativ: Löschen bestätigt auch die Deaktivierung der Wiederholung.
