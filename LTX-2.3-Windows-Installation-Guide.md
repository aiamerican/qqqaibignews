# LTX 2.3 Windows Installation Guide - ComfyUI (Full Tutorial)

**LTX 2.3** is the latest powerful open-source AI video generation model from Lightricks. It supports **Text-to-Video**, **Image-to-Video**, and **Audio-to-Video** with native synchronized audio, sharper details, better motion control, and true native **9:16 portrait** output.

This guide provides a complete **manual installation** for **Windows** users using the portable ComfyUI version.

> **Full Video Tutorial**: [Watch the Windows LTX 2.3 Tutorial](https://youtu.be/FeAh8lD-IFo)

---

## Easy One-Click Installation (For Supporters)

I provide a **one-click .bat installer** for my Patreon supporters to simplify the entire process.

[Download One-Click LTX 2.3 Installer](https://www.patreon.com/posts/one-click-ltx-2-155349599)

---

## Manual Installation Steps (Windows Portable)

### Step 1: Download and Extract ComfyUI

1. Download the latest **ComfyUI_windows_portable** from the official repository.
2. Extract the zip file to a folder with sufficient free space (50-100GB recommended).

### Step 2: Place Model Files

Create the correct folder structure and place the following models:

**Model Paths:**

- `ComfyUI\models\text_encoders\`
  - `ltx-2.3_text_projection_bf16.safetensors`
  - `gemma_3_12B_it_fp4_mixed.safetensors`

- `ComfyUI\models\vae\`
  - `LTX23_audio_vae_bf16.safetensors`
  - `LTX23_video_vae_bf16.safetensors`

- `ComfyUI\models\unet\`
  - `ltx-2.3-22b-dev-Q6_K.gguf` (Recommended GGUF quantized version for lower VRAM)

- `ComfyUI\models\latent_upscale_models\`
  - `ltx-2.3-spatial-upscaler-x2-1.1.safetensors`

- `ComfyUI\models\loras\`
  - `ltx-2.3-22b-distilled-lora-384.safetensors`
  - `ltx-2-19b-ic-lora-detailer.safetensors`
  - `ltx-2.3-22b-ic-lora-union-control-ref0.5.safetensors`

**Important**: Add FFmpeg files (required for video generation):

Place these three files in the `ComfyUI_windows_portable\` root folder:
- `ffmpeg.exe`
- `ffplay.exe`
- `ffprobe.exe`

Without FFmpeg, video generation will fail.

### Step 3: Install Custom Nodes

1. Open Command Prompt (CMD) and navigate to the custom nodes folder:
   ```cmd
   cd ComfyUI\custom_nodes

2.Run the following git clone commands:

git clone https://github.com/ltdrdata/ComfyUI-Manager.git

git clone https://github.com/city96/ComfyUI-GGUF

git clone https://github.com/rgthree/rgthree-comfy

git clone https://github.com/yolain/ComfyUI-Easy-Use

git clone https://github.com/kijai/ComfyUI-KJNodes

git clone https://github.com/ClownsharkBatwing/RES4LYF

git clone https://github.com/Lightricks/ComfyUI-LTXVideo

git clone https://github.com/pythongosssss/ComfyUI-Custom-Scripts

git clone https://github.com/Kosinkadink/ComfyUI-VideoHelperSuite

git clone https://github.com/kijai/ComfyUI-WanVideoWrapper

git clone https://github.com/ltdrdata/ComfyUI-Impact-Pack

git clone https://github.com/TTPlanetPig/Comfyui_TTP_Toolset

git clone https://github.com/evanspearman/ComfyMath

git clone https://github.com/Fannovel16/comfyui_controlnet_aux.git

git clone https://github.com/akatz-ai/ComfyUI-DepthCrafter-Nodes.git

3.Install dependencies (run these commands from the ComfyUI root folder):

..\..\python_embeded\python.exe -m pip install -U pip

..\..\python_embeded\python.exe -m pip install -r custom_nodes\ComfyUI-Manager\requirements.txt

..\..\python_embeded\python.exe -m pip install -r custom_nodes\ComfyUI-GGUF\requirements.txt

..\..\python_embeded\python.exe -m pip install -r custom_nodes\rgthree-comfy\requirements.txt

..\..\python_embeded\python.exe -m pip install -r custom_nodes\ComfyUI-Easy-Use\requirements.txt

..\..\python_embeded\python.exe -m pip install -r custom_nodes\ComfyUI-KJNodes\requirements.txt

..\..\python_embeded\python.exe -m pip install -r custom_nodes\RES4LYF\requirements.txt

..\..\python_embeded\python.exe -m pip install -r custom_nodes\ComfyUI-LTXVideo\requirements.txt

..\..\python_embeded\python.exe -m pip install -r custom_nodes\ComfyUI-Custom-Scripts\requirements.txt

..\..\python_embeded\python.exe -m pip install -r custom_nodes\ComfyUI-VideoHelperSuite\requirements.txt

..\..\python_embeded\python.exe -m pip install -r custom_nodes\ComfyUI-WanVideoWrapper\requirements.txt

..\..\python_embeded\python.exe -m pip install -r custom_nodes\ComfyUI-Impact-Pack\requirements.txt

..\..\python_embeded\python.exe -m pip install -r custom_nodes\ComfyMath\requirements.txt

..\..\python_embeded\python.exe -m pip install -r custom_nodes\comfyui_controlnet_aux\requirements.txt

..\..\python_embeded\python.exe -m pip install -r custom_nodes\ComfyUI-DepthCrafter-Nodes\requirements.txt

Step 4: Launch ComfyUI and TestDouble-click run_nvidia_gpu.bat in the ComfyUI root folder to start.
Open your browser and go to http://127.0.0.1:8188
Download the recommended workflows:LTX 2.3 Image to Video.json
LTX-2.3-Video control+.json

Drag and drop the JSON files into ComfyUI and start generating!

Tips & TroubleshootingUse the GGUF quantized model for GPUs with 8-12GB VRAM.
Make sure your NVIDIA drivers and CUDA are up to date.
First launch and model loading may take several minutes.
If nodes are missing, use ComfyUI Manager to install or update them.

You can now generate high-quality LTX 2.3 videos with native audio completely locally and for free!

Keywords: LTX 2.3, LTX 2.3 Windows, LTX 2.3 ComfyUI, ComfyUI LTX 2.3 installation, LTXVideo, open source AI video model, local AI video generation, GGUF LTX 2.3, text to video, image to videoLast updated: April 2026






