# 📝 LoRA Training Notes

## Dataset
- Total images: 30 (sci-fi lab, jacket, goggles, orb scenes)
- Image resolution: 512x512
- Augmentation: Random crop, flip

## Model
- Base Model: Flux
- Training Type: LoRA fine-tuning
- Style: 3D stylized + cel shading
- Character: Luna (yellow jacket, goggles, space explorer look)

## Training Settings
- Epochs: 10
- Batch size: 2
- Learning rate: 1e-4
- Rank: 16

## Hardware
- GPU: A100 (Google Colab Pro)
- Training time: ~2.5 hours

## Output
- Final LoRA: `lunaGirl_flux_lora.safetensors`
- Usage: Loaded on top of Flux model in ComfyUI workflow
- Result: Consistent Luna character across 6-panel comic
