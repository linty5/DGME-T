# DGME-T

🎞️ **DGME-T**: Directional Grid Motion Encoding for Transformer-Based Historical Camera Movement Classification.  
Accepted to **ACM Multimedia 2025 – The 7th ACM International Workshop on Analysis, Understanding and Promotion of Heritage Contents (SUMAC ’25)**,  
**27–31 October 2025, Dublin, Ireland 🇮🇪**.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Paper](https://img.shields.io/badge/Paper-ACM%20MM%202025%20SUMAC-orange)](#)
[![Code](https://img.shields.io/badge/Code-Coming%20Soon-lightgrey)](#)

---

## 🧭 Overview

**DGME-T** targets **camera movement classification** in **historical/archival footage**, where degradations (noise, blur, low contrast, irregular frame rates) weaken motion cues and hurt models trained on clean modern video.  

We introduce **Directional Grid Motion Encoding (DGME)**—a compact motion prior computed from optical flow over a 3×3 grid with **directional histograms + static bin**—and **late-fuse** it with a **Video Swin Transformer** via **LayerNorm-calibrated features and a learnable scalar**.  

Beyond the model, we **standardize the label space** across domains: we unify two modern corpora into **four classes** (*static, tilt, pan, zoom*) and **restructure HISTORIAN** into **five classes** (*static, tilt, pan, zoom, track*).  

<p align="center">
  <img src="historian_sample.png" alt="Examples of camera motion in historical film" width="70%">
</p>

<p align="center">
  <em>Example frames from the HISTORIAN dataset illustrating typical visual degradation, blur, and low contrast encountered in archival footage.</em>
</p>

---

## 📦 Code Release (Coming Soon)

The source code, pretrained weights, and evaluation scripts will be publicly released after the ACM Multimedia 2025 presentation.  

---

## 📄 Citation

If you find **DGME-T** useful for your research, please cite:

Coming soon...

---

## 📜 License

- Code: **MIT License**  
- Figures and examples: **CC BY 4.0**

---

## 🔗 Related Links

- 🎥 [HISTORIAN Dataset (Source archival videos)](https://zenodo.org/record/6644516)  
- 📘 [ACM Multimedia 2025 – Workshops](https://acmmm2025.org/workshops)  
---

> Maintained by [@linty5](https://github.com/linty5) | TU Wien, Computer Vision Lab  
> For inquiries, please open an issue or contact tylin@cvl.tuwien.ac.at
