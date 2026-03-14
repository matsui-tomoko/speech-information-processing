# Speech Information Processing (PhD)
 
Shenzhen Loop Area Institute (SLAI)

## Course Staff

Instructor:
- Prof. Tomoko Matsui

Co-Instructors:
- Prof. Zhaojie Luo (Weeks 11–13)
- Prof. Shuai Wang (Week 9)

Teaching Assistant:
- Wenpu Sun

---
## Course Phases

- Phase A (Weeks 1–3): Signal foundations
- Phase B (Weeks 4–6): Classical → deep models
- Phase C (Weeks 7–10): Bayesian modeling & speech drift
- Phase D (Weeks 11–13): Explainability & statistical claimability

- Weeks 14–17: Research design & project defense

Guest Lecturer:
- Week 9:  Prof. Shuai Wang

Second Lecturer:
- Weeks 11–13:  Prof. Zhaojie Luo

---

## Dataset Policy

Datasets such as LibriSpeech and VoxCeleb must be downloaded from official sources.  
Students are responsible for complying with dataset licenses.

This repository does **not** host copyrighted datasets.

---

## Reproducibility Policy

All experiments must:
- Log configuration settings
- Fix and record random seeds
- Report uncertainty (e.g., 95% confidence intervals)
- Include a decision table linking diagnostics to actions

---
## Teaching Data

Synthetic teaching data used for the hands-on experiments is available under:

`data/audio_samples.zip`

---

## Recent Updates

### Week 3 Materials

The Week 3 materials have been added to the repository.

Updates include:

- Updated teaching dataset  
  `data/audio_samples.zip` now includes **synthetic speech samples** generated for robustness experiments.

- Week 3 notebooks:

  - `notebooks/SIP_Week3_Synthetic_Data_Generation.ipynb`  
    Generates synthetic speech data used in the experiments.

  - `notebooks/SIP_Week3_Template.ipynb`  
    Main notebook for the Week 3 hands-on robustness experiments.

The Week 3 notebooks implement the following experiments:

1. Baseline feature extraction (clean speech)
2. Noise augmentation (different SNR levels)
3. Reverberation experiments (different RT60 values)
4. Combined noise + reverberation

These experiments analyze the **robustness of log-Mel and MFCC features under realistic acoustic distortions**.
