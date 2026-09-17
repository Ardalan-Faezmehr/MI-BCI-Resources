# Deep Learning Toolboxes and Models for MI-EEG Decoding

This folder lists deep learning frameworks, toolboxes, and model implementations commonly used for Motor Imagery (MI) EEG decoding. Each entry includes the original paper, the official code repository, and the main contribution or problem addressed.

---

## ⚠️ Attribution and Citation Notice

All toolboxes and code repositories listed below are the work of their original authors and are maintained by them. Please refer to their repositories for the code.

**Before using any toolbox or method, you must read and follow the citation and usage instructions provided in the original repository and cite the corresponding original paper(s).**

If you accessed any of these resources through this repository or through our review paper, we would be pleased if you also cite:

> **A. Faezmehr, S. Fatemi, V. Shalchyan, and M. R. Daliri**,
> *"From EEG Signals to Commands: A Review of Machine Learning Pipelines in Motor Imagery Brain-Computer Interfaces."*

---

## 📋 Model Summary Table

| Model / Toolbox | Author(s) (Year) | Code Link | Novelty / Problem Addressed |
|---|---|---|---|
| **Braindecode (ShallowConvNet, DeepConvNet)** | Schirrmeister et al. (2017) | Original link: https://github.com/robintibor/braindecode/ · Updated link: https://github.com/braindecode/braindecode *(also covers many advanced DL models)* | Introduced end-to-end deep ConvNets for raw EEG decoding — replacing handcrafted features with learned representations. |
| **EEGNet** | Lawhern et al. (2018) | https://github.com/vlawhern/arl-eegmodels | Introduced EEGNet, a compact CNN with depthwise and separable convolutions designed to generalize across diverse BCI paradigms while learning interpretable EEG features. |
| **EEG-TCNet** | Ingolfsson et al. (2020) | https://github.com/iis-eth-zurich/eeg-tcnet | Introduced EEG-TCNet, a lightweight temporal convolutional network for MI-EEG decoding — achieving competitive accuracy with few trainable parameters and low computational complexity for embedded, resource-constrained BCI applications. |
| **EEG-ITNet** | Salami et al. (2022) | https://github.com/AbbasSalami/EEG-ITNet | Introduced EEG-ITNet, a compact end-to-end architecture combining inception and dilated causal convolutions — capturing multi-scale spectral, spatial, and temporal EEG features with improved interpretability. |
| **FBMSNet** | Liu et al. (2022) | https://github.com/Want2Vanish/FBMSNet | Introduced FBMSNet, an end-to-end filter-bank multiscale CNN — combining multiview spectral representations with mixed depthwise convolutions and joint cross-entropy/center loss to learn discriminative MI-EEG features. |
| **IFNet** | Wang et al. (2023) | https://github.com/Jiaheng-Wang/IFNet | Introduced IFNet, a lightweight CNN for MI-EEG decoding — explicitly modeling cross-frequency interactions between low- and high-frequency bands to learn robust spectro-spatio-temporal features. |
| **EEG-SimpleConv** | El Ouahidi et al. (2024) | https://github.com/elouayas/EEGSimpleconv | Introduced EEG-SimpleConv, a straightforward 1D CNN baseline for MI-EEG decoding — using standard components to achieve competitive performance, efficient inference, and strong cross-subject knowledge transfer. |
| **MT-MBCNN** | Cai et al. (2024) | https://github.com/my94my/MT-MBCNN | Introduced MT-MBCNN, a multi-task multi-branch CNN for MI-EEG decoding — jointly learning spatial-temporal and spectral representations with class-prototype learning and sample augmentation. |
| **OPTICAL** | Kumar et al. (2019) | https://github.com/ShiuKumar/OPTICAL | Introduced OPTICAL, a hybrid CSP–LSTM framework for MI-EEG decoding — combining spatially filtered CSP features with sliding-window temporal representations and an LSTM-derived regression feature for improved classification. |
| **TD-LSTM** | Karimian-Kelishadrokhi et al. (2024) | https://github.com/jingwang2020/ECML-PKDD_MMCNN | Introduced TD-LSTM for MI/ME-EEG decoding — combining time-distributed processing with LSTM to efficiently learn spatiotemporal dependencies from long multichannel EEG sequences. |
| **EEG-Transformer** | Song et al. (2021) | https://github.com/anranknight/EEG-Transformer | Introduced EEG-Transformer for EEG decoding — using attention transformations across spatial and temporal dimensions to capture global dependencies with a lightweight architecture. |
| **LightConvNet** | Ma et al. (2023) | https://github.com/Ma-Xinzhi/LightConvNet | Introduced LightConvNet, a temporal-dependency learning CNN with attention — segmenting EEG into time windows and using temporal attention to capture MI-related patterns and their dependencies across different stages of the task. |
| **EEG Conformer** | Song et al. (2023) | https://github.com/eeyhsong/EEG-Conformer | Introduced EEG Conformer, a compact convolutional Transformer — combining convolutional layers for local temporal–spatial features with self-attention for global dependencies to overcome the limited receptive field of CNNs. |
| **LMDA-Net** | Miao et al. (2023) | https://github.com/MiaoZhengQing/LMDA-Code | Introduced LMDA-Net, a lightweight multi-dimensional attention network — using channel and depth attention to improve EEG feature integration, generalization, and interpretability while addressing the low spatial resolution, low SNR, and instability of EEG decoding. |
| **ATCNet** | Altaheri (2023) | https://github.com/Altaheri/EEG-ATCNet | Introduced ATCNet, a physics-informed attention temporal convolutional network — combining domain-specific design, multi-head self-attention, temporal convolutions, and sliding-window augmentation to improve MI decoding with relatively few parameters. |
| **HCANN** | Ji et al. (2024) | https://github.com/youshuoji/HCANN | Introduced HCANN, a hybrid CNN–multi-head self-attention network — combining multi-scale depthwise separable convolutions with adaptive attention to jointly capture temporal and complementary spatial representations across EEG tasks. |
| **ADFCNN** | Tao et al. (2024) | https://github.com/UMTao/ADFCNN-MI | Introduced ADFCNN, an attention-based dual-scale fusion CNN — extracting spectral and spatial features at multiple scales and using self-attention to effectively fuse complementary representations from different scales. |
| **CTNet** | Zhao et al. (2024) | https://github.com/snailpt/CTNet | Introduced CTNet, a convolutional Transformer network — combining EEGNet-like convolutional layers for local spatial features with Transformer self-attention for global dependencies to improve MI-EEG decoding. |
| **TSFF-Net** | Miao et al. (2024) | https://github.com/MiaoZhengQing/TSFF | Introduced TSFF-Net, a lightweight time–space–frequency feature-fusion network for low-channel MI-EEG — combining time–frequency and time–space representations with MMD-based feature alignment to compensate for the limited spatial information of three-channel EEG. |
| **SST-DPN** | Han et al. (2025) | https://github.com/hancan16/SST-DPN | Introduced SST-DPN, a spatial–spectral and temporal dual-prototype network — combining lightweight spatial–spectral attention, parameter-free multi-scale variance pooling, and dual-prototype learning to improve feature distribution and generalization under small-sample conditions. |
| **MSCFormer** | Zhao et al. (2025) | https://github.com/snailpt/MSCFormer | Introduced MSCFormer, a multi-scale convolutional Transformer — using multiple CNN branches to capture diverse features and a Transformer encoder to model global dependencies, addressing individual EEG variability and the limited receptive field of conventional CNNs. |
| **TCFormer** | Altaheri et al. (2025) | https://github.com/altaheri/TCFormer | Introduced TCFormer, a temporal convolutional Transformer — integrating multi-kernel CNNs, grouped-query self-attention, and dilated causal convolutions to capture spatial–temporal features, global contextual dependencies, and long-range temporal patterns. |
| **TMSA-Net** | Zhao et al. (2025) | https://github.com/Whit3Zhao/TMSA-Net | Introduced TMSA-Net, a computationally efficient CNN–Transformer architecture with a novel attention mechanism — designed to better capture the interrelationships between local and global EEG features that conventional CNN–Transformer models may overlook. |

---

## 📚 Full References

1. R. T. Schirrmeister et al., "Deep learning with convolutional neural networks for EEG decoding and visualization," *Hum. Brain Mapp.*, vol. 38, no. 11, pp. 5391–5420, 2017.
2. V. J. Lawhern, A. J. Solon, N. R. Waytowich, S. M. Gordon, C. P. Hung, and B. J. Lance, "EEGNet: a compact convolutional neural network for EEG-based brain–computer interfaces," *J. Neural Eng.*, vol. 15, no. 5, p. 56013, 2018.
3. T. M. Ingolfsson, M. Hersche, X. Wang, N. Kobayashi, L. Cavigelli, and L. Benini, "EEG-TCNet: An accurate temporal convolutional network for embedded motor-imagery brain–machine interfaces," in *2020 IEEE International Conference on Systems, Man, and Cybernetics (SMC)*, IEEE, 2020, pp. 2958–2965.
4. A. Salami, J. Andreu-Perez, and H. Gillmeister, "EEG-ITNet: An explainable inception temporal convolutional network for motor imagery classification," *IEEE Access*, vol. 10, pp. 36672–36685, 2022.
5. K. Liu, M. Yang, Z. Yu, G. Wang, and W. Wu, "FBMSNet: A filter-bank multi-scale convolutional neural network for EEG-based motor imagery decoding," *IEEE Trans. Biomed. Eng.*, vol. 70, no. 2, pp. 436–445, 2022.
6. J. Wang, L. Yao, and Y. Wang, "IFNet: An interactive frequency convolutional neural network for enhancing motor imagery decoding from EEG," *IEEE Trans. Neural Syst. Rehabil. Eng.*, vol. 31, pp. 1900–1911, 2023.
7. Y. El Ouahidi, V. Gripon, B. Pasdeloup, G. Bouallegue, N. Farrugia, and G. Lioi, "A strong and simple deep learning baseline for BCI motor imagery decoding," *IEEE Trans. Neural Syst. Rehabil. Eng.*, vol. 32, pp. 3338–3347, 2024.
8. Z. Cai, T. Luo, and X. Cao, "Multi-branch spatial-temporal-spectral convolutional neural networks for multi-task motor imagery EEG classification," *Biomed. Signal Process. Control*, vol. 93, p. 106156, 2024.
9. S. Kumar, A. Sharma, and T. Tsunoda, "Brain wave classification using long short-term memory network based OPTICAL predictor," *Sci. Rep.*, vol. 9, no. 1, p. 9153, 2019.
10. M. Karimian-Kelishadrokhi and F. Safi-Esfahani, "TD-LSTM: a time distributed and deep-learning-based architecture for classification of motor imagery and execution in EEG signals," *Neural Comput. Appl.*, vol. 36, no. 25, pp. 15843–15868, 2024.
11. Y. Song, X. Jia, L. Yang, and L. Xie, "Transformer-based spatial-temporal feature learning for EEG decoding," *arXiv Prepr. arXiv2106.11170*, 2021.
12. X. Ma, W. Chen, Z. Pei, J. Liu, B. Huang, and J. Chen, "A temporal dependency learning CNN with attention mechanism for MI-EEG decoding," *IEEE Trans. Neural Syst. Rehabil. Eng.*, vol. 31, pp. 3188–3200, 2023.
13. Y. Song, Q. Zheng, B. Liu, and X. Gao, "EEG Conformer: Convolutional Transformer for EEG Decoding and Visualization," *IEEE Trans. Neural Syst. Rehabil. Eng.*, vol. 31, pp. 710–719, 2023, doi: 10.1109/TNSRE.2022.3230250.
14. Z. Miao, M. Zhao, X. Zhang, and D. Ming, "LMDA-Net: A lightweight multi-dimensional attention network for general EEG-based brain-computer interfaces and interpretability," *Neuroimage*, vol. 276, p. 120209, 2023.
15. H. Altaheri, G. Muhammad, and M. Alsulaiman, "Physics-informed attention temporal convolutional network for EEG-based motor imagery classification," *IEEE Trans. Ind. Informatics*, vol. 19, no. 2, pp. 2249–2258, 2022.
16. Y. Ji et al., "A novel hybrid decoding neural network for EEG signal representation," *Pattern Recognit.*, vol. 155, p. 110726, 2024.
17. W. Tao et al., "ADFCNN: Attention-based dual-scale fusion convolutional neural network for motor imagery brain–computer interface," *IEEE Trans. Neural Syst. Rehabil. Eng.*, vol. 32, pp. 154–165, 2023.
18. W. Zhao, X. Jiang, B. Zhang, S. Xiao, and S. Weng, "CTNet: a convolutional transformer network for EEG-based motor imagery classification," *Sci. Rep.*, vol. 14, no. 1, p. 20237, 2024.
19. Z. Miao and M. Zhao, "Time–space–frequency feature fusion for 3-channel motor imagery classification," *Biomed. Signal Process. Control*, vol. 90, p. 105867, 2024.
20. C. Han, C. Liu, J. Wang, Y. Wang, C. Cai, and D. Qian, "A spatial–spectral and temporal dual prototype network for motor imagery brain–computer interface," *Knowledge-Based Syst.*, vol. 315, p. 113315, 2025.
21. W. Zhao, B. Zhang, H. Zhou, D. Wei, C. Huang, and Q. Lan, "Multi-scale convolutional transformer network for motor imagery brain-computer interface," *Sci. Rep.*, vol. 15, no. 1, p. 12935, 2025.
22. H. Altaheri, F. Karray, and A.-H. Karimi, "Temporal convolutional transformer for EEG based motor imagery decoding," *Sci. Rep.*, vol. 15, no. 1, p. 32959, 2025.
23. Q. Zhao and W. Zhu, "TMSA-Net: A novel attention mechanism for improved motor imagery EEG signal processing," *Biomed. Signal Process. Control*, vol. 102, p. 107189, 2025.

---

## 🔗 Back to Main Repository

← [Return to main README](../../README.md)
