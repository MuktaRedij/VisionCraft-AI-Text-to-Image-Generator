# 📸⚡VisionCraft – AI Text-to-Image Generation System

VisionCraft is an AI-driven image generation system that transforms natural language prompts into high-quality images using Stable Diffusion.  
The project integrates **PyTorch**, **Hugging Face Diffusers**, and a **Gradio-based web interface**, enabling users to generate AI images without requiring programming experience.  
VisionCraft focuses on accessibility, customization, responsible AI usage, and hands-on experience with modern generative AI systems.

---

## 📌 Project Overview

VisionCraft demonstrates the use of open-source diffusion-based models for generative AI image synthesis.  
Users can generate visual content by entering text prompts and selecting image styles such as Photorealistic, Artistic, or Cartoon.

The project is designed for:
- Generative AI learning
- Model inference experimentation
- Prompt engineering practice
- Research and portfolio use

---
## 🏗️ Architecture

VisionCraft follows a modular pipeline architecture that processes the user input, generates an AI-based image using Stable Diffusion, enhances output quality, and returns the result through a graphical interface.  
Each stage of the workflow plays a specific role in transforming natural language into a visual output.
---

### System Architecture Flow
User Prompt → Prompt Enhancer → Stable Diffusion Model → Post-Processing (Watermark + Metadata) → Gradio UI → Output & Storage

### Component Breakdown

| Component | Description |
|----------|-------------|
| **User Interface (Gradio)** | Allows users to input prompts, select style, adjust settings, and view generated images. |
| **Prompt Enhancer Module** | Automatically adds descriptive keywords based on selected style to improve prompt clarity and output quality. |
| **Stable Diffusion Engine** | Core neural model responsible for generating images from text using latent diffusion. |
| **Inference Controller** | Manages guidance scale, inference steps, negative prompts, random seed, and device selection (CPU/GPU). |
| **Post-Processing Layer** | Applies watermark for ethical use and formats output into final image form. |
| **Metadata Logger** | Stores prompt details, generation settings, timestamps, and hardware configuration. |
| **Storage System** | Saves generated images and associated metadata into organized folders. |

---

### Architectural Characteristics

- **Modular Design:** Each processing block is independent and reusable.  
- **Hardware Adaptive:** Automatically detects and switches between CPU and GPU.  
- **Open-Source Dependency:** Built entirely using open-source framework components.  
- **Extensible Pipeline:** Future model versions (SDXL, DreamShaper) can be integrated with minimal modification.  

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

## 🛠️ Technology Stack

| Category | Details |
|----------|----------|
| Model | Stable Diffusion v1.5 |
| Frameworks | PyTorch, Hugging Face Diffusers |
| UI | Gradio |
| Image Processing | Pillow |
| Environment | Google Colab / Local Python |

---
## 🧩 Hardware Requirements

| Hardware Type | Recommended | Notes |
|---------------|-------------|-------|
| CPU | ✔ Supported | Slower generation (10–25s/image) |
| GPU (CUDA) | ✔✔ Recommended | Best performance (2–6s/image) |
| Apple Silicon (M-Series) | ✔ Partial Support | Requires PyTorch MPS |

---
##  ⚙️🔍Model Information

VisionCraft uses a pretrained Stable Diffusion model.

- **Model Name:** `runwayml/stable-diffusion-v1-5`
- **Architecture:** Latent diffusion text-to-image model
- **Source:** Hugging Face Model Hub

---

## 🧩 Hardware Requirements

| Hardware Type | Recommended | Notes |
|---------------|-------------|-------|
| CPU | ✔ Supported | Slower generation (10–25s/image) |
| GPU (CUDA) | ✔✔ Recommended | Best performance (2–6s/image) |
| Apple Silicon (M-Series) | ✔ Partial Support | Requires PyTorch MPS |

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
##  🛠️🔄System Workflow

1. User enters a text prompt.
2. System enhances prompt with selected style modifiers.
3. Model generates image using Stable Diffusion.
4. Negative prompt removes distortions and unwanted elements.
5. Watermark is added for responsible AI usage.
6. Final image is displayed and saved automatically.

---
## 🧠 Prompt Engineering Best Practices

| Tip | Example |
|------|---------|
| Specify style | “oil painting”, “photorealistic”, “anime style” |
| Add detail descriptors | “high resolution”, “sharp lighting”, “4k texture” |
| Use negative prompts | “low quality”, “distorted”, “extra limbs”, “blur” |
| Use subject + context | “A medieval castle on floating rocks during sunset” |
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
## ⚠️ Limitations

While VisionCraft provides high-quality image generation, the system has some known limitations:

- **Generation Time on CPU:**  
  Running on CPU mode can be significantly slower compared to GPU acceleration.

- **Image Accuracy Depends on Prompt Quality:**  
  Vague or unclear prompts may produce unexpected or inconsistent results.

- **Resolution Restrictions:**  
  Default Stable Diffusion model generates images at 512×512 resolution unless modified or upscaled.

- **Limited Realism for Complex Requests:**  
  Some outputs (e.g., text in images, human hands, or precise details) may not be perfectly accurate depending on prompt structure.

- **Watermark Placement is Fixed:**  
  The watermark is included for responsible use and currently cannot be repositioned or customized through UI.

- **Model Bias:**  
  Like most AI models, Stable Diffusion may reflect biases present in its training dataset, especially in cultural, gender, and contextual outputs.


---
## 🔮⚙️Future Enhancements

- Integration with SDXL and DreamShaper models
- Image upscaling and super-resolution enhancement
- User-selectable watermark options
- Multi-image gallery and batch generation
- Fine-tuning support for custom datasets
---
## 🪪License
This project is licensed under the **MIT License** — see the [LICENSE](./LICENSE) file for details.
---
## 👤 Author
**Mukta Redij**  
B.Tech (Information Technology) | AI & ML Enthusiast
