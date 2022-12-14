# AA_Team_12_Assignment

## Setup
- Github Account erstellen
- Git installieren
- Jupyter notebook oder IDE (z.B. Visual Studio Code) nutzen - letzteres evtl. einfacher, bei jupyter notebook müsstet ihr git bash nutzen zum downloaden und hochladen des Codes
- Ordner erstellen für Projekt

- Git login (wenn neu installiert) 

Dazu am besten in IDE Terminal öffnen (mit Strg+Shift+Ö) oder im Ordner rechtsklick "Weitere Optionen anzeigen" -> Git bash öffnen. Dann Name und Password von github.com hinterlegen. Wenn es nicht klappt auch mail hinterlegen.


>`git config --global user.name "UserName"`

>`git config --global user.password "Password"`

>`git config --global user.email "BeispielMail@mail.com"`

- Remote repo von github.com downloaden

`git clone https://github.com/JuliusScheuerer/AA_Team_12_Assignment.git`

- Ggf. mit remote repo verbinden (in IDE Terminal oder Git bash)
1. Test: `git remote add origin https://@github.com/JuliusScheuerer/AA_Team_12_Assignment.git`
2. Test: `git remote add origin https://<UserName>:<Passwort>@github.com/JuliusScheuerer/AA_Team_12_Assignment.git`


- Beide zips aus WhatsApp downloaden und entzippen. Dann datasets im gleichen Ordner wie AA_Team_12_code.ipynb ablegen und csv in datasets ablegen.

- Dann git commands unten testen


## Wichtige Git commands: 

Erstellen einer neuen lokalen branch, z.B. feature-branch `<data-prep-and-cleaning>`, hier einfacher `<eigener-name>`:
```
git checkout -b <name-der-branch>
```
Added alle geänderte Dateien in staging area ("bereit hochgeladen zu werden"):
```
git add .
```

Änderungen werden commited mit einer Nachricht, z.B. `data preparation` oder `kpi revenue implementiert`:
```
git commit -m <nachricht-deiner-wahl>
```

Änderungen auf der lokalen branch werden in remote branch auf github.com hochgeladen:
```
git push
```

Beim erstmaligen Erstellen einer lokalen branch (s.o.) muss diese zunächst remote gepusht werden:
```
git push --set-upstream origin <name-der-branch>
```
Änderungen der remote branch auf lokale branch downloaden:
```
git pull
```
Wechseln der lokalen branch:
```
git checkout <name-der-branch>
```
Sollte es zu Fehlermeldungen kommen, bspws. durch den Versuch zu pushen vor dem pullen von remote Änderungen o.Ä., googlen oder mich fragen :)
