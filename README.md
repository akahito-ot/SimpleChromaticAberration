# Simple Chromatic Aberration (GPU)

A lightweight **chromatic aberration** effect for **DaVinci Resolve / Fusion**, implemented in `.fuse` format with a DCTL kernel.

---

## Features
- GPU-accelerated DCTL processing  
- Pixel-based **Spread** and optional **Blur**  
- **Border-aware sampling** (Clamp / Wrap / Mirror / Black)  
- **Preserve Alpha** toggle  
- Adjustable **Anchor**, **Rotation**, and **Scale**  
- Three channel pair modes: R&B / R&G / G&B  
- Optional soft blending via **Mix With Original**

---

## Description

This effect simulates chromatic aberration by shifting RGB channels separately in space.  
Unlike purely optical simulation, this version emphasizes **artistic control and speed**.  
Ideal for compositing, stylization, or adding subtle fringing.

---

## Installation

1. Place `SimpleChromaticAberration.fuse` into your **Fusion Modules / Fuses** folder:

   - **Windows:**  
     `C:\ProgramData\Blackmagic Design\DaVinci Resolve\Fusion\Modules\Fuses`

   - **macOS:**  
     `/Library/Application Support/Blackmagic Design/DaVinci Resolve/Fusion/Modules/Fuses`

2. Restart Resolve or Fusion.  
3. Find it under **AK_Tools → Simple Chromatic Aberration**.

---

## Parameters

| Parameter | Description |
|------------|-------------|
| **Channels** | Choose which RGB pairs to offset |
| **Spread (px)** | Channel offset radius in pixels |
| **Blur Radius (px)** | Box blur applied to shifted channels |
| **Anchor X/Y (%)** | Anchor point position |
| **Rotation (°)** | Direction of chromatic offset |
| **Scale (%)** | Relative scaling of offset channels |
| **Edge Mode** | Clamp / Wrap / Mirror / Black border |
| **Preserve Original Alpha** | Keep original alpha channel |
| **Mix With Original (%)** | Blend effect with source image |

---

## Author
**akahito_ot**  
[itch.io](https://akahito-ot.itch.io) / [GitHub](https://github.com/akahito-ot)

---

## 🪪 License
Released under the [MIT License](LICENSE).
