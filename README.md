<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=4,10,18&height=160&section=header&text=Advanced%20Image%20Generation&fontSize=36&fontColor=fff&animation=twinkling&fontAlignY=36&desc=ComfyUI%20Workflow%20%E2%80%94%20ControlNet%20%2B%20LoRA%20%2B%20Pose%20Transfer&descAlignY=58&descSize=14" width="100%"/>

[![ComfyUI](https://img.shields.io/badge/ComfyUI-Workflow-orange?style=for-the-badge)](https://github.com/comfyanonymous/ComfyUI)
[![ControlNet](https://img.shields.io/badge/ControlNet-Enabled-blue?style=for-the-badge)](https://github.com/lllyasviel/ControlNet)
[![SDXL](https://img.shields.io/badge/SDXL-Base-purple?style=for-the-badge)](https://stability.ai/)

**Pose-controlled portrait generation with ControlNet + 4x upscaling**

</div>

---

## 🎯 What It Does

A **ComfyUI workflow** that generates high-quality AI portraits using a reference photo + pose control image. Takes any person's photo and places them in a new scene with a custom pose — powered by ControlNet and SDXL.

---

## ✨ Workflow Features

| Feature | Description |
|---|---|
| 🎭 **ControlNet Pose** | Transfer exact pose from a control image to the output |
| 🖼️ **Image-to-Image** | Use a reference photo to preserve subject identity |
| 📐 **Canny Control** | Edge-based composition control for precise results |
| 🔍 **4x Upscaling** | SwinIR upscaling for high-resolution final output |
| ✍️ **Prompt Styling** | Text prompt drives scene, lighting, and style |

---

## 🏗 How It Works

```
Input: Reference photo + Pose control image
        ↓
ControlNet (Canny) — guides composition + pose
        ↓
SDXL generates base image with text prompt
        ↓
SwinIR 4x upscaler — enhances resolution
        ↓
Final high-quality portrait output
```

---

## 🛠 Models Used

| Model | Purpose |
|---|---|
| `diffusers_xl_canny_full_v10.safetensors` | ControlNet Canny for SDXL |
| `ControlNet-Canny.safetensors` | Edge-based pose control |
| `SwinIR_4x.safetensors` | 4x image upscaling |

---

## 🚀 Setup

1. Install [ComfyUI](https://github.com/comfyanonymous/ComfyUI)
2. Place model files in `ComfyUI/models/` directories
3. Load `final.json` workflow in ComfyUI
4. Connect your reference photo and pose image
5. Run the workflow

---

## 📬 Contact

**Built by [Vijay Krishna](https://github.com/Vijaykrishna2334)**
- 📧 vijaykrishna2334@gmail.com
- 💼 [LinkedIn](https://linkedin.com/in/vijaykrishna2334)

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=4,10,18&height=80&section=footer" width="100%"/>
