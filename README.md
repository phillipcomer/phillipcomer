# 🔭 Helix Nebula (NGC 7293) – Astrophotography by Phillip Comer

This project showcases an original astrophotograph of the Helix Nebula (NGC 7293), captured using the **Seestar S50 telescope** under dark skies at 37°N, 90°W. Over 13 minutes of stacked exposure brought out rich ionization details and color gradients consistent with high-resolution scientific imagery.

---

## 📸 Imaging Details
- **Telescope**: Seestar S50
- **Exposure Time**: 13 minutes (stacked)
- **Location**: Missouri, USA (approx. 37°N, 90°W)
- **Target**: NGC 7293 (The Helix Nebula)
- **Capture Time**: 2025-07-30 @ 04:49 UTC

---

## 🧠 Processing Workflow (PixInsight)
Post-processing was performed using **PixInsight**, following a verified workflow:

1. **Calibration** – Bias/Dark subtraction
2. **Star Alignment** – With PSF matching
3. **Noise Reduction** – MultiscaleLinearTransform
4. **Stretching** – HistogramTransformation
5. **Color Enhancement** – SCNR + Curves
6. **Deconvolution** – With star mask protection
7. **Final Touches** – Saturation boost, star sharpening

See full workflow: [`NGC7293_PixInsight_Workflow.pdf`](./NGC7293_PixInsight_Workflow.pdf)

---

## 📁 File Proof
- `NGC7293_Raw.jpg` – Original stacked image
- `NGC7293_Final.jpg` – Final processed result
- `NGC7293_SideBySide.jpg` – Raw vs. Processed
- `NGC7293_PixInsight_Workflow.pdf` – Full steps

Each file is timestamped, geotagged, and reproducible from Seestar logs.

---

## 🧠 Why This Matters

This project is proof of **authentic human work** — not AI-generated, not simulated.  
It reflects my journey in astrophotography and post-processing, as part of **ComerConsults**.

---

### 🌌 ComerConsults  
*Field systems | Remote imaging | Edge observatories*  
📡 `@phillipcomer`
