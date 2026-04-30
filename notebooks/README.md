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

---

## Week 4 — Classical ASR (GMM/HMM + Viterbi)

In this week, we study classical speech recognition based on probabilistic sequence models.

### Topics
- Hidden Markov Models (HMM)
- EM / Baum–Welch training
- Viterbi decoding
- Model selection (AIC/BIC)

### Exercise
We build a simple ASR system step by step:

1. Segment speech into word-level units (YESNO dataset)
2. Extract MFCC features
3. Train HMMs for each class (lo / ken)
4. Decode using Viterbi
5. Evaluate classification accuracy
6. Compare models using AIC / BIC

Notebook: `notebooks/SIP_Week4_Template.ipynb`

---

## Week 5 — CTC-Based ASR

Week 5 introduces Connectionist Temporal Classification (CTC) for sequence modeling.

### Topics
- CTC formulation
- alignment without frame-level labels
- independence assumption
- decoding (collapse + remove blanks)

### Exercise
We implement a simple CTC-based ASR system:

1. Load speech data (YESNO dataset)
2. Extract log-Mel features
3. Train a neural network with CTC loss
4. Decode predictions
5. Evaluate performance (WER / CER)

Notebook: `notebooks/SIP_Week5_Template.ipynb`

---

## Week 6 — Modern ASR and Attention

Week 6 connects CTC with modern deep learning-based ASR systems.

### Topics
- wav2vec 2.0 (pretrained encoder)
- CTC decoding in real ASR systems
- attention and multi-head attention
- global vs local context
- latency vs accuracy trade-off

### Exercise
We analyze real ASR behavior through experiments:

1. Run CTC-based ASR (wav2vec + CTC decoding)
2. Visualize attention weights from the model
3. Simulate latency by limiting future context
4. Perform final analysis of model behavior

### Notes
- No training is required
- All experiments run on CPU
- Data is downloaded automatically in the notebook
- Pip dependency warnings can be ignored if execution succeeds

Notebook: `notebooks/SIP_Week6_Template.ipynb`

---

## Learning Progression

Week 5:
→ Understand CTC (alignment and decoding)

Week 6:
→ Run real ASR systems  
→ Understand attention mechanisms  
→ Analyze real-world constraints (latency)

## Week 7: Representation and Speaker Modeling

Topics include:

- embedding representation \( z = f_\theta(x) \)
- similarity and distance (Euclidean, cosine)
- speaker embeddings (d-vector, x-vector, ECAPA)
- visualization (PCA, t-SNE)
- distance analysis and robustness

The notebook focuses on understanding embedding geometry through visualization and simple experiments.

## Week 8 — Uncertainty and Decision Making

Week 8 focuses on how to connect prediction, uncertainty, and decision making.

### Topics

- simple cough detection
- uncertainty estimation
- event-level aggregation
- decision making (accept / refer)

### Exercise

We implement a minimal system to illustrate:

prediction → uncertainty → decision

Notebook: `notebooks/SIP_Week8_Template.ipynb`

---

## Week 10 — Gaussian Processes and Structured Variation

Week 10 introduces Gaussian Processes for modeling structured variation in speech data.

### Topics

- Gaussian Processes (GP)
- kernel design
- hierarchical modeling
- multi-output GP
- sparse GP

### Exercise

We use synthetic data to:

- visualize different sources of variation
- decompose signals into components
- understand GP-based modeling and uncertainty

Notebook: `notebooks/SIP_Week10_Template.ipynb`

