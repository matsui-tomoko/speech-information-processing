# Notebooks

This folder contains Jupyter notebooks used in the weekly hands-on exercises.

---

## Week 2 — Feature Extraction

Week 2 focuses on spectral feature extraction and validation.

Topics include:

- log-Mel spectrograms
- MFCC features
- reconstruction metric $\rho(D)$
- decorrelation metrics $\phi_L$, $\phi_c$, and $\Delta \phi$
- statistical comparison
- mini sensitivity experiment

### How to run

Step 1  
Run

notebooks/SIP_Week2_Data_Download.ipynb

to download a small dataset.

Step 2  
Run

notebooks/SIP_Week2_Template.ipynb

to perform Tasks A–D.

---

## Week 3 — Feature Robustness

Week 3 investigates how speech features behave under realistic acoustic distortions.

Experiments include:

- baseline feature extraction
- noise augmentation (different SNR levels)
- reverberation experiments (different RT60 values)
- combined noise + reverberation

### Notebooks

- `notebooks/SIP_Week3_Synthetic_Data_Generation.ipynb`  
  Generates synthetic speech samples used in the experiments.

- `notebooks/SIP_Week3_Template.ipynb`  
  Main notebook for the Week 3 robustness experiments.

### Data

Synthetic teaching data is provided in:

`data/audio_samples.zip`