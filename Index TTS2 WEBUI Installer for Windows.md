This repository provides a simple installer script (run.bat) to set up and run the Index TTS2 WEBUI on Windows systems. Index TTS2 is an advanced text-to-speech (TTS) tool with a web-based user interface, ideal for AI voice generation, synthesis, and experimentation.The installation guide is based on the tutorial from QQQ AI News on Patreon. For full details and updates, check the original post.FeaturesEasy one-click setup for Windows users.
Supports TTS2 models for high-quality voice output.
WebUI for intuitive control via browser.
Compatible with Python environments and common dependencies.

PrerequisitesBefore running the installer, ensure you have:Windows 10 or later (64-bit recommended).
Python 3.10+ installed (download from python.org).
Git installed (download from git-scm.com) for cloning repositories.
At least 8 GB RAM and 5 GB free disk space for models and dependencies.
NVIDIA GPU with CUDA support (optional, but recommended for faster inference).

Installation Steps

Clone this Repository:
Open Command Prompt or PowerShell and run:

git clone https://github.com/yourusername/index-tts2-webui-installer.git
cd index-tts2-webui-installer

Run the Installer:
Double-click run.bat or execute it from the command line:

run.bat

This script will:Check and install required Python packages (e.g., torch, transformers, gradio).
Download necessary TTS2 models.
Set up the WEBUI environment.
Launch the local server.

Access the WEBUI:
Once the server starts, open your browser and navigate to http://127.0.0.1:7860 (or the port shown in the console).
Troubleshooting:If you encounter CUDA errors, ensure your GPU drivers are up to date.
For CPU-only mode, edit run.bat to add --cpu flag.
Check the console output for detailed logs.

UsageUpload text or audio files via the WEBUI.
Select TTS models and generate speech.
Export outputs in WAV/MP3 format.
Customize parameters like voice, speed, and pitch.

Example command for manual run (after installation):

python app.py --model index-tts2 --port 7860


ContributingContributions are welcome! Fork the repo, make changes, and submit a pull request. For issues, open a ticket with logs.LicenseMIT License. See LICENSE for details.AcknowledgmentsOriginal tutorial by QQQ AI News.
Built on open-source TTS2 and Gradio libraries.



