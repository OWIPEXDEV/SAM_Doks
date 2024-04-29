### README

---

#### Projektbeschreibung
Dieses Repository enthält Skripte und Konfigurationen für das Projekt owipex-sps, entwickelt von KARIM Technologies.

---

#### Installationsanweisungen
1. Klone das Repository:
   ```bash
   git clone https://github.com/KARIM-Technologies/owipex-sps.git

Navigiere zum Verzeichnis der Installations-Skripte:
bash
Copy code
cd owipex-sps/installer/initial/
Mache das Skript bootSpeeder.sh ausführbar:
bash
Copy code
sudo chmod +x bootSpeeder.sh
Führe das Skript bootSpeeder.sh aus:
bash
Copy code
sudo ./bootSpeeder.sh
Falls Fehler auftreten, siehe die Logs mit:
bash
Copy code
systemctl status systemd-networkd-wait-online.service
journalctl -xeu systemd-networkd-wait-online.service
Einrichtungsanweisungen
Führe das Einrichtungs-Skript aus:
bash
Copy code
sudo python3 setupBot.py
Gib bei Aufforderung den gewünschten Hostnamen ein (z.B. 9240011).
Folge den Anweisungen, um einen neuen Routing-Schlüssel und ein Geheimnis zu generieren.
Gib die erforderlichen Passwörter ein, wenn du dazu aufgefordert wirst.
Falls eine .env-Datei bereits existiert, wird sie nicht überschrieben.
Das Einrichtungs-Skript erstellt eine Systemd-Service-Datei für powerWatchdog, lädt die Systemd-Konfiguration neu, aktiviert und startet den powerWatchdog-Service.
Wenn du dazu aufgefordert wirst, wähle aus, das System neu zu starten.
