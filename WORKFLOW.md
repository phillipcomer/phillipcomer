# PixInsight Workflow – Helix Nebula by Phillip Comer

This document outlines the full manual PixInsight processing flow used on my Helix Nebula image. No automated AI processing was used — only calibrated steps built from experience.

---

## 📌 Original File
- Source: Seestar S50 stacked image
- Format: Native JPEG (exported to TIFF for processing)

---

## 🧰 Step-by-Step Processing

### 1. Background Neutralization
- Removed natural color cast from light pollution and atmospheric tint.
- Tool: `BackgroundNeutralization`
- Reference: average sky sample

---

### 2. Dynamic Background Extraction (DBE)
- Created a custom point grid to subtract uneven background gradients.
- Tool: `DynamicBackgroundExtraction`
- Parameters:
  - Tolerance: 0.5
  - Sample radius: 15
  - Correction: Subtraction

---

### 3. EZ Denoise
- Smoothed noise without removing nebular details.
- Tool: `EZ Processing Suite > EZ Denoise`
- Used with default mild parameters
- Masking enabled to preserve star edges

---

### 4. Histogram Transformation
- Non-linear stretch to reveal brightness of nebular detail
- Tool: `HistogramTransformation`
- Manual adjustment:
  - Shadows clipped just above black point
  - Midtones stretched gently

---

### 5. Curves Transformation
- Enhanced contrast and deepened red/blue features
- Tool: `CurvesTransformation`
- Adjusted:
  - RGB-K (contrast S-curve)
  - Blue (boosted)
  - Red (refined core)

---

### 6. Star Reduction (optional)
- Minimal, only for peripheral stars
- Tool: `MorphologicalTransformation` via star mask
- Iterations: 2
- Shape: Circular, threshold 0.6

---

### 7. Final Annotation (added in post)
- Added "Captured by Phillip Comer" footer in Photoshop for attribution

---

## 🧪 Notes

- All operations performed manually with close attention to image integrity
- No artificial content generation, cloning, or fabrications applied
- No AI upscaling used — resolution is native to stacked capture

---

© Phillip Comer, 2025  
Crow Hill Observatory – ComerConsults
