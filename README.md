
# MeinProjekt

Dieses Repository dokumentiert die Schritte zur Einrichtung eines GitHub-Repositories und eines Workflows. Es enthält eine lokale Implementierung des Projekts sowie die Dokumentation.

## 1. GitHub Repository Setup

### Schritte
1. GitHub aufgerufen und neues Repository erstellt: `MeinProjekt`.
2. SSH-URL des Repositories: `git@github.com:DeinBenutzername/MeinProjekt.git`.

---

## 2. Erstellen eines SSH-Schlüssels

### Schritte
1. Überprüfung auf vorhandenen Schlüssel: `ls ~/.ssh/`
2. Neuer SSH-Schlüssel erstellt: `ssh-keygen -t rsa -b 4096 -C "deine_email@beispiel.com"`.
3. Öffentlichen Schlüssel zu GitHub hinzugefügt.

---

## 3. Lokales Repository eingerichtet

### Schritte
1. Repository geklont: `git clone git@github.com:DeinBenutzername/MeinProjekt.git`.
2. Git konfiguriert:
    ```bash
    git config user.name "Dein Name"
    git config user.email "deine_email@beispiel.com"
    ```
3. Datei `main.py` hinzugefügt und initialer Commit erstellt.

---

## 4. Branch-Management und Merge-Konflikt

### Schritte
1. Neuen Branch erstellt: `git checkout -b feature`.
2. Datei `utils/database.py` hinzugefügt und Commit erstellt.
3. Änderungen in `main.py` auf "feature"-Branch vorgenommen und Commit erstellt.
4. Zurück zum "master"-Branch und dort Änderungen vorgenommen.
5. Merge durchgeführt: `git merge feature` und Konflikt in `main.py` manuell gelöst.

---

## 5. Repository gepusht

1. Änderungen nach GitHub hochgeladen: `git push origin master`.


    