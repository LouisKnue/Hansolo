# Adminhandbuch

## Lokales Repository erstellen

### SSH Key erstellen und einfügen

1. Auf Github mit seinem Konto anmelden

2. Powershell starten

3. Folgendes eingeben:
```
ssh-keygen -t ed25519
```

4. Danach den public Key unter einstellungen als SSH Key einfügen

5. Erstelle auf deinem Github account ein neues Repository 


### Git auf den PC installieren

1. Powershell starten

2. Folgendes eingeben:
   
3. ```
   winget install -e --id Git.Git
   ```
4. Nun Sollten drei apps Installiert sein. Git GUI, Git Bash und Git CMD.

### Lokales Repository anlegen

1. Du bewegst dich in den Ordner Dokumente und legst dort einen neuen Ordner namens s23BIT2 an.

2. Dort gehst du rein und erstellst den Ordner Firstrepo.

3. Hier gehst du wieder rein und erstellst mit dem unten genannten befehl ein repository:
   ```
   git init
   ```
4. Mit den unten genannten befehlen kannst du nun in dein Repository rein gehen und dateien erstellen.
   ```
   git branch -M main
   touch test.md
   nano test.md
   ```
   In der Datei kannst du jetzt änderungen vornehmen und mit STRG+X und 'Yes' wieder heraus gehen.

### Die datei dem Repository hinzufügen

1. Mit ``` git status``` kannst du einsehen was du zutun hast. Wenn dort in rot deine Datei auftaucht hast du alles richtig gemacht.

2. Mit ```git add test.md``` wird die Datei dem Repository hinzugefügt

3. Da du dich das erste mal anmeldest musst du ``` git commit -m "first commit"``` eingeben. Dort wirst du dann aufgefordert deine Email und deinen Namen einzutragen.

4. Mit ``` git remote add origin git@github.com:LouisKnue/Hansolo.git``` kann man dann die datei Hochladen und mit ``` git push -u origin main``` wird das ganze gepusht.

5. Dann kannst du die Github seite neu Laden und alles ist fertig.
