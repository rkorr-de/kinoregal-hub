# kinoregal-hub

Cast-Receiver-Seite für die Filmanzeige auf dem Nest Hub Max ("Wohnzimmer Display").
Nur HTML/JS, keine Daten und keine Schlüssel: Titel, Cover und Dauer schickt Kinoregal beim Casten mit.
Wird über GitHub Pages unter https://rkorr-de.github.io/kinoregal-hub/ ausgeliefert.

Kamera-Alarm: Die TV-App (PLEX+) schickt bei Person oder Bewegung an einer Nest-Kamera ein Standbild (`{"typ":"kamera",…}`), das 30 s über allem steht.

`stille.mp3` (10 min Stille, 8 kbit/s): spielt die Seite selbst, solange sie Film, Musik oder Kamera der TV-App zeigt, damit der Nest Hub keinen Bildschirmschoner darüberlegt.

Ruheseite: `{"typ":"ruhe","ort","temp","wetter"}` (alle 5 min, solange PLEX+ ohne Film und Musik läuft) zeigt große Uhr, Datum und Wetter.

Korraoke: `{"typ":"karaoke",…}` (Format im Kopf von index.html) zeigt Sänger, Lied mit Fortschritt, Warteschlange und QR/Raumcode.
