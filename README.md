
# Exploring Electroacoustic Music Analysis with Multimodal Large Language Models

This repository contains supplementary files and resources for my talk at the **Jahrestagung der Gesellschaft für Musikforschung**, 11–14 September 2024 in Köln. The materials are designed to provide a deeper understanding and hands-on examples related to the topics discussed during the presentation.

## Environment Setup

The code and notebooks in this repository are optimized for **Python 3.11**. We recommend setting up a virtual environment using Conda to manage the dependencies. You can create a new environment named `gfm_eallm` by running:

```bash
conda create -n gfm_eallm python=3.11
```

Once the environment is created and activated, install the required packages after cloning the repository using:

```bash
pip install -r requirements.txt
```

## Repository Structure

The repository contains the following files and directories:

### Slides:
- `ppt/ea_llm.pdf`: Presentation slides from the talk in PDF format.
- `ppt/ea_llm.pptx`: Presentation slides without audio in PowerPoint format.

### Audio Samples:
- `audio/bayle.wav`: François Bayle - *l'Aventure du cri* (1969), 2:10–2:20.
- `audio/bayle_whisper.wav`: Whisper encoding of `bayle.wav`.
- `audio/bayle2.wav`: François Bayle - *l'Aventure du cri* (1969), 0:22–0:32.
- `audio/bayle2_whisper.wav`: Whisper encoding of `bayle2.wav`.
- `audio/parm_de_nat1.wav`: Bernard Parmegiani - *De Natura Sonorum* - *incidences / battements* (1975), 0:00–0:10.
- `audio/parm_de_nat1_whisper.wav`: Whisper encoding of `parm_de_nat1.wav`.
- `audio/parm_de_nat1_clap.wav`: CLAP encoding of `parm_de_nat1.wav`.

### Notebooks:
- `clap_reconstruct.ipynb`: Visualization of MFCC filterbank used in CLAP (Elizalde et al., 2022). Python code for MFCC resynthesis using CLAP settings to demonstrate the quality loss during the encoding process.
- `whisper_reconstruct.ipynb`: Visualization of MFCC filterbank used in OpenAI Whisper (Radford et al., 2022). Python code for MFCC resynthesis using Whisper settings to show the quality loss during the encoding process.
- `whisper_hacks.ipynb`: Various interactions with OpenAI Whisper, including latent representation extractions. Visualizations of Whisper's latent space using t-SNE, PCA, and UMAP. Requires **CUDA GPU** to run!

## Getting Started

To get started, clone this repository and navigate to the cloned directory. Activate your `gfm_eallm` environment and install the required packages as described in the Environment Setup section above.

You can then open the notebooks using **Jupyter Notebook** or **JupyterLab** to follow along with the examples and explore the concepts discussed in the talk.
