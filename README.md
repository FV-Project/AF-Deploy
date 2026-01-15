# AF-Deploy

Ein einfaches Docker-Compose Setup zum Deployen von Node.js Projekten.

## Download

Lade alle benötigten Dateien direkt von GitHub herunter:

**[📦 Download alle Dateien als ZIP](https://github.com/FV-Project/AF-Deploy/archive/refs/heads/main.zip)**

Oder lade die einzelnen Dateien herunter:

- [docker-compose.yml](https://raw.githubusercontent.com/FV-Project/AF-Deploy/main/docker-compose.yml)
- [.env](https://raw.githubusercontent.com/FV-Project/AF-Deploy/main/.env)
- [.gitignore](https://raw.githubusercontent.com/FV-Project/AF-Deploy/main/.gitignore)
- [.gitattributes](https://raw.githubusercontent.com/FV-Project/AF-Deploy/main/.gitattributes)

## Verwendung

1. Lade die vier Dateien herunter
2. Passe die `.env` Datei an deine Bedürfnisse an:
   - `Project_Folder`: Name deines Projekt-Ordners
   - `APP_Port`: Port auf dem die App laufen soll
   - `PACKAGE_MANAGER`: npm oder pnpm (oder auto für automatische Erkennung)
3. Lege dein Node.js Projekt in den Ordner, der in `Project_Folder` angegeben ist
4. Starte mit `docker-compose up -d`

## Features

- 🚀 Automatische Paketmanager-Erkennung (npm/pnpm)
- 🔄 Auto-Restart bei Fehlern
- 📦 Unterstützt Build-Schritt vor dem Start
- 🐳 Verwendet Node.js 22 Alpine (klein & schnell)
