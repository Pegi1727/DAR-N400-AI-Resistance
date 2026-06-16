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

📂 Data Directory Structure
This folder contains the datasets used for the Distributed Authorial Resistance (DAR) project. The data is organized into summary-level and trial-level formats to facilitate both statistical analysis and visualization of N400/P300 components and Theta/Alpha ratios.

📊 Dataset Overview
File Name	Granularity	Key Features / Columns	Description
DAR_Results_PegahM.csv	Condition Level	Condition, N400_uV, P300_uV, Theta_Alpha_Ratio, Interpretation	Aggregated summary of ERP amplitudes and cognitive load indicators per experimental condition.
DAR_Trial_Level_Dataset_Pegah.csv	Trial Level	Participant, Condition, Trial, RT_ms, Theta_Alpha, N400/P300	Detailed trial-by-trial data including reaction times (RT) and frequency band ratios for high-resolution analysis.
DAR_Study_Trial_Level_Data.csv	Study Level	Participant, Group, Session, Item_ID, N400_uV, P300_uV	Longitudinal study data capturing changes across different sessions (Pre-test vs. Post-test) and participant groups.
processed_erp_data.csv	Processed	time_ms, amplitude_uV, channel	Cleaned and filtered ERP waveform data ready for plotting Grand Average Waveforms.
🛠 Data Dictionary
N400_uV: Negative-going deflection peaking around 400ms (indicates conceptual processing/resistance).
P300_uV: Positive-going deflection peaking around 300ms (indicates attention and decision-making).
Theta_Alpha_Ratio: Indicator of cognitive workload and engagement.
RT_ms: Reaction time in milliseconds.
Condition: Experimental labels (conceptual_cliche, human_authentic, ai_neutral, etc.).
📝 Notes
All files are provided in .csv format for compatibility with Python (Pandas), R, and SPSS.
Data involving Prof. Pegah M. includes metadata such as author and date for version tracking of the results.

}")
