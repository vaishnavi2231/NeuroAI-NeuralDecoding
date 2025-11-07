# 🧠 Understanding Brain Waves: The Foundation of EEG

**Date:** Jan 5, 2025  
**Tags:** EEG, NeuroSignals, AlphaWaves  

---

## 🌍 Overview
This week, I explored the fundamentals of EEG — understanding how electrical activity across the scalp translates into meaningful brain rhythms.

---

## 🧠 Key Concepts
- **Delta (0.5–4 Hz):** Deep sleep and unconscious processes  
- **Theta (4–8 Hz):** Creativity, relaxation  
- **Alpha (8–12 Hz):** Calm wakefulness, eyes closed  
- **Beta (13–30 Hz):** Active thinking and movement  
- **Gamma (30+ Hz):** Cognitive processing  

---

## 🧪 Experiment
Used `MNE-Python` to visualize EEG sample data:

```python
import mne
raw = mne.io.read_raw_fif('sample_eeg.fif', preload=True)
raw.plot_psd(fmin=1, fmax=40)
