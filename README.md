# 📸⚡VisionCraft – AI Text-to-Image Generation System

VisionCraft is an AI-driven image generation system that transforms natural language prompts into high-quality images using Stable Diffusion.  
The project integrates **PyTorch**, **Hugging Face Diffusers**, and a **Gradio-based web interface**, enabling users to generate AI images without requiring programming experience.  
VisionCraft focuses on accessibility, customization, responsible AI usage, and hands-on experience with modern generative AI systems.

---

## ✨Features

 1. 🖼️**Text-to-Image Conversion**  
  Generates images from natural language prompts.

 2. 🎨**Multiple Styles Supported**  
  - 📸Photorealistic  
  - 🖌️Artistic  
  - 🤡Cartoon

 3.  ⚙️**Adjustable Model Parameters**  
  - 🎚️Guidance scale  
  - 🔁Inference steps  
  - 🚫Negative prompts

 4. 🚀**Prompt Enhancement**  
  Improves prompt quality automatically for better results.

 5. 🔏**Ethical Watermarking**  
  Each generated image includes a small “AI Generated” stamp.

 6.  💾**Automatic Saving With Metadata**  
  Includes prompt text, timestamp, device type, and model version.

 7. 💻⚡**Hardware Flexibility**  
  Works on both CPU and GPU environments (GPU recommended).

 8. 🧡**Fully Open-Source**  
  No paid APIs or proprietary tools required.

---

## 🛠️💻 Technology Stack

| Component | Technology |
|----------|------------|
| Model | Stable Diffusion v1.5 |
| Core Frameworks | PyTorch, Hugging Face Diffusers |
| Interface | Gradio |
| Image Processing | Pillow (PIL) |
| Runtime Environment | Google Colab or local Python environment |

---

##  ⚙️🔍Model Information

VisionCraft uses a pretrained Stable Diffusion model.

- **Model Name:** `runwayml/stable-diffusion-v1-5`
- **Architecture:** Latent diffusion text-to-image model
- **Source:** Hugging Face Model Hub

---

##  🛠️🔄System Workflow

1. User enters a text prompt.
2. System enhances prompt with selected style modifiers.
3. Model generates image using Stable Diffusion.
4. Negative prompt removes distortions and unwanted elements.
5. Watermark is added for responsible AI usage.
6. Final image is displayed and saved automatically.

---

##  🛠️📥Installation & Execution

### 🎯☁️Option A — Google Colab (Recommended)
- Upload the `.ipynb` notebook  
- Run all cells  
- The Gradio interface launches automatically  

### 🧰💻Option B — Local Setup

```bash
git clone https://github.com/<USERNAME>/VisionCraft.git
cd VisionCraft
pip install -r requirements.txt
python run.py   # if applicable
```
---
## 🎨💡Example Prompts
- A futuristic floating castle above clouds, ultra realistic, cinematic lighting
- A baby dragon holding a lantern, watercolor illustration
- A cyberpunk skyline with neon reflections, concept art style

---
## ⚡📈 Performance Notes
| Hardware | Expected Speed |
|----------|------------|
| CPU only | 10–25 seconds per image |
| GPU (T4 / RTX) | 2–6 seconds per image |
| Apple Silicon | Moderate performance depending on configuration |

---
## 🛡️🤝Ethical Use Guidelines

- Avoid generating harmful or misleading content.
- Do not remove the watermark unless for research purposes.
- Avoid using prompts related to real individuals without permission.

---
## 🔮⚙️Future Enhancements

- Support for additional SD model variants (SDXL, DreamShaper)
- Image upscaling and refinement tools
- Public web deployment (Hugging Face Spaces)
- Gallery display for multi-image output
- Custom dataset fine-tuning support
---
## 🪪License
This project is licensed under the **MIT License** — see the [LICENSE](./LICENSE) file for details.
---
## 👤 Author
**Mukta Redij**  
B.Tech (Information Technology) | AI & ML Enthusiast
