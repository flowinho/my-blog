---
layout: post
title:  "macOS: VLC das Streamen von YouTube-Videos (wieder) beibringen"
---

VLC ist seit meiner Jugend eine absolute Allzweckwaffe. Das [französische Studentenprojekt](https://www.vlc.de/vlc_informationen.php) mauserte sich in kürzester Zeit nicht nur zu einem etablierten Media Player, sondern zu dem Standard in Sachen Videowiedergabe. Auch in Sachen Multiplattform existiert ein entsprechendes Derivat für die gängigsten Betriebssystem, nämlich Android, iOS, Linux, macOS und Windows. Entsprechend häufig ist dieses kleine Software-Meisterwerk auf nahezu jedem Desktop-PC oder Notebook zu finden.

![](/assets/images/vlc_kripp.png)

VLC bietet ein Funktion zum Abspielen von Netzwerkstreams, die auch in der Lage ist YouTube-Videos innerhalb des Players abzuspielen. Doch warum sollte man das wollen? Nun, es bringt so einige Vorteile:

- Es lassen sich Playlisten anlegen.
- Audio- und Video-Einstellungen wie Equalizer, Gamma, Scharfzeichnung, Wiedergabe-Geschwindigkeit und weitere Parameter lassen sich einstellen. Diese Konfigurationsmöglichkeiten sind auf der Website nicht vorhanden.
- Die Videos können abgespielt werden, ohne dass der Browser geöffnet sein muss.
- Es können erweiterte Tastatur-Shortcuts benutzt werden.
- Das Ausgabemedium für Ton und Bild lässt sich wählen. Video über AirPlay, Ton über ein dediziertes Soundsystem? Solange VLC dieses erkennt, ist das kein Problem. Auch hier eine deutliche Verbesserung gegenüber YouTube im Browser.

Doch leider funktioniert das Abspielen von YouTube-Videos nicht auf Anhieb. Fügt man den YouTube-Link in das Dialogfeld des Menüs “Netzwerk öffnen” ein, passiert zumindest unter macOS erst einmal leider gar nichts. Das liegt darin begründet dass das YouTube-Plugin, vermutlich aus lizenzrechtlichen Gründen, standardmäßig nicht mitgeliefert wird. Beheben lässt sich diese “Fehlverhalten” auf folgende Weise.

- Ladet euch das Plugin einfach direkt von GitHub herunter. Entweder durch Rechtsklick -> Ziel speichern unter oder ihr öffnet den Link und kopiert den Inhalt in einen Texteditor eurer Wahl, um die dann eine Datei mit den Name youtube.luac abzuspeichern.
- Stellt sicher dass die Dateiendung luac lautet und nicht lua.
- Verschiebt die Datei in /Applications/VLC.app/Contents/MacOS/share/lua/playlist/.
- Startet VLC neu.

Das wars. =)

