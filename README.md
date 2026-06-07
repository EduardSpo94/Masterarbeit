Development of a Conditional Latent Diffusion Model for the Synthesis of Machine Sound Anomalies

# Generative Anomaly Detection in Industrial Machinery

This repository contains the source code, Jupyter notebooks, and evaluation scripts developed 
for the Master's Thesis titled **Development of a Conditional Latent Diffusion Model for the Synthesis of Machine Sound Anomalies**.

## Abstract
This project investigates the use of Latent Diffusion Models (LDMs) to generate synthetic industrial sound anomalies. 
The generated data is used for "Outlier Exposure" to enhance the robustness of Anomaly Sound Detection (ASD) systems under domain shift conditions, specifically focusing on the MIMII-DG dataset.

## Project Structure
The repository is structured into modular components:

```text
/
├── notebooks/                    # Jupyter Notebooks for pipeline execution
│   ├── 00_data_prep.ipynb        # Data aggregation & EnCodec feature extraction
│   ├── 10_diffusion_train.ipynb  # Training the Conditional Latent Diffusion Model
│   ├── 11_sampling.ipynb         # Generation of synthetic anomalies
│   ├── 20_eval_gen.ipynb         # Audio quality evaluation (FAD, CLAP)
│   ├── 21_eval_asd_s1.ipynb      # Baseline evaluation (Autoencoder)
│   └── 22_eval_asd_s2.ipynb      # Evaluation of proposed OEC System
├── system_1_ae/                 # ASD System 1: Autoencoder (Baseline)
│  
│  
│
├── system_2_mobilenet/          # ASD System 2: MobileNetV2 (Proposed)
│   
│   
│
├── mimii_gen/                   # Generative model implementation
│   ├── unet.py                  # Wide-UNet architecture
│   └── inference.py             # Sampling & post-processing logic
│
└── README.md                    # Project documentation

