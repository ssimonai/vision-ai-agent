# Vision AI Agent
This repository contains code for a computer vision AI agent pipeline for non-contact material strain and property extraction from video data, demonstrated on video taken during hydrostatic testing of four OFHC copper cylinders conducted as part of the LEGEND-1000 hardware validation campaign.

See our paper on [arXiv](https://arxiv.org/abs/2606.18294).

## Installation

### Requirements
- FFmpeg (system dependency)
- Python 3.10+
- GPU with CUDA support recommended

### Setup
```bash
pip install -r requirements.txt
```

**Note:** SAM2 is installed from a specific commit (`2b90b9f`) to ensure reproducibility with the version used in this work. For more details on installing SAM2, please see the [SAM2 GitHub repository](https://github.com/facebookresearch/sam2).
