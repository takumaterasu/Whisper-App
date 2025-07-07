# 📱 Installation Guide - WhisperApp Standalone

## 🎯 Autonomous Version - All-Inclusive!

This **standalone** version of WhisperApp bundles **all required binaries** and **automatically** downloads the Whisper model on first launch.

✅ **No manual setup needed!**
✅ **Works immediately after installation**
✅ **Automatic model download**

---

## 📋 System Requirements

* **macOS**: 14.0 or newer
* **CPU**: Intel (x86\_64) or Apple Silicon (M1/M2/M3)
* **RAM**: 4 GB minimum recommended
* **Disk Space**: 2 GB free (for the Whisper model)
* **Internet**: Required on first launch to download the model

---

## 🚀 Quick Installation

### Option 1: DMG (Recommended)

1. **Download** `WhisperApp-Standalone-v1.0.dmg`
2. **Double-click** the DMG to mount it
3. **Drag** WhisperApp into your **Applications** folder
4. **Launch** WhisperApp from Applications 🚀

### Option 2: ZIP Archive

1. **Download** `WhisperApp-Standalone-v1.0.zip`
2. **Unzip** the archive
3. **Drag** the app into your **Applications** folder
4. **Open** WhisperApp and you’re ready! 🎉

---

## ⚡ First Launch Details

On the first launch, WhisperApp will:

1. Prompt for **permission** (macOS security dialog)
2. **Download** the Whisper model (\~1.5 GB)
3. **Configure** necessary settings automatically
4. **Notify** when ready for use

Example download progress:

```
📥 Downloading Whisper model (first use)...
   This may take several minutes (~1.5 GB)...

██████████████████████ 100%

✅ Model downloaded successfully!
```

---

## ⚠️ macOS Permissions

### Possible alert on first run:

> "WhisperApp cannot be opened because the developer cannot be verified."

**Solutions:**

**Option 1: System Preferences**

1. Go to **System Settings** → **Privacy & Security**
2. Click **Open Anyway** next to WhisperApp

**Option 2: Terminal**

```bash
sudo xattr -rd com.apple.quarantine /Applications/WhisperApp.app
```

**Option 3: Right-click**

1. Right-click the app in **Applications**
2. Select **Open**
3. Confirm **Open** in the popup

---

## 📊 Standalone vs. Standard

| Feature                  | Standard Version | Standalone Version |
| ------------------------ | ---------------- | ------------------ |
| Initial Download Size    | 0.5 MB           | 1.5 MB             |
| Binary Installation      | Manual           | Automatic          |
| Model Download           | Manual           | Automatic          |
| Ready to Use Immediately | No               | Yes                |
| External Dependencies    | Yes              | No                 |

---

## 🔧 Technical Structure

```
WhisperApp.app/
├── Contents/
│   ├── MacOS/WhisperApp         # Main app executable
│   ├── bin/                     # Bundled binaries
│   │   ├── whisper-cli          # Whisper transcription engine
│   │   └── ffmpeg               # Audio/video converter
│   ├── models/                  # Downloads model files
│   │   └── ggml-medium.bin      # Whisper model (first launch)
│   └── Resources/
│       └── whispercpp_run.sh    # Smart wrapper script
```

### Startup sequence:

1. Check bundled binaries
2. Detect if model exists
3. Download model from Hugging Face if missing
4. Configure paths and permissions
5. Ready to transcribe

---

## 🎯 How to Use

1. **Open** WhisperApp
2. **Select** your audio/video file
3. **Choose** a language (English/French)
4. **Click** Transcribe
5. **Retrieve** your subtitles (.srt, .vtt) and transcript (.txt)

### Supported formats:

* **Video**: MP4, MOV, AVI, MKV, etc.
* **Audio**: MP3, WAV, M4A, FLAC, etc.

---

## 🚨 Troubleshooting

* **"Binary not found"**: Reinstall the app; it may be corrupted.
* **Model download failure**:

  * Check internet connection
  * Ensure 2 GB free disk space
  * Retry later
* **App slow or unresponsive**:

  * First-download in progress
  * Very large media file
  * Insufficient RAM

---

## 📞 Support

This standalone version is designed to work out-of-the-box on any modern Mac. If you encounter issues:

1. **Verify** macOS 14.0+
2. **Ensure** 2 GB available disk space
3. **Allow** the app in **Privacy & Security**
4. **Wait** for the first model download to complete

---

**Version**: Standalone 1.0
**Compatibility**: macOS 14.0+
**Architectures**: Universal (Intel + Apple Silicon)
**Size**: \~1.5 GB after download
