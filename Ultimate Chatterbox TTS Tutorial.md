# Chatterbox Master Tutorial - Install Chatterbox WEBUI with One Click! Get the Best Open-Source TTS Model for Text-to-Speech!

Updated: June 2025

In this tutorial, I’ll guide you through installing the **Chatterbox** clone on your computer, bringing you the ultimate AI voice tool for memes, videos, games, or AI agents. Chatterbox is the first open-source text-to-speech (TTS) model with **emotion exaggeration control**, perfect for creating unique and expressive voices that breathe life into your projects.

## Why Choose Chatterbox?
No matter your goals, Chatterbox delivers top-tier AI voice capabilities. Its standout feature—emotion exaggeration control—sets it apart, making it ideal for creative projects requiring distinctive voice outputs.

## Windows Tutorial
Watch the full Windows installation tutorial here: [YouTube Tutorial](https://youtu.be/WZXLXzfupqs). Trust me, you won’t regret it—it’s awesome!

## One-Click Installation
For those who support me on Patreon, I provide a **local one-click installation script** to make setup a breeze. Check it out here: [Patreon Post](https://www.patreon.com/posts/open-source-text-130838188).

## Manual Installation
Follow these steps to manually install Chatterbox and set up the WEBUI:

1. **Create a Project Folder**
   - Create a folder named `chatterbox_env`.

2. **Set Up a Virtual Environment**
   - Open a Command Prompt (CMD) in the `chatterbox_env` folder and run the following commands:
     ```bash
     python -m venv venv
     call venv\Scripts\activate.bat
     python -m pip install --upgrade pip
     ```

3. **Install Chatterbox and Dependencies**
   - Install Chatterbox, Gradio, and required libraries:
     ```bash
     pip install chatterbox-tts gradio torchaudio
     ```

4. **Set Up the Gradio WEBUI**
   - Create a file named `gradio_app.py` in an `examples` folder within `chatterbox_env`. Add the following code to `gradio_app.py`:
     ```python
     from chatterbox.tts import ChatterboxTTS
     import gradio as gr
     import torch

     model = ChatterboxTTS.from_pretrained(device="cuda" if torch.cuda.is_available() else "cpu")

     def generate_audio(text):
         audio = model.generate(text)
         return (model.sr, audio.numpy())

     iface = gr.Interface(fn=generate_audio, inputs="text", outputs="audio")
     iface.launch()
     ```

5. **Launch Chatterbox TTS**
   - Navigate to the `examples` folder in CMD and run:
     ```bash
     python gradio_app.py
     ```

## Support the Project
Thank you for your support! By joining me on [Patreon](https://www.patreon.com/posts/open-source-text-130838188), you help me continue creating helpful content like this for everyone. Your support makes a huge difference!

Happy voice crafting with Chatterbox!