# DGME-T

🎞️ **DGME-T**: Directional Grid Motion Encoding for Transformer-Based Historical Camera Movement Classification.  
Accepted to **ACM Multimedia 2025 – The 7th ACM International Workshop on Analysis, Understanding and Promotion of Heritage Contents (SUMAC ’25)**,  
**27–31 October 2025, Dublin, Ireland 🇮🇪**.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Paper](https://img.shields.io/badge/Paper-arXiv%3A2510.15725-red)](https://arxiv.org/abs/2510.15725)
[![Code](https://img.shields.io/badge/Code-Coming%20Soon-lightgrey)](#)

---

## 🧭 Overview

**DGME-T** targets **camera movement classification** in **historical/archival footage**, where degradations (noise, blur, low contrast, irregular frame rates) weaken motion cues and hurt models trained on clean modern video.  

Our method, **Directional Grid Motion Encoding (DGME)**, represents motion by computing optical flow over a 3×3 grid and summarizing it as **directional histograms with an additional static bin**. The encoded motion is then combined with a **Video Swin Transformer** using **LayerNorm-calibrated features** and a **learnable scalar for fusion**.

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

```bibtex
@misc{lin2025dgmet,
      title={DGME-T: Directional Grid Motion Encoding for Transformer-Based Historical Camera Movement Classification}, 
      author={Tingyu Lin and Armin Dadras and Florian Kleber and Robert Sablatnig},
      year={2025},
      eprint={2510.15725},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2510.15725}, 
}
```

---

## 📜 License

- Code: **MIT License**  
- Figures and examples: **CC BY 4.0**

---

## 🔗 Related Links

- 🎥 [HISTORIAN Dataset (Source archival videos)](https://zenodo.org/record/6644516)  
- 📘 [SUMAC 2025](https://sumac-workshops.github.io/2025/)  
---

> Maintained by [@linty5](https://github.com/linty5) | TU Wien, Computer Vision Lab  
> For inquiries, please open an issue or contact tylin@cvl.tuwien.ac.at
