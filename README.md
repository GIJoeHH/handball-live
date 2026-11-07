# Handball Live

Web-App zum Vorbereiten, Live-Erfassen und Analysieren von Handballspielen auf dem iPad. Sie läuft nach dem ersten Öffnen komplett offline.

**Reiter:**
1. **Vorbereitung:** Spieldaten, Gegner, Kader und Schwerpunkte. Dazu Gegner-Scouting aus mehreren Spielberichten von handball.net.
2. **Spiel erfassen:** Ballbesitz für Ballbesitz mit Spielzug, Wurfort, Qualität, Werfer, Assist, Abwehrspieler und Ergebnis. Eine Hinweisleiste zeigt Auffälligkeiten live.
3. **Analyse:** Spielbericht-Import und Abgleich, Auffälligkeiten in Angriff und Abwehr, Ursachen, Wurfbild und Spielerübersicht.

Alle Daten, auch importierte Namen, bleiben im Browser des Geräts. Auf keinem Server wird etwas gespeichert.

## Veröffentlichen mit GitHub Pages

1. Den Inhalt dieses Ordners in ein GitHub-Repository legen, zum Beispiel `handball-live`.
2. Auf GitHub: **Settings → Pages → Build and deployment**. Bei *Source* „Deploy from a branch“ wählen, dann Branch `main` und Ordner `/ (root)`. Speichern.
3. Nach ein bis zwei Minuten ist die App erreichbar unter `https://<github-name>.github.io/handball-live/`.

## Auf dem iPad installieren

1. Die Adresse in **Safari** öffnen, mit Internet.
2. Teilen-Symbol → **Zum Home-Bildschirm**.
3. Die App einmal über das neue Symbol öffnen und kurz warten. Danach läuft sie auch ohne Internet.

Empfehlungen für den Spieltag:
- Automatische Sperre auf „Nie“ stellen. Die App versucht während der Erfassung zusätzlich, den Bildschirm wach zu halten.
- Optional *Geführter Zugriff* einschalten, damit die App nicht versehentlich verlassen wird.
- Nach dem Spiel im Reiter Analyse auf **„Daten sichern“** tippen und die Sicherung zum Beispiel in iCloud ablegen.

## Updates

Nach Änderungen an `index.html` in `sw.js` die Zeile `const VERSION = 'v1';` hochzählen, zum Beispiel auf `'v2'`. Die iPads laden die neue Fassung beim nächsten Öffnen mit Internet; die App meldet dann „Neue Version geladen“.

Wichtig: Die Daten hängen an der Adresse der App. Wer die Adresse wechselt, etwa auf ein anderes Repository, startet mit leeren Daten. Vorher „Daten sichern“.
