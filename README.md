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

The AI agent pipeline is in `content/cv-pipeline-clean.ipynb` (note that an Anthropic API key is necessary for usage); code for performing the physics-based analysis of the extracted diameters can be found in `content/physics-analysis-clean.ipynb`. A pickle file with pressure and diameter data for both tests---for use in the analysis---is available in `content/AllHoustontestingdata_May2026_v20260506.pkl`.

**Note:** SAM2 can be installed from a specific commit (`2b90b9f`) to ensure reproducibility with the version used in this work. For more details on installing SAM2, please see the [SAM2 GitHub repository](https://github.com/facebookresearch/sam2).

**Note:** Due to the sizes of the original video files (~1GB each), 2.5min trimmed clips are available for use with the pipeline in `content/trimmed_vids`; note that these clips are each roughly 75MB. If interested in acquiring the original files, please reach out to Sonata Simonaitis-Boyd ([sonata@ucsd.edu](mailto:sonata@ucsd.edu)) or Alexander Leder ([aleder@lanl.gov](mailto:aleder@lanl.gov)).
