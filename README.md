<meta name="google-site-verification" content="nzH-PhV2Ni9dHbwKxh2-MihmDu18zGX10Y2v2TTkpZg" />

# YouTube-Downloader GUI

Ein plattformübergreifendes Tool zum Herunterladen von Videos und Audios von YouTube, Vimeo, TikTok und anderen Plattformen.

## 📋 Inhaltsverzeichnis
1. [Funktionen](#-funktionen)
2. [Voraussetzungen](#-voraussetzungen)
3. [Installation](#-installation)
4. [Verwendung](#-verwendung)
5. [Konfiguration](#-konfiguration)
6. [Unterstützte Plattformen](#-unterstützte-plattformen)
7. [Fehlerbehebung](#-fehlerbehebung)
8. [Lizenz](#-lizenz)

## 🚀 Funktionen
- **Multiplattform-Downloads** von 6 beliebten Diensten
- **Intuitive GUI** mit Tkinter-Oberfläche
- **Wahl zwischen Video (MP4)** und **Audio (MP3)**
- **Adaptive Qualitätseinstellungen**:
  - *Video*: 1080p bis 240p
  - *Audio*: 32-320 kbps
- **Playlist-Unterstützung** für Batch-Downloads
- **Automatische Speicherung** der letzten Einstellungen
- **Fortschrittsbalken** mit 5%-Update-Intervallen
- **Plattformübergreifende Kompatibilität** (Windows/Linux/macOS)

## 🛠 Voraussetzungen

### 📦 Python-Pakete
``pip install yt-dlp tkinter``

### 🖥 Systemabhängigkeiten (Debian/Ubuntu)
``sudo apt install ffmpeg libx11-6 libxext6 libxrender1``

## 📥 Installation

1. Repository klonen: ```git clone https://github.com/Theo555/Youtube-Downloader-GUI.git```
2. ```cd ytdlp-gui```

3. Ausführungsrechte setzen:
```chmod +x ytdlp.py```

4. Starten der Anwendung:
```./ytdlp.py```

## 🖱 Verwendung
1. **Plattform auswählen** aus dem Dropdown-Menü.
2. **URL einfügen** (Rechtsklick → Einfügen oder Strg+V).
3. **Zielordner** festlegen (Standard: Aktuelles Verzeichnis).
4. **Format wählen**:
   - **MP4** mit Qualitätsstufen (Beste/Mittlere/Niedrigste).
   - **MP3** mit Bitraten von 32-320 kbps.
5. Download starten mit entsprechendem Button.

## ⚙ Konfiguration
Einstellungen werden automatisch in `settings.ini` gespeichert:

[Settings]

```video_quality = 0    # 0=Beste, 1=Mittel, 2=Niedrig```

```audio_quality = 0    # 0=320kbps, ..., 5=32kbps```

```platform = 0         # 0=YouTube, ..., 5=Twitter```

```download_folder = /pfad/zum/ordner```

## 🌐 Unterstützte Plattformen
| Plattform    | Video | Audio | Playlists |
|--------------|-------|-------|-----------|
| YouTube      | ✅    | ✅    | ✅        |
| Vimeo        | ✅    | ✅    | ❌        |
| Dailymotion  | ✅    | ❌    | ✅        |
| SoundCloud   | ✅    | ✅    | ✅        |
| TikTok       | ✅    | ✅    | ❌        |
| Twitter      | ✅    | ❌    | ❌        |

## 🔧 Fehlerbehebung

### Fehler: Tkinter nicht installiert
```sudo apt install python3-tk```

### Fehler: "ffmpeg nicht gefunden"
```sudo apt install ffmpeg && pip install --upgrade yt-dlp```


### Download-Abbruch bei Playlists:
- Prüfen Sie die Internetverbindung.
- Reduzieren Sie die Qualitätseinstellung.

## 📄 Lizenz

MIT License

Copyright (c) 2025 TK

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.



