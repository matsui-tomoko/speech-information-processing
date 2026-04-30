# Speech Information Processing (PhD)

Shenzhen Loop Area Institute (SLAI)

---

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
- Phase B (Weeks 4–7): Classical → deep models and representation learning  
- Phase C (Weeks 8–10): Uncertainty, decision making, and generative modeling
- Phase D (Weeks 11–13): Explainability & statistical claimability  

- Weeks 14–17: Research design & project defense  

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

## Current Focus

### Week 5 — CTC-Based ASR

Topics:
- Connectionist Temporal Classification (CTC)  
- alignment without frame-level labels  
- independence assumption  
- decoding (collapse + blank removal)  

Notebook:
- `notebooks/SIP_Week5_Template.ipynb`

---

### Week 6 — Modern ASR and Attention

Topics:
- wav2vec 2.0 (pretrained encoder)  
- CTC decoding in real ASR systems  
- attention and multi-head attention  
- global vs local context  
- latency vs accuracy trade-off  

Notebook:
- `notebooks/SIP_Week6_Template.ipynb`

---

### Week 7 — Representation and Speaker Modeling

This week focuses on how speech signals are transformed into embedding representations, and how these representations encode speaker identity and enable similarity-based decisions.

Topics:
- representation learning \( z = f_\theta(x) \)  
- feature vs embedding  
- similarity and distance (Euclidean, cosine)  
- speaker embeddings (d-vector, x-vector, ECAPA)  
- embedding geometry (clustering, separability, invariance)  
- robustness and domain shift  

Notebook:
- `notebooks/SIP_Week7_Template.ipynb`

---

### Week 8 — Uncertainty and Decision Making

This week focuses on how prediction is connected to uncertainty and decision making, with a simple medical-audio example.

Topics:
- uncertainty estimation  
- decision under uncertainty  
- simple cough detection system  
- accept / refer decisions  

Notebook:
- `notebooks/SIP_Week8_Template.ipynb`


---

### Week 10 — Gaussian Processes and Structured Variation

This week introduces Gaussian Processes for modeling structured variation in speech information across time, speakers, and conditions.

Topics:
- Gaussian Processes (GP)  
- kernel design for structured variation  
- hierarchical modeling and decomposition  
- multi-output GP (correlated signals)  
- sparse GP (scalability)  

Notebook:
- `notebooks/SIP_Week10_Template.ipynb`

---


## Learning Flow

Week 4:
→ Classical ASR (HMM-based models)

Week 5:
→ CTC (alignment and decoding)

Week 6:
→ Modern ASR (wav2vec + CTC)  
→ Attention and context modeling  
→ Real-world constraints (latency)

Week 7:
→ Representation learning  
→ Speaker modeling (who is speaking)

Week 8:
→ Uncertainty and decision making  
→ When not to decide

Week 10:
→ Modeling structured variation  
→ Gaussian Processes (function-level modeling)  
→ From prediction to interpretation

---

## How to Run Notebooks

### 1. Install required packages (only if needed)

```bash
pip install torchaudio transformers matplotlib
