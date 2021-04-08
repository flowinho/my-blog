---
layout: post
title:  "Den HEAD eines GIT-Repositories fachgerecht exportieren"
tags: .git .bash
categories: ~/tools
---

GIT-Repositories sammeln im Laufe der Zeit recht viel Ballast, da die Unterschiede der einzelnen Revisions irgendwo gespeichert werden müssen. Nun könnte man das Verzeichnis kopieren, den `.git` Ordner löschen und das Ergebnis packen, beispielsweise mit tar.gz, oder man nutzt die in GIT eingebaute Archivierungsfunktion.

Nach Wechsel in das Verzeichnis welches das GIT-Repo enthält sollte man sicherstellen auf welchem Branch man sich befindet. Anschließend lassen sich beliebige Revisionen archivieren, hier am Beispiel von `~HEAD`

```bash
git archive --output=../archive-2021-04-08.tar.gz --format=tar HEAD
```

Viel Spaß beim Packen 📦