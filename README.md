## Naturzoo-Rheine
# Programmablaufplan
1. Programmstart
2. Initialisierung des Systems
   - Verbindung zur MySQL-Datenbank herstellen
   - Systemparameter laden

3. Hauptmenü
   - [1] Eingabe (Verwaltung)
   - [2] Ausgabe (Abfrage durch Pfleger und Besucher)
   - [3] Beenden

4. Eingabe-Modus
   - Tierdaten eingeben
     - Art, Name, Geschlecht, Geburtsdatum, ggf. Todes-/Abgabedatum
     - Zuordnung: Revier, Gebäude, Pfleger
   - Futterdaten eingeben
     - Futterart, Lieferant, Menge, Lieferzeitplan
   - Protokollieren der Eingaben
   - Rückkehr zum Hauptmenü

5. Ausgabe-Modus
   - Auswahl der Benutzerrolle
     - [1] Verwaltung
        - Abfrage: Vollständige Datenbankansicht
        - Protokolle einsehen
     - [2] Pfleger
        - Abfrage: Futterplan pro Tier/Revier
     - [3] Besucher
        - Abfrage: Fütterungszeiten und Mengen pro Tier
   - Rückkehr zum Hauptmenü

6. Fehlerhandling
   - Eingabevalidierung (z.B. Pflichtfelder, Wertebereiche)
   - Protokollierung von Fehleingaben
   - Benutzerfreundliche Fehlermeldungen

7. Datenschutzmaßnahmen
   - Einschränkung der Zugriffsrechte
   - Verschlüsselte Speicherung sensibler Daten

8. Beenden
   - Datenbankverbindung schließen
   - Log-Dateien sichern
   - Programm beenden
