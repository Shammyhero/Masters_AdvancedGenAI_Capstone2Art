# Capstone Project: Generative AI Media Cover Reimagining

## Project Objective
The goal of this project was to take three iconic pieces of media—an audio album, a book, and a movie—and use a self-hosted Generative AI pipeline to create alternative cover variations.

---

## 1. Audio Album: Pink Floyd - *Atom Heart Mother*
*   **Original Work:** [Insert Original Image Here]
*   **AI-Generated Variation:** [Insert Generated Image Here]
*   **Concept:** Reimagining the iconic cow pasture with a surreal, high-fidelity modern aesthetic.

## 2. Book Cover: *Journey* (by various/generic selection)
*   **Original Work:** [Insert Original Image Here]
*   **AI-Generated Variation:** [Insert Generated Image Here]
*   **Concept:** Transforming the classic adventure theme into a cinematic, atmospheric landscape.

## 3. Movie Box: *Pulp Fiction*
*   **Original Work:** [Insert Original Image Here]
*   **AI-Generated Variation:** [Insert Generated Image Here]
*   **Concept:** A "Medieval Fantasy" reimagining, turning the characters into knights in a tavern.

---

## Technical Workflow & Resources

### Hardware & Environment
*   **Hardware:** MacBook Pro M4 Pro (24GB Unified Memory)
*   **Environment:** Local self-hosted installation (no external APIs used)
*   **WebUI:** ComfyUI (Node-based interface)

### Generation Model
*   **Model Name:** RealVisXL V4.0 Lightning
*   **Version:** SDXL-Lightning
*   **Link:** [Hugging Face - RealVisXL V4.0 Lightning](https://huggingface.co/SG161222/RealVisXL_V4.0_Lightning)
*   **Adapters/LoRAs:** None (Native Lightning Checkpoint)

### Technical Generation Details
*   **Sampler:** `dpmpp_sde`
*   **Scheduler:** `karras`
*   **Steps:** 6 - 8 steps (optimized for Lightning model)
*   **CFG Scale:** 1.5
*   **Denoise (for Img2Img):** 0.65
*   **Resolution:** 1024 x 1024

### Pipeline Screenshot
[Insert Screenshot of ComfyUI Workflow Here]

---

## Prompts Used

### Audio (Atom Heart Mother)
*   **Positive:** `(masterpiece), high fidelity photography of a single cow in a lush green pasture, surreal blue sky, cinematic lighting, sharp focus, 8k resolution`
*   **Negative:** `text, logo, blurry, low quality, distorted anatomy`

### Book (Journey)
*   **Positive:** `epic book cover illustration, a lone traveler walking toward a massive ancient temple in a desert, dramatic sunset, cinematic atmosphere, intricate details`
*   **Negative:** `text, title, author name, blurry, simple, low res`

### Video (Pulp Fiction)
*   **Positive:** `medieval oil painting, two knights in silver armor sitting at a wooden table in a dark tavern, candlelight, dramatic shadows, renaissance style, highly detailed`
*   **Negative:** `guns, suits, modern clothing, sunglasses, digital art, text, blurry`
