# Index TTS2 WEBUI Installer for Windows

Index TTS2 is an advanced text-to-speech (TTS) tool with a web-based user interface, ideal for AI voice generation, synthesis, and experimentation.

The installation guide is based on the tutorial from [QQQ AI News on Patreon](https://www.patreon.com/posts/install-index-on-139848920). For full details and updates, check the original post.

## Features
- Easy one-click setup for Windows users.
- Supports TTS2 models for high-quality voice output.
- WebUI for intuitive control via browser.
- Compatible with Python environments and common dependencies.

## Prerequisites
Before running the installer, ensure you have:
- **Windows 10 or later** (64-bit recommended).
- **Python 3.10+** installed (download from [python.org](https://www.python.org/downloads/)).
- **Git** installed (download from [git-scm.com](https://git-scm.com/downloads)) for cloning repositories.
- At least **8 GB RAM** and **5 GB free disk space** for models and dependencies.
- NVIDIA GPU with CUDA support (optional, but recommended for faster inference).

## Installation Steps Video:
[Index TTS2 is out,local install in 1 click  open source text to speach with emotion](https://youtu.be/4ppdDmSYpms)

## Usage
- Upload text or audio files via the WEBUI.
- Select TTS models and generate speech.
- Export outputs in WAV/MP3 format.
- Customize parameters like voice, speed, and pitch.

Example command for manual run (after installation):
python app.py --model index-tts2 --port 7860


## Acknowledgments
- Original tutorial by [QQQ AI News](https://www.patreon.com/QQQAINews).
- Built on open-source TTS2 and Gradio libraries.

---
