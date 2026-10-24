# Voxel – Downloads

Hier liegen die fertigen Fassungen des Spiels **Voxel** (Blockwelt mit realistischer Grafik, Godot 4). Dieses Repo enthält keinen Quellcode, nur die Dateien zum Spielen.

## Spielen

1. Unter [Releases](../../releases/latest) die Datei `Voxel.exe` herunterladen (Windows 10/11, 64 Bit, etwa 150 MB).
2. In einen eigenen Ordner legen (zum Beispiel `C:\Spiele\Voxel\`) und starten. Ein Installationsprogramm gibt es nicht.
3. Beim ersten Start meldet sich Windows SmartScreen, weil die Datei nicht signiert ist: „Weitere Informationen“ und dann „Trotzdem ausführen“.

Das Spiel sucht beim Start selbst nach neuen Fassungen und tauscht sich auf Wunsch aus. Welten und Einstellungen liegen unter `%APPDATA%\Godot\app_userdata\Voxel` und bleiben beim Aktualisieren erhalten.

Die Prüfsumme zu jeder Datei steht in der zugehörigen `.sha256`-Datei.

## Eigener Server (Linux, NAS)

`voxel-server-linux.x86_64` ist der eigenständige Server für Linux (`--server`, `--relay`). Für ein NAS mit Docker gibt es das fertige Paket `voxel-nas-<Fassung>.zip` mit Anleitung.

## Empfohlene Server

`servers.json` in diesem Repo enthält die Liste der empfohlenen Server, die das Spiel oben in der Serverliste als „Empfohlen“ zeigt. Felder je Eintrag: `name`, `address` (Host:Port für ENet), `wss` (Tunnel-Adresse, optional), `fingerprint` (DTLS-Fingerabdruck des Servers), `motd`, `relay`.
