# Naturzoo-Rheine
## Programmablaufplan
1. Programmstart
2. Initialisierung des Systems
   - Verbindung zur MySQL-Datenbank herstellen
   - Systemparameter laden

3. Ausgabe-Modus
   - Auswahl der Benutzerrolle
     - [1] Verwaltung
        - Abfrage: Vollständige Datenbankansicht
        - Protokolle einsehen
     - [2] Pfleger
        - Abfrage: Futterplan pro Tier/Revier
     - [3] Besucher
        - Abfrage: Fütterungszeiten und Mengen pro Tier
   - Rückkehr zum Hauptmenü

4. Fehlerhandling
   - Eingabevalidierung (z.B. Pflichtfelder, Wertebereiche)
   - Protokollierung von Fehleingaben
   - Benutzerfreundliche Fehlermeldungen

5. Datenschutzmaßnahmen
   - Einschränkung der Zugriffsrechte
   - Verschlüsselte Speicherung sensibler Daten

8. Beenden
   - Datenbankverbindung schließen
   - Log-Dateien sichern
   - Programm beenden
     
## Programmplanung und Dokumentation: NaturZoo Rheine

1. Einleitung

Der NaturZoo Rheine plant, sein bestehendes Karteikartensystem für die Verwaltung von Tieren, Pflegern und Fütterungen durch ein digitales Datenbanksystem zu ersetzen. Gleichzeitig soll der Internetauftritt überarbeitet werden, um verschiedene Benutzerrollen (Verwaltung, Pfleger, Besucher) mit spezifischen Anforderungen zu bedienen. Diese Dokumentation beschreibt die Planung des Programms, basierend auf den Anforderungen des Lastenhefts.

2. Zielsetzung

   - Digitalisierung der Tier-, Pfleger- und Futterverwaltung mit einer relationalen MySQL-Datenbank.

   - Bereitstellung einer benutzerfreundlichen Weboberfläche für die Verwaltung, Pfleger und Besucher.

   - Sicherstellung von Datenschutz und Fehlertoleranz.

   - Protokollierung aller Vorgänge und Einhaltung ergonomischer Prinzipien.

3. Anforderungen


   - Verwaltung: Eingabe und Bearbeitung von Tier-, Pfleger- und Futterdaten sowie Erstellung eines wöchentlichen Futterplans.

   - Pfleger: Zugriff auf spezifische Futterpläne und Tierinformationen.

   - Besucher: Einsicht in öffentlich zugängliche Informationen (z. B. Fütterungszeiten).

   - Benutzerfreundlichkeit: Intuitive und einheitliche Oberfläche.

   - Fehlertoleranz: Abfangen von Fehleingaben ohne Systemabstürze.

   - Plattformunabhängigkeit: Lauffähig auf aktuellen Rechnern und Browsern.

4. Systemübersicht

Datenbankdesign

   - Die relationale MySQL-Datenbank enthält folgende Tabellen:

   - Tiere: Art, Name, Geschlecht, Geburtsdatum, Todes-/Abgabedatum.

   - Pfleger: Name, Adresse, Telefon, Geburtsdatum.

   - Futter: Art, Lieferant, Menge, Lieferzeitplan.

   - Reviere: Zuordnung von Tieren und Pflegern.

Weboberfläche

   - Verwaltungsbereich: Eingabe- und Bearbeitungsmasken.

   - Pflegerbereich: Anzeige der relevanten Daten.

   - Besucherbereich: Öffentliche Informationen über Tiere und Fütterungszeiten.

5. Projektplanung

Projektphasen

Analysephase:

   - Anforderungen validieren und dokumentieren.

   - Erstellung eines ER-Diagramms.

Entwurfsphase:

   - Datenbankstruktur entwerfen.

   - Programmablaufplan und Maskendesign erstellen.

Implementierungsphase:

   - Entwicklung der MySQL-Datenbank.

   - Implementierung der Webanwendung.

Testphase:

   - Unit- und Integrationstests.

   - Benutzerakzeptanztests (UAT).

Einführungsphase:

   - Schulung der Mitarbeiter.

   - Deployment der Anwendung.
