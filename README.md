# Image Captioning with CLIP + GPT-2

**IE 7615 Deep Learning for AI — Generative Project**  
**Northeastern University | Group 9**

## Overview
An image captioning system that generates natural language descriptions from photographs by combining a frozen CLIP (ViT-B/32) vision encoder with a GPT-2 language decoder.

## Architecture
- **Image Encoder:** CLIP ViT-B/32 (frozen, 512-dim embeddings)
- **Language Decoder:** GPT-2 (124M params, 768-dim hidden)
- **Integration:** Prefix conditioning — CLIP embedding projected to GPT-2 hidden dim via learned linear layer

## Dataset
- **Primary:** COCO Captions (Karpathy split), 5K subset, 25K captions
- **Secondary:** VizWiz-Captions (accessibility-focused robustness evaluation)

## Project Milestones
| Milestone | Description | Status |
|-----------|-------------|--------|
| M1 | Dataset preprocessing, CLIP embeddings, GPT-2 tokenization | ✅ Complete |
| M2 | CLIP–GPT-2 integration, decoding strategies | ⬜ Upcoming |
| M3 | Evaluation metrics, fine-tuning comparisons, VizWiz evaluation | ⬜ Upcoming |
| M4 | Final report, presentation, demo | ⬜ Upcoming |

## Setup
```bash
pip install torch torchvision transformers datasets pillow matplotlib open-clip-torch pycocoevalcap
```

## Usage
Open `milestone1_image_captioning.ipynb` in Google Colab with GPU runtime and run all cells.

## Team
- Reshma Sri Gollapudi
- Atharva Yogesh Parulkar
