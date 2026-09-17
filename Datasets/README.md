# EEG Datasets for Motor Imagery Brain-Computer Interfaces

This folder lists commonly used, publicly available EEG datasets for Motor
Imagery (MI) Brain-Computer Interface research. They are grouped into three
sections:

1. **[Commonly Used Datasets](#-commonly-used-datasets)** — Widely adopted
   benchmark datasets with detailed specifications.
2. **[Other Datasets](#-other-datasets)** — Additional MI datasets covering
   diverse paradigms (multi-class, multi-joint, clinical, etc.).
3. **[Dataset Collections](#-dataset-collections)** — Frameworks and
   repositories that aggregate many BCI datasets under a unified interface.

---

## ⚠️ Attribution and Citation Notice

All datasets listed below are **owned and maintained by their respective
authors and institutions**. We do not host any of the data.

**Before using any dataset, you must read and follow the citation and usage
instructions provided at the original source and cite the corresponding
original paper(s).**

If you accessed any of these datasets through this repository or through our
review paper, we would be pleased if you also cite:

> **A. Faezmehr, S. Fatemi, V. Shalchyan, and M. R. Daliri**,
> *"From EEG Signals to Commands: A Review of Machine Learning Pipelines in
> Motor Imagery Brain-Computer Interfaces."*


## 📌 Commonly Used Datasets

These datasets are the most frequently used benchmarks in MI-BCI research.

---

### BCIC-III-IIIa

- **Access:** http://www.bbci.de/competition/iii/ · [Dataset description](http://www.bbci.de/competition/iii/desc_IIIa.pdf)
- **Subjects:** 3 (k3, k6, l1)
- **Channels:** 60 EEG
- **Sampling rate:** 250 Hz
- **Classes:** 4 (left hand, right hand, foot, tongue)
- **Citation:** B. Blankertz et al., *"The BCI Competition III: Validating Alternative Approaches to Actual BCI Problems,"* IEEE Trans. Neural Syst. Rehabil. Eng., vol. 14, no. 2, pp. 153–159, Jun. 2006.

---

### BCIC-III-IVa

- **Access:** http://www.bbci.de/competition/iii/ · [Dataset description](http://www.bbci.de/competition/iii/desc_IVa.html)
- **Subjects:** 5 (aa, al, av, aw, ay)
- **Channels:** 118 EEG
- **Sampling rate:** 1000 Hz and 100 Hz versions
- **Classes:** 2 (right hand, foot)
- **Notes:** Suitable for evaluating algorithms with limited training data
- **Citation:** B. Blankertz et al., *"The BCI Competition III: Validating Alternative Approaches to Actual BCI Problems,"* IEEE Trans. Neural Syst. Rehabil. Eng., vol. 14, no. 2, pp. 153–159, Jun. 2006.

---

### BCIC-IV-1

- **Access:** https://www.bbci.de/competition/iv/#dataset1
- **Subjects:** 7 healthy (data for subjects c, d, e were artificially generated)
- **Channels:** 59 EEG
- **Sampling rate:** 1000 Hz (also available downsampled at 100 Hz)
- **Classes:** 2 MI tasks, selected from left hand, right hand, and foot
- **Citation:** BCI Competition IV (2008), http://www.bbci.de/competition/iv/

---

### BCIC-IV-2a

- **Access:** http://www.bbci.de/competition/iv/#dataset2a
- **Subjects:** 9 healthy
- **Channels:** 22 Ag/AgCl EEG
- **Sampling rate:** 250 Hz (bandpass 0.5–100 Hz)
- **Classes:** 4 (left hand, right hand, feet, tongue)
- **Citation:** BCI Competition IV (2008), http://www.bbci.de/competition/iv/

---

### BCIC-IV-2b

- **Access:** http://www.bbci.de/competition/iv/#dataset2b
- **Subjects:** 9
- **Channels:** 3 EEG (C3, Cz, C4) + 3 EOG
- **Sampling rate:** 250 Hz (bandpass 0.5–100 Hz)
- **Classes:** 2 MI tasks (left hand, right hand)
- **Citation:** BCI Competition IV (2008), http://www.bbci.de/competition/iv/

---

### PhysioNet EEG Motor Movement/Imagery

- **Access:** https://doi.org/10.13026/C28G6P
- **Subjects:** 109
- **Channels:** 64 EEG
- **Sampling rate:** 160 Hz
- **Classes:** 4 (left fist, right fist, both fists, both feet) — includes both motor execution and motor imagery
- **Notes:** Large dataset, well-suited for deep learning. Recorded with the BCI2000 system.
- **Citation:** Schalk, G., McFarland, D. J., Hinterberger, T., Birbaumer, N., and Wolpaw, J. R. (2004). *"BCI2000: A General-Purpose Brain-Computer Interface (BCI) System."* IEEE Trans. Biomed. Eng. 51, 1034–1043. doi: 10.1109/TBME.2004.827072

---

### OpenBMI

- **Access:** https://doi.org/10.1016/j.jneumeth.2024.109999
- **Subjects:** 54 healthy
- **Channels:** 62 Ag/AgCl EEG
- **Sampling rate:** 1000 Hz
- **Classes (MI paradigm):** 2 (left hand, right hand)
- **Sessions:** 2 per subject; 200 trials per session (100 per class)
- **Trial duration:** 4 s
- **Notes:** Covers three BCI paradigms: MI, ERP, and SSVEP.
- **Citation:** M.-H. Lee et al., *"EEG dataset and OpenBMI toolbox for three BCI paradigms: An investigation into BCI illiteracy,"* GigaScience, vol. 8, no. 5, May 2019, giz002.

---

### High Gamma Dataset (HGD)

- **Access:** https://github.com/robintibor/high-gamma-dataset
- **Subjects:** 14
- **Channels:** 128 EEG
- **Sampling rate:** 500 Hz
- **Classes:** 4 (left hand, right hand, feet, rest)
- **Trials:** ~880 training + ~160 test per subject
- **Citation:** Schirrmeister, R. T. et al., *"Deep learning with convolutional neural networks for EEG decoding and visualization,"* Human Brain Mapping 38, 5391–5420, 2017.

---

### GigaDB MI Dataset

- **Access:** https://doi.org/10.1093/gigascience/gix034
- **Subjects:** 52 healthy (19 female; 2 both-handed, rest right-handed)
- **Channels:** 64 Ag/AgCl active electrodes (10–10 system)
- **Sampling rate:** 512 Hz
- **Classes:** 2 (left hand, right hand MI)
- **Trials:** 100–120 per class per subject
- **Notes:** Also includes non-task EEG (eye blinking, eye movement, head movement, jaw clenching, resting state), EMG, and questionnaire data. Contains both well-discriminated and less-discriminative subjects.
- **Citation:** Cho, H., Ahn, M., Ahn, S., Kwon, M. & Jun, S. C., *"EEG datasets for motor imagery brain–computer interface,"* GigaScience 6, 1–8, 2017.

---

## 📦 Other Datasets

Additional MI datasets covering diverse paradigms, populations, and clinical applications.

### Classical BCI Competition Datasets

| Dataset | Access | Subjects | Channels | Sampling Rate | Classes | Notes |
|---|---|---|---|---|---|---|
| **BCIC-III-IIIb** | [Link](http://www.bbci.de/competition/iii/) · [Description](http://www.bbci.de/competition/iii/desc_IIIb.pdf) | 3 (O3, S4, X11) | 3 (10–20 system) | 125 Hz (0.5–30 Hz notch) | 2 | 7 s trials; 320 (O3), 1080 (S4, X11) trials |
| **BCIC-III-IVb** | [Link](http://www.bbci.de/competition/iii/) · [Description](https://www.bbci.de/competition/iii/desc_IVb.html) | 1 | 118 (10/20) | 1000 Hz | 2 (LH, RF) | 210 trials/class; visual cues 3.5 s; bandpass 0.5–200 Hz |
| **BCIC-III-V** | [Link](https://www.bbci.de/competition/iii/) · [Description](https://www.bbci.de/competition/iii/desc_V.html) | 3 healthy | 32 | 512 Hz | 3 (LH, RH, word generation) | 3 sessions per subject |

### Task-Diverse MI Datasets

| Dataset | Access | Tasks | Sampling Rate | Channels | Subjects | Notes |
|---|---|---|---|---|---|---|
| **Ofner et al.** | [Link](https://zenodo.org/records/834976) | EF, EE, SP, PR, HC, HO | 521 Hz | 128 | 15 | More inclined to joints |
| **Cho et al.** | [Link](http://gigadb.org/dataset/100295) | LFinger, RFinger | 512 Hz | 64 | 52 | Imagine movement of each finger |
| **Kaya et al.** | [Link](https://doi.org/10.6084/m9.figshare.c.3917698.v1) | LH, RH, LL, RL, T | 200 Hz | 22 | 13 | 4-MI paradigms |
| **Ma et al.** | [Link](https://doi.org/10.7910/DVN/RBN3XG) | RH, RE | 1000 Hz | 64 | 25 | Different joints of the same limb |
| **MIMED** | [Link](https://data.mendeley.com/datasets/zs25xxjkm9/3) | RU, RD, LU, LD, ST, SI | 128 Hz | 14 | 30 | Rehab-related, 4-band MI |
| **SHU** | [Link](https://figshare.com/articles/software/shu_dataset/19228725/1) | LH, RH | 250 Hz | 32 | 25 | Cross-session: 5-day × 5-period |

**Task abbreviations:** EF = elbow flexion, EE = elbow extension, SP = shoulder pronation, PR = pronation, HC = hand close, HO = hand open, LH = left hand, RH = right hand, LL = left leg, RL = right leg, T = tongue, LFinger = left finger, RFinger = right finger, RE = right elbow, RU = right upper limb, RD = right lower limb, LU = left upper limb, LD = left lower limb, ST = standing, SI = sitting.

### Clinical / Patient Datasets

| Dataset | Access | Disease | Tasks | Sampling Rate | Channels | Subjects | Trials | System |
|---|---|---|---|---|---|---|---|---|
| **LLMI-Stroke** | [Link](https://figshare.com/articles/dataset/Lower_limb_motor_imagery_EEG_dataset_based_on_the_multi-paradigm_and_longitudinal-training_of_stroke_patients/27130299) | Stroke-recovered | IG, KS | 1000 Hz | 64 | 27 | 40 | 10/20 |
| **XuanWu-Stroke** | [Link](https://figshare.com/articles/dataset/EEG_datasets_of_stroke_patients/21679035/5) | Acute stroke | LH, RH | 500 Hz | 32 | 50 | 40 | 10/10 |
| **EEGET-ALS** | [Link](https://doi.org/10.6084/m9.figshare.c.6910027.v1) | ALS | LHU, RHU, LLU, RLU, OM, NH, SH | 128 Hz | 32 | 6 | 210 | 10/10 |
| **WCCI2020-Glasgow** | [Link](https://github.com/5anirban9/Clinical-Brain-Computer-Interfaces-Challenge-WCCI-2020-Glasgow) | Hemiplegia | LH, RH | 512 Hz | 12 | 10 | 40 | 10/20 |

**Task abbreviations:** IG = idle ground, KS = knee support, LHU = left hand up, RHU = right hand up, LLU = left leg up, RLU = right leg up, OM = open mouth, NH = nod head, SH = shake head.

---

## 🗃️ Dataset Collections

These are frameworks and databases that aggregate many BCI datasets under a standardized interface, making it easier to benchmark and compare algorithms across datasets.

---

### MOABB (Mother of All BCI Benchmarks)

- **Official website:** https://moabb.neurotechx.com/
- **Dataset summary:** https://moabb.neurotechx.com/docs/dataset_summary.html
- **GitHub:** https://github.com/NeuroTechX/moabb
- **Description:** A framework providing standardized access to a large collection of publicly available BCI datasets and enabling reproducible benchmarking of EEG decoding algorithms. Current catalog: **160 datasets, >3,600 subjects**.

---

### BNCI Horizon 2020

- **Official database:** https://bnci-horizon-2020.eu/database/data-sets
- **MOABB documentation:** https://moabb.neurotechx.com/docs/dataset_summary.html
- **Description:** A collection of openly available datasets covering several BCI paradigms, including numerous motor imagery datasets. Examples: BNCI2014-001, BNCI2014-002, BNCI2014-004, BNCI2015-001, BNCI2015-004, and BNCI2019-001.
- **Useful for:** Cross-subject, cross-session, and transfer-learning investigations.

---

## 📝 Notes

- **Sampling rates** are as reported at the original source; some datasets provide multiple versions (e.g., downsampled).
- **Channel counts** refer to EEG channels only unless otherwise stated.
- Always consult the original dataset page for the most up-to-date information, license terms, and citation requirements.

---

## 🔗 Back to Main Repository

← [Return to main README](../README.md)

