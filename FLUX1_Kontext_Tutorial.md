# FLUX.1 Kontext Master Tutorial – Local Install with One Click!

Get the best image editing experience powered by FLUX.1 Kontext!  
This tutorial provides everything you need to install and use **FLUX.1 Kontext** on your local machine.

FLUX.1 Kontext marks a significant expansion of classic text-to-image models by unifying **instant text-based image editing** and **text-to-image generation**.

As a **multimodal flow model**, it features:
- State-of-the-art **character consistency**
- Advanced **context understanding**
- Powerful **local editing capabilities**
- Strong **text-to-image synthesis**

---

🆕 **Updated: July 2025**  
📺 **Watch the Full Windows Tutorial**: [YouTube Tutorial](https://youtu.be/FRmJtRurOsA)  
👍 You won't regret it!

---

## 🔁 One-Click Local Install (Supporters Only)

I provide a **one-click installation script** exclusively for Patreon supporters:  
👉 [Patreon Installation Link](https://www.patreon.com/posts/open-source-flux-133086184)

Supporting me helps keep content like this alive — thank you!

---

## ⚙️ Manual Installation Guide

### 1. Download ComfyUI  
Get the base UI at: [https://github.com/comfyanonymous/ComfyUI](https://github.com/comfyanonymous/ComfyUI)

---

### 2. Install Custom Nodes
Clone the required custom nodes into your ComfyUI installation:

```bash
git clone https://github.com/ltdrdata/ComfyUI-Manager.git
git clone https://github.com/mit-han-lab/ComfyUI-nunchaku.git


3. Download FLUX.1 Kontext Models
Place the following files into the ComfyUI/models/ directory:

ComfyUI/models/unet/
  - svdq-int4_r32-flux.1-kontext-dev.safetensors

ComfyUI/models/clip/
  - t5xxl_fp8_e4m3fn_scaled.safetensors
  - clip_l.safetensors

ComfyUI/models/vae/
  - ae.safetensors

ComfyUI/models/loras/
  - flux-turbo-alpha.safetensors

4. Download Attachments
Make sure to download:

install_wheel.json

Flux Kontext.json
5. Setup in ComfyUI

Start ComfyUI.

Load install_wheel.json.

Choose the new version and Run.
6. Have Fun!
Load Flux Kontext.json to start using FLUX.1 Kontext with full features.

Explore editing, generating, and modifying your images like never before!
❤️ Support Me
Your support on Patreon keeps tutorials and tools like this coming!

Thank you 🙏


