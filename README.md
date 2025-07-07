# 🎬 WhisperApp

**AI-powered video transcription made simple**

Transform your videos into accurate subtitles using OpenAI's Whisper technology. Drop your videos, choose your language, and get professional subtitles in seconds.

## ✨ Features

- 🎯 **Drag & Drop Interface** - Simply drop your video files
- 🚀 **Batch Processing** - Handle multiple videos at once
- 🌍 **Multi-language Support** - English and French transcription
- 📄 **Multiple Output Formats** - TXT, SRT, and VTT subtitles
- ⚡ **Real-time Progress** - See your transcription progress live
- 🔒 **100% Local Processing** - Your videos never leave your computer
- 📦 **Standalone App** - No additional software required

## 📋 System Requirements

- **macOS**: 14.0 or later
- **Processor**: Intel (x86_64) or Apple Silicon (M1/M2/M3)
- **RAM**: 4 GB minimum recommended
- **Storage**: 2 GB free space (for AI model)
- **Internet**: Required only for first-time model download

## 🚀 Quick Start

### Installation

1. **Download** the latest release
2. **Extract** the ZIP file or mount the DMG
3. **Move** WhisperApp to your Applications folder
4. **Right-click** → **Open** (first time only, due to macOS security)

### First Launch

The app will automatically download the Whisper AI model (~1.5 GB) on first use. This only happens once!

### Usage

1. **Launch** WhisperApp
2. **Drag & drop** your video files (MP4, MOV, AVI)
3. **Select language** (English or French)
4. **Click Start** and wait for processing
5. **Find your subtitles** next to the original video files

## 📁 Supported Formats

### Input Videos
- **MP4** (recommended)
- **MOV** (QuickTime)
- **AVI** (Audio Video Interleave)

### Output Subtitles
- **TXT** - Plain text transcription
- **SRT** - Standard subtitle format (VLC, Final Cut Pro, etc.)
- **VTT** - Web-compatible subtitles (HTML5 video)

## ⚠️ First Launch Security Notice

Since WhisperApp is distributed outside the Mac App Store, macOS will show a security warning:

### Option 1: Right-click Method
1. **Right-click** on WhisperApp
2. Select **"Open"**
3. Click **"Open"** in the security dialog

### Option 2: System Settings
1. Try to open WhisperApp normally
2. Go to **System Settings** → **Privacy & Security**
3. Click **"Open Anyway"** next to WhisperApp

## 🔧 Technical Details

### What's Included
- **FFmpeg** - High-performance audio/video processing
- **Whisper** - OpenAI's state-of-the-art speech recognition
- **All Dependencies** - No separate installations needed

### Processing Speed
- Approximately **10-15% of video duration**
- Example: 10-minute video ≈ 1-2 minutes processing time
- Varies based on audio complexity and system performance

### Privacy & Security
- **No data collection** - Everything runs locally
- **No internet required** after initial setup
- **Your content stays private** - Never uploaded anywhere
- **Apple code-signed** for security

## ❓ Troubleshooting

### "App is damaged" Error
```bash
# Run this in Terminal to fix quarantine issues:
sudo xattr -rd com.apple.quarantine /Applications/WhisperApp.app
```

### Model Download Fails
- Check your internet connection
- Restart the app to retry download
- Ensure you have 2GB+ free disk space

### Processing Fails
- Verify the video file plays correctly in other apps
- Check available disk space
- Try with a shorter video first

### App Won't Start
- Verify macOS 14.0+ requirement
- Try the right-click → Open method
- Check Console.app for detailed error messages

## 🆘 Support

Having issues? Here's how to get help:

1. **Check the troubleshooting section above**
2. **Try with a different video file**
3. **Restart the application**
4. **Open an issue on GitHub** with:
   - Your macOS version
   - Video file format/size
   - Error messages (if any)

## 📄 License & Credits

WhisperApp is built using:
- **OpenAI Whisper** - Speech recognition (MIT License)
- **FFmpeg** - Audio/video processing (LGPL License)

Created by **Luca Smith** • Distributed under MIT License

## 🔄 Changelog

### v1.0
- Initial release
- English and French transcription
- Batch processing support
- Multiple output formats
- Standalone distribution

---

**Made with ❤️ for content creators, educators, and accessibility advocates**

*Generate professional subtitles with the power of AI* 
