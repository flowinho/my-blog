---
layout: post
title:  "Nicht noch ein Post über Visual Studio Code - aber dieses Mal wird alles anders!"
---

Ich weiß, ich weiß. Jetzt bloggt auch noch Flo über Visual Studio Code. So langsam sollte doch alle Welt begriffen haben, dass VSCode den neuen Standard der Text-Editoren setzt. Oder doch nicht? Ich möchte mich mal an Blickwinkel versuchen, der meiner Meinung nach etwas Aufmerksamkeit verdient.

> Nicht Microsoft macht Visual Studio Code zu dem was es ist, sondern die Community. Und leider bekommt man nicht die Software, die versprochen wird.

VSCode sollte differenzierter betrachtet werden. Es stimmt, dass VSCode "die Welt im Sturm erobert hat". [Google Mitarbeiter](https://www.cnbc.com/2018/12/20/microsoft-cmo-capossela-says-google-employees-use-visual-studio-code.html) nutzen es, Facebook ["umarmt Visual Studio Code"](https://visualstudiomagazine.com/articles/2019/11/21/fb-vs-code.aspx) und die repräsentativen Umfragen in einem  der größten Entwickler-Netzwerke der Welt [untermauern die Annahme dass es sich bei VSCode um die beliebteste IDE handelt.](https://insights.stackoverflow.com/survey/2018/)

Doch warum schreibe ich darüber, dass man VSCode differenzierter betrachten muss? 

Nun, folgendes:

**Microsoft hätte gerne dass VSCode als IDE betrachtet wird.** 

![](/assets/images/2020-12-04-vscode.png)

VSCode ist in erster Linie ein modularer, erweiterbarer **Text-Editor**. Zu einer IDE für bestimmte Sprachen wird diese Software erst, wenn Sie durch die Community entsprechend *erweitert wird.* Und genau hier steckt der Knackpunkt: Microsoft stellt mit VSCode ein, zugegebenermaßen sehr solides, Grundgerüst bereit, dass von der Community erst zu dem gemacht wird, dass es bis heute geworden ist. 

Beispielsweise sorgt die Community für:
  - Die Erweiterung des Editors um **Sprachen** wie SWIFT, GO und PERL sowie *Versuchen* für diese Sprachen entsprechende Compiler zur Verfügung zu stellen.
  - Die Erweiterung des Editors um **Themes**, ein Faktor der tatsächlich leider nicht vernachlässigt werden sollte, bestimmen doch Übersicht, Fontwahl und Farbwahl, insbesondere bei Syntax-Highlighting, über die tägliche Nutzbarkeit des Editors. Durch das Angebot an **Community**-Themes findet jeder etwas.
  - Die Erweiterung des Editors um **Funktionen**, wie etwa tiefgreifende GIT-Integration, LaTeX-Zeichensetzung, 

**VSCode ist zwar Open Source, aber Microsoft bindet weitreichende Telemetrie in den Editor ein.** 

Es ist sogar noch schlimmer. Der Programmcode des Editors ist frei verfügbar, allerdings erhält man von Microsofts Download-Servern **eine veränderte Version**. Dieser Umstand allein ist erschreckend genug, aber Microsoft wählt für diese abgeänderte Version sogar eine [proprietäre Lizenz.](https://code.visualstudio.com/license). Microsoft macht keinen Hehl daraus, die Entwickler [sprechen offen auf GitHub darüber.](https://github.com/Microsoft/vscode/issues/60#issuecomment-161792005). Unter anderem aufgrund dieser Umstände sahen es einige Entwickler für notwendig an mit [VSCodium](https://vscodium.com) eine *echte Open Source Variante* von Visual Studio Code anzubieten.

> The VSCodium project exists so that you don’t have to download+build from source. This project includes special build scripts that clone Microsoft’s vscode repo, run the build commands, and upload the resulting binaries for you to GitHub releases. These binaries are licensed under the MIT license. Telemetry is disabled.

Visual Studio Code ist sicherlein ein toller **Editor**, und **kann, wenn durch die Community dazu ermächtigt**, eine *Erweiterung* zu einer IDE darstellen, dieser aber in den meisten Fälle nicht *ersetzen.* Meiner Meinung nach lehnt sich Microsoft hier aber zu weit aus dem Fenster. 

- Die Arbeit der Community wird nicht genug betont.
- Microsoft bewirbt einen Text-Editor als Intelligent Development Environment.
- Nutzer erwarten eine Open Source Software, erhalten aber eine proprietäre Lizenz - aka. "Mogelpackung".
- Nutzer vertrauen Open Source Software unter anderem auch aufgrund der Tatsache dass Tracking nur begrenzt eingebettet werden kann, bevor dieses der Community auffällt. Microsoft greift hier zu etwas fadenscheinigen Methoden, um Telemetrie dennoch unter die User zu bekommen.

**Ein typischer Microsoft Snitch-Move.**

Wie schade. Gottseidank gibt es in VSCodium eine Möglichkeit von der Arbeit der talentierten VSCode-Entwickler zu profitieren ohne gleich jedes Spielchen seitens MS mitmachen zu müssen.

[Hier geht es zu VSCodium](https://vscodium.com)



