# LTX 2.0 ComfyUI Installation Guide (Windows)

This document provides a complete Windows installation tutorial for LTX 2.0 using ComfyUI, including video guidance, manual setup steps, required models, and runtime environment notes.

---

## Windows Video Tutorial

A full step-by-step Windows tutorial has been published on YouTube:

https://youtu.be/fbCddtkQ-Rc

This tutorial covers:
- Installing ComfyUI on Windows
- Setting up required custom nodes
- Downloading and placing LTX 2.0 models
- Running LTX 2.0 with an NVIDIA GPU

---

## One-Click Installation (Members Only)

For users who support me on Patreon, I provide a local one-click ComfyUI + LTX 2.0 zip package.

https://www.patreon.com/posts/ltx-2-0-comfy-ui-148916347

---

## Manual Installation Guide

### Step 1: Download ComfyUI

1. Download ComfyUI Windows Portable
2. Unzip it to your preferred directory

---

### Step 2: Install Required Custom Nodes

Navigate to:

ComfyUI_windows_portable/ComfyUI/custom_nodes

Then run:

git clone https://github.com/ltdrdata/ComfyUI-Manager.git

git clone https://github.com/city96/ComfyUI-GGUF.git

git clone https://github.com/rgthree/rgthree-comfy.git

git clone https://github.com/yolain/ComfyUI-Easy-Use.git

git clone https://github.com/kijai/ComfyUI-KJNodes.git

git clone https://github.com/Lightricks/ComfyUI-LTXVideo.git

---

### Step 3: Download LTX 2.0 Models

Place all models into:

ComfyUI_windows_portable/ComfyUI/models

checkpoints:
- LTX2_audio_vae_bf16.safetensors

text_encoders:
- ltx-2-19b-embeddings_connector_dev_bf16.safetensors
- gemma-3-12b-it-IQ4_XS.gguf

vae:
- LTX2_video_vae_bf16.safetensors

unet:
- ltx-2-19b-dev-Q4_K_S.gguf

latent_upscale_models:
- ltx-2-spatial-upscaler-x2-1.0.safetensors

diffusion_models:
- MelBandRoformer_fp32.safetensors

loras:
- ltx-2-19b-distilled-lora-384.safetensors
- ltx-2-19b-ic-lora-detailer.safetensors

---

### Step 4: Run ComfyUI

Double-click:

run_nvidia_gpu.bat

LTX 2.0 installation is now complete.

---

## Workflow

Download the provided workflow attachment and import it into ComfyUI to start Text-to-Video generation.

---

## System Requirements

- NVIDIA GPU required
- CUDA Runtime: 12.8
- Recommended RAM: 64GB or more
- If RAM is below 64GB, configure Windows Virtual Memory

---

## Required Dependencies

NVIDIA GPU driver (latest version recommended)

Visual C++ Redistributable:
https://aka.ms/vc14/vc_redist.x64.exe

---

## SEO Keywords

LTX 2.0, ComfyUI, LTX Video, Text to Video AI, ComfyUI Windows, NVIDIA CUDA 12.8, AI Video Generation, Local AI Video Model
