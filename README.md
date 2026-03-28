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
- Phase B (Weeks 4–6): Classical → deep models  
- Phase C (Weeks 7–10): Representation learning & speaker modeling  
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

## Learning Flow

Week 4:
→ Classical ASR (HMM-based models)

Week 5:
→ CTC (alignment and decoding)

Week 6:
→ Modern ASR (wav2vec + CTC)  
→ Attention and context modeling  
→ Real-world constraints (latency)

---

## How to Run Notebooks

### 1. Install required packages (only if needed)

```bash
pip install torchaudio transformers matplotlib
