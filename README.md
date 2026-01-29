# Capstone Project: Generative AI Media Cover Reimagining

## Project Objective
The goal of this project was to take three iconic pieces of media—an audio album, a book, and a movie—and use a self-hosted Generative AI pipeline to create alternative cover variations.

---

## 1. Audio Album: Pink Floyd - *Atom Heart Mother*
*   **Original Work:** ![Atom Heart Mother](https://github.com/user-attachments/assets/a9927172-c325-4038-bd64-aca0cb8942f1)

*   **AI-Generated Variation:** <img width="1024" height="1024" alt="Atom Heart Mother" src="https://github.com/user-attachments/assets/a90a2dd4-b66a-4b5c-b768-8dec83c63db9" />

*   **Concept:** Reimagining the iconic cow pasture with a surreal, high-fidelity modern aesthetic.

## 2. Book Cover: *Journey* (by various/generic selection)
*   **Original Work:** ![Journey](https://github.com/user-attachments/assets/d41852f8-bbb8-4f0f-9b7d-c87c14f2ffe4)

*   **AI-Generated Variation:** <img width="1024" height="1024" alt="Journey" src="https://github.com/user-attachments/assets/9169dd4b-cfa0-4dae-b356-b3ba18d90837" />

*   **Concept:** Transforming the classic adventure theme into a cinematic, atmospheric landscape.

## 3. Movie Box: *Pulp Fiction*
*   **Original Work:** ![Pulp Fiction](https://github.com/user-attachments/assets/11dd2b33-db9e-4cc8-afb6-8b90b171848a)

*   **AI-Generated Variation:** <img width="1676" height="2034" alt="Ready PULP FICTION" src="https://github.com/user-attachments/assets/9793711e-c4de-4adc-8ac4-cbf4f9364910" />

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

<img width="1510" height="848" alt="Screenshot 2026-01-30 at 02 34 02" src="https://github.com/user-attachments/assets/fcc31226-b88d-47e3-99a5-89ed80e82f1b" />

<img width="1512" height="837" alt="Screenshot 2026-01-30 at 02 39 33" src="https://github.com/user-attachments/assets/1a7001eb-0d15-4a96-932f-145cf65dd916" />


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
