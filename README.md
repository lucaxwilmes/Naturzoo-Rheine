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
