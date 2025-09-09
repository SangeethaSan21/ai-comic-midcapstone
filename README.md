# 🎨 AI-Enhanced Comic Creation (Mid-Capstone Project)

## 📌 Overview  
This project was completed as part of my **Mid-Capstone assignment**.  
The objective was to design and generate a **6-panel comic page** using AI tools, with a **consistent 3D character style** and a clear storytelling flow.  

I chose to work with **Flux in ComfyUI** because of its strong 3D stylization and cinematic rendering ability.  
Final Grade: **19/20** ✅  

---

## 🎯 Goals  
- Build a **consistent AI character** (*Luna*, a curious space explorer).  
- Create a **6-panel comic page** showing a mini sci-fi story.  
- Ensure character consistency across all panels (expressions, outfit, style).  
- Automate the process using a **single ComfyUI workflow** (instead of manual editing).  
- Add **speech bubbles and dialogues** for authentic comic feel.  

---

## 🛠️ Tools & Technologies  
- **Model**: Flux  
- **LoRA Training**: Custom-trained on 30 images of Luna  
- **Workflow Engine**: ComfyUI  
- **Nodes Used**:  
  - CLIP Text Encode (for prompts)  
  - Flux LoRA Loader  
  - KSampler (image generation)  
  - VAE Decode (latent → image)  
  - Image Batch + Image Grid (for 6-panel layout)  
  - Text Overlay / Speech Bubble nodes (for dialogues)  
  - Latent Upscale (for final quality)  

---

## 📖 Storyline (Comic Panels)  
1. **Panel 1** – Luna tinkers in her sci-fi lab with her robot-cat and a mysterious glowing orb.  
2. **Panel 2** – She adjusts her goggles, surprised as the orb reacts.  
3. **Panel 3** – The orb begins to glow intensely, filling the lab with light.  
4. **Panel 4** – Luna releases the orb, which transforms into a holographic star map.  
5. **Panel 5** – She reaches for the map with determination, studying its path.  
6. **Panel 6** – Final cinematic shot: Luna ready to embark on her cosmic journey.  

---

## ⚡ Challenges & Solutions  
- **Character Consistency**  
  - Issue: Luna’s outfit (jacket) sometimes changed.  
  - Solution: Trained LoRA with more outfit-focused images + prompt reinforcement (`bright yellow space-jacket`).  

- **Wide vs Close-up Shots**  
  - Issue: Some outputs were too zoomed-in.  
  - Solution: Used prompts like `wide cinematic shot`, `sci-fi chamber`, `cinematic perspective`.  

- **Automation vs Manual Work**  
  - Issue: Many workflows required manual pasting.  
  - Solution: Built a **single automated workflow** using Image Batch + Image Grid to generate the final comic page in one go.  

---

## ✅ Results  
- A **6-panel AI-generated comic page** with consistent character styling.  
- Fully automated **end-to-end workflow** in ComfyUI.  
- Achieved **19/20 grade** 🎉  


---

## 💡 Key Learnings  
- The importance of **LoRA training** for consistency in multi-panel storytelling.  
- How **prompt engineering** controls framing and cinematic style.  
- Using **workflow automation** to save time and avoid manual assembly.  
- Balancing **technical problem-solving with creative storytelling**.  

---

## 🚀 Next Steps  
- Experiment with **ControlNet / IPAdapter** for stronger outfit consistency.  
- Expand into a **multi-page comic** project.  
- Explore animation workflows for turning panels into short AI-animated clips.  

---



