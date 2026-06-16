# Distributed Authorial Resistance (DAR)
### Neural Correlates of Critical Engagement vs. Fatigue in Human-AI Collaborative Writing

This repository contains the official EEG dataset processing scripts and visualization tools for the study on **Distributed Authorial Resistance (DAR)**. Our research investigates the N400 and P300 ERP components as markers of active human resistance against algorithmic homogenization, as opposed to mental fatigue.

---

## 🖼️ Graphical Abstract
<p align="center">
  <img src="figures/graphical_abstract.png" width="850" alt="DAR vs Fatigue Framework">
</p>

> **Key Hypothesis:** While mental fatigue attenuates neural responses, DAR manifests as a selective enhancement of the N400 (epistemic monitoring) and preserved P300 (authorial agency), indicating a "fight" rather than "flight" response to AI-generated text.

---

## 📊 Key Experimental Results

### 1. Neural Markers of Epistemic Monitoring (N400)
The DAR group shows a significant increase in N400 amplitude when encountering stylistic incongruities in AI text, reflecting active critical engagement.
<p align="center">
  <img src="figures/figure_1_simulated_erp_n400.png" width="800">
</p>

### 2. Cognitive Engagement Index (Theta/Alpha Ratio)
Increased Frontal Theta/Alpha ratio in the DAR condition confirms that the observed neural activity is due to high executive control and task engagement, not fatigue.
<p align="center">
  <img src="figures/figure_4_theta_alpha_ratio.png" width="700">
</p>

### 3. Statistical Analysis of ERP Dynamics
Summary of amplitude and latency differences across conditions.
<p align="center">
  <img src="figures/figure_2_erp_amplitudes_bar.png" width="400">
  <img src="figures/figure_3_erp_latencies_bar.png" width="400">
</p>

---

## 📁 Repository Structure
```text
├── data/               # De-identified processed EEG data (epochs)
├── scripts/            # Core analysis pipeline
│   ├── preprocess.py   # Artifact rejection (ICA) and filtering
│   └── erp_extract.py  # Epoching and N400/P300 averaging
├── figures/            # High-resolution plots for the manuscript
├── notebooks/          # Jupyter Notebooks for interactive visualization
├── requirements.txt    # Python dependencies
└── LICENSE             # MIT License

### 📂 Data Directory Structure

| File Name | Granularity | Key Features | Description |
|:---|:---|:---|:---|
| `DAR_Results_PegahM.csv` | Condition Level | ERP Amplitudes, Theta/Alpha | Aggregated summary for ANOVA testing. |
| `DAR_Trial_Level_Dataset_Pegah.csv` | Trial Level | RT_ms, Theta_Alpha, N400 | Detailed trial-by-trial data for LMM analysis. |
| `DAR_Study_Trial_Level_Data.csv` | Study Level | Group, Session, N400, P300 | Longitudinal comparisons (Pre vs. Post). |
| `processed_erp_data.csv` | Processed | Waveform Amplitudes | Cleaned data for Grand Average plotting. |


}")
