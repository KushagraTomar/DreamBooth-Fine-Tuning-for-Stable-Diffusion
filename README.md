# 🚀 DreamBooth Fine-Tuning for Stable Diffusion

Fine-tune [Stable Diffusion](https://github.com/CompVis/stable-diffusion) with **DreamBooth** to teach the model new, unique visual concepts using just a few images. This project shows how to build a fully custom pipeline for personalized text-to-image generation.

---

## 📌 What is DreamBooth?

DreamBooth is a fine-tuning technique that enables Stable Diffusion to learn a new concept (like a person, pet, or object) with just 10–20 images.  
It injects a **unique identifier** (like `ccorgi`) into text prompts, so the model generates the subject in new contexts without overwriting its general knowledge.

---

## ✨ Key Features

- ✅ **Custom Concept Learning:** Add your own pet, object, or style with minimal data.
- ⚙️ **Memory-Efficient Training:** Uses gradient checkpointing and 8-bit Adam optimizer for low-VRAM setups.
- ⚡ **Distributed Training:** Scales with [Hugging Face Accelerate](https://huggingface.co/docs/accelerate/index) for multi-GPU support.
- 🖼️ **Reusable Pipeline:** Save and share your fine-tuned model for interactive prompt-based generation.
- 🎛️ **Adjustable Guidance:** Control how closely outputs follow your text prompt using classifier-free guidance.

---

## 🧩 Tech Stack

- Python, PyTorch
- [Hugging Face Diffusers](https://github.com/huggingface/diffusers)
- Hugging Face Datasets, Transformers
- bitsandbytes (8-bit Adam)
- Accelerate
- CLIP Tokenizer, OpenCV, torchvision

---

## 📊 Results

- **Model:** Stable Diffusion v1.4  
- **Training Time:** ~400 steps, 1 GPU (adjustable)  
- **Output:** High-quality custom images faithful to the prompt  
- **Optimizations:** Gradient checkpointing, 8-bit Adam, Accelerate for distributed training  

---

## 📚 References

- [DreamBooth Paper](https://dreambooth.github.io/)
- [Hugging Face Diffusers](https://github.com/huggingface/diffusers)
- [Stable Diffusion](https://github.com/CompVis/stable-diffusion)
- [bitsandbytes](https://github.com/TimDettmers/bitsandbytes)
