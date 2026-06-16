# DAR-N400-AI-Resistance
Official repository for “Distributed Authorial Resistance (DAR): Neural Correlates of Critical Engagement vs. Fatigue in Human-AI Collaborative Writing” — An EEG study on N400/P300 dynamics.
# Distributed Authorial Resistance (DAR): Neural Correlates of Critical Engagement vs. Fatigue

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![EEG Analysis: MNE](https://img.shields.io/badge/EEG-MNE--Python-green.svg)](https://mne.tools/stable/index.html)

This repository contains the official code, preprocessing pipelines, and statistical analysis for the paper: **"Distributed Authorial Resistance (DAR): N400 as a Marker of Epistemic Monitoring in Human-AI Collaborative Writing."**

## 🧠 Abstract
As AI-mediated writing becomes ubiquitous, understanding the human cognitive response to algorithmic suggestions is crucial. The **Distributed Authorial Resistance (DAR)** model posits that writers do not passively accept AI output but engage in active epistemic monitoring. 

This study utilizes Event-Related Potentials (ERPs) to differentiate between **Mental Fatigue** and **Active Resistance**. Our findings demonstrate that an increased **N400** amplitude—traditionally associated with semantic incongruity—serves as a neural signature of the writer's resistance to algorithmic homogenization, rather than a byproduct of cognitive depletion.

## 🔬 Key Neural Findings: N400 vs. Fatigue
A critical challenge in Neuro-AI studies is distinguishing effort-related fatigue from active task engagement. This project provides evidence that:
- **Selectivity:** Unlike fatigue, which causes a global attenuation (flattening) of ERPs, our DAR model shows a selective **enhancement of N400**.
- **Active Monitoring:** The increased N400 reflects the detection of "stylistic or semantic mismatches" between the AI's suggestion and the author's intent.
- **Decision Making:** The preservation or increase of the **P300** component further supports the "Active Agency" hypothesis over the "Passive Exhaustion" (Fatigue) account.

## 📂 Repository Structure
```text
├── data/               # Preprocessed EEG data (Anonymous)
├── scripts/            # Core analysis scripts
│   ├── preprocess.py   # Artifact rejection and filtering (MNE-Python)
│   ├── erp_extract.py  # Epoching and N400/P300 averaging
│   └── stats_models.R  # Linear Mixed-Effects Models for DAR
├── notebooks/          # Visualization (ERP Waveforms, Topomaps)
├── figures/            # High-resolution plots for the manuscript

# Distributed Authorial Resistance (DAR): Neural Correlates of Critical Engagement

Official repository for the study: **"Distributed Authorial Resistance (DAR): Neural Correlates of Critical Engagement vs. Fatigue in Human-AI Collaborative Writing."**

---

## 🖼️ Graphical Abstract
Below is the conceptual framework of the DAR model compared to passive AI-mediated writing.

![Graphical Abstract](./figures/graphic%20abstract.png)
*Figure 0: Conceptual overview of the DAR framework vs. Mental Fatigue during AI collaboration.*

---

## 📊 Key Experimental Results

### 1. Neural Markers of Epistemic Monitoring (N400)
The following waveform shows the Grand Average ERPs. The increased N400 amplitude in the DAR group signifies active semantic processing of AI-generated text.

![Figure 1: N400 Waveforms](./figures/figure_1_simulated_erp_n400.png)
*Figure 1: Grand average ERP waveforms at the Cz electrode site. Red: DAR Group, Blue: Control Group.*

### 2. Statistical Analysis of ERP Amplitudes
Comparison of peak amplitudes for N400 and P300 components.

![Figure 2: Amplitudes](./figures/figure_2_erp_amplitudes_bar.png)
*Figure 2: Mean peak amplitudes. Significant enhancement (p < 0.001) in N400 reflects deeper critical engagement.*

### 3. ERP Latency Results
Analysis of processing speed across different groups.

![Figure 3: Latencies](./figures/figure_3_erp_latencies_bar.png)
*Figure 3: Peak latency distribution, showing stability in processing speed despite higher cognitive load in DAR.*

### 4. Cognitive Engagement Index (Theta/Alpha)
The Frontal Theta/Alpha ratio serves as a robust marker for task engagement and executive control.

![Figure 4: Theta/Alpha Ratio](./figures/figure_4_theta_alpha_ratio.png)
*Figure 4: Frontal Theta/Alpha Ratio during AI-text evaluation. DAR group shows significantly higher engagement (Cohen's d = 0.82).*

---

## 📁 Repository Structure
- `data/`: Raw and processed EEG data (simulated/anonymized).
- `scripts/`: Python scripts for signal processing and ERP extraction.
- `notebooks/`: Jupyter Notebooks for statistical analysis and plotting.
- `figures/`: High-resolution versions of all plots.

## 🚀 How to Use
1. Clone the repository: `git clone https://github.com/Pegi1727/DAR-N400-AI-Resistance.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Run the analysis: `python scripts/analyze_erp.py`


└── requirements.txt    # Python dependencies

