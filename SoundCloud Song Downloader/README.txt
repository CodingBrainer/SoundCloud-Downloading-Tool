# SoundCloud Playlist and Song Downloader

## 📌 Description
This script allows you to download individual songs or entire playlists from SoundCloud and convert them into MP3 format.

---

## 📥 Installation Guide

### 🖥️ Step 1: Install Python (If Not Installed)
Ensure you have Python 3 installed. You can download it from:
https://www.python.org/downloads/

To check if Python is installed, run:

python3 --version

---

### 🛠️ Step 2: Install Dependencies
Navigate to the folder containing this project and run:

pip -r requirements.txt

This will install:
- `yt-dlp` (for downloading from SoundCloud)
- `ffmpeg-python` and `imageio[ffmpeg]` (for audio conversion)

---

### 🎵 Step 3: Install FFmpeg
FFmpeg is required to convert downloaded files into MP3.

#### **Windows Installation:**
1. Download FFmpeg from:  
   https://ffmpeg.org/download.html  
   (Choose "Windows builds from gyan.dev" and download "ffmpeg-release-essentials.zip")
2. Extract it to `C:\ffmpeg\`
3. Add `C:\ffmpeg\bin` to the system PATH:
   - Press **Win + R**, type **sysdm.cpl**, and hit Enter.
   - Go to **Advanced** → **Environment Variables**.
   - Under **System variables**, find `Path` and click **Edit**.
   - Click **New**, then add `C:\ffmpeg\bin`.
   - Click **OK** → Restart your computer.

#### **macOS Installation:**
Install via Homebrew:

brew install ffmpeg

sudo apt update && sudo apt install ffmpeg -y

(For Fedora, use `dnf install ffmpeg -y` instead)

To verify installation, run:

ffmpeg -version

---

## 🚀 How to Use
1. Run the script:

python soundcloud_downloader.py

2. Choose an option:
   - **1** to download a single song
   - **2** to download a full playlist
3. Enter the SoundCloud URL.
4. The files will be downloaded and saved in the `downloads/` folder.

---

## ❓ Troubleshooting
- **FFmpeg Not Found?**
  - Make sure FFmpeg is installed and added to the system PATH.
- **Download Fails?**
  - Double-check the SoundCloud URL.
  - Try updating `yt-dlp`:
    ```
    pip install --upgrade yt-dlp
    ```
- **Files Not Converting to MP3?**
  - Run the script with admin privileges.
  - Ensure FFmpeg is installed and correctly configured.

---

## ✅ Credits
This project uses:
- `yt-dlp` for downloading SoundCloud tracks
- `FFmpeg` for audio conversion

Enjoy your music downloads! 🎶


------------------------------------------------------------------

Thank you for using my program. I hope you enjoy my future projects - CodingBrainer