# Conventional Machine Learning Toolboxes and Methods for MI-EEG Decoding

This folder lists conventional (non-deep-learning) machine learning frameworks, toolboxes, and algorithm implementations commonly used for Motor Imagery (MI) EEG decoding. These methods typically rely on spatial filtering, feature engineering, and classical classifiers rather than end-to-end learned representations.

---

## ⚠️ Attribution and Citation Notice

All toolboxes and code repositories listed below are **owned and maintained by their respective authors**. We do not host or reimplement any of these methods.

**Before using any toolbox or method, you must read and follow the citation and usage instructions provided at the original repository and cite the corresponding original paper(s).**

If you accessed any of these resources through this repository or through our review paper, we would be pleased if you also cite:

> **A. Faezmehr, S. Fatemi, V. Shalchyan, and M. R. Daliri**,
> *"From EEG Signals to Commands: A Review of Machine Learning Pipelines in Motor Imagery Brain-Computer Interfaces."*

---

## 📋 Method Summary Table

| Method / Toolbox | Author(s) (Year) | Code Link | Novelty / Problem Addressed |
|---|---|---|---|
| **Regularized CSP (RCSP) Framework** | Lotte and Guan (2011) | [Code & software page](https://sites.google.com/site/fabienlotte/research/code-and-softwares) | Developed a unified framework and regularized CSP algorithms — addressing CSP overfitting and noise sensitivity. Includes: CSP, CCSP1, CCSP2, DL_CSP, DL_CSP_auto, DL_CSP_diff, generic_RCSP, GLR_CSP, SR_CSP, SSR_CSP, TR_CSP, WTR_CSP. |
| **MNS-ELR** | Hou et al. (2025) | https://github.com/Rayzhe/MNS-ELR | Jointly optimized spatial filters and classifiers with sparse L21/L1 regularization — addressing robust and efficient MI feature extraction. |
| **MTGCSP** | Mi et al. (2026) | https://github.com/RF-Li/MTGCSP/ | Introduced multi-scale time-window and frequency-band optimization with sparse joint CSP selection, addressing fixed temporal scales and independent time-frequency optimization. |
| **CSP-based CDF Filtering** | Faezmehr et al. (2026) | https://github.com/Ardalan-Faezmehr/CSP_based_CDF_Filtering | Provides an EEG preprocessing approach based on class-discrepancy-guided sub-band filtering and Common Spatial Pattern (CSP)-related processing. |
| **Covariance Toolbox** | Barachant | https://github.com/alexandrebarachant/covariancetoolbox | MATLAB toolbox for covariance-matrix processing and Riemannian geometry, developed for EEG/BCI applications. Relevant to covariance-matrix estimation, Riemannian geometry, spatial feature representations, and transfer learning / domain adaptation. |

---

### 📝 Note on the Lotte & Guan Code Page

The [code and software page](https://sites.google.com/site/fabienlotte/research/code-and-softwares) by Prof. Fabien Lotte hosts not only the regularized CSP implementations but also **additional codes and toolboxes from his other works**, including:

- Advanced frequency-band selection on the Riemannian manifold
  *(M. S. Yamamoto, F. Lotte, F. Yger, S. Chevallier, "Class-distinctiveness-based frequency band selection on the Riemannian manifold for oscillatory activity-based BCIs: preliminary results," IEEE EMBC, 2022)*
- Modeling complex EEG data distribution on the Riemannian manifold for outlier detection and multimodal classification
  *(M. S. Yamamoto, K. Sadatnejad, T. Tanaka, M. R. Islam, F. Dehais, Y. Tanaka, F. Lotte, "Modeling complex EEG data distribution on the Riemannian manifold toward outlier detection and multimodal classification," IEEE Trans. Biomed. Eng., 2023)*
- And several other related resources.

Users are encouraged to explore the full page to discover additional relevant tools.

---

## 📚 Full References

1. F. Lotte and C. Guan, "Regularizing common spatial patterns to improve BCI designs: Unified theory and new algorithms," *IEEE Trans. Biomed. Eng.*, vol. 58, no. 2, pp. 355–362, Feb. 2011, doi: 10.1109/TBME.2010.2082539.
2. R. Hou, S. Dong, W. Wang, T. Yu, Z. Yu, and Z. Gu, "A Novel Motor Imagery EEG Decoding Approach via Sparse Latent-Space Regression With Multi-Norm Regularization," *IEEE Trans. Consum. Electron.*, 2025.
3. J.-X. Mi, R.-F. Li, K. Liu, and W. Li, "Exploring multi-scale time group for common spatial pattern feature-based motor imagery EEG classification," *Biomed. Signal Process. Control*, vol. 112, p. 108591, 2026.
4. A. Faezmehr, A. Farrokhi, V. Shalchyan, and M. R. Daliri, "Designing class discrepancy-guided sub-band filter using common frequency pattern for preprocessing EEG signals in MI-BCIs," *Heliyon*, vol. 12, no. 2, 2026.
5. A. Barachant, "Covariance Toolbox," GitHub repository: https://github.com/alexandrebarachant/covariancetoolbox

---

## 🔗 Back to Main Repository

← [Return to main README](../../README.md)
