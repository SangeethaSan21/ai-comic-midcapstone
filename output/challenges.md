# ⚡ Challenges Faced & Solutions

### 1. Character Consistency
- **Challenge:** Luna’s jacket and goggles were not always consistent across panels.
- **Solution:** Trained a custom LoRA with 30+ images to lock in Luna’s appearance, and refined prompts with style tokens.

### 2. Panel Layout in One Go
- **Challenge:** Most people created separate images and manually pasted them into comic panels.  
- **Solution:** I built a **single workflow** in ComfyUI using Flux + Image Batch + Image Grid to generate a full 6-panel page automatically.

### 3. Wide vs. Close Shots
- **Challenge:** Some outputs were zoomed in on Luna only, instead of wide cinematic panels.  
- **Solution:** Adjusted prompts with framing keywords like *“wide shot, cinematic view”* and added robot-cat + background elements.

### 4. Adding Speech Bubbles
- **Challenge:** Aligning speech bubbles and making them comic-style inside ComfyUI.  
- **Solution:** Used text overlay nodes and prompt styling (e.g., *“comic-style font, bold text, speech bubble pointing at Luna”*).

### 5. Flux Workflow Errors
- **Challenge:** First attempts at running all 6 panels in one go led to node errors.  
- **Solution:** Broke down workflow step-by-step, then reconnected prompts with 6 Clip nodes and 1 Image Grid Join node for final assembly.
