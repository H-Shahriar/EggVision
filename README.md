# 🥚 EggVision

<p align="center">
  <img src="eggvision/Assets.xcassets/AppIcon.appiconset/appstore.png" width="150"/>
</p>

<p align="center">
  An iOS capstone project that classifies egg types and predicts the gender 
  of unhatched chicks using LiDAR-based shape analysis — offering a humane 
  solution to reduce mass culling of male chicks in the poultry industry.
</p>

---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Gender Prediction Logic](#gender-prediction-logic)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Screenshots](#screenshots)
- [Credits](#credits)
- [License](#license)

---

## 🔍 Overview

EggVision is an iOS-based capstone project developed for **Harmony Harvesty Farm**
that uses machine learning and spatial computing to:

- Classify eggs as **chicken** or **quail** using CoreML
- Predict the **gender of unhatched chicks** for chicken eggs using
  LiDAR-based shape analysis

By analyzing egg morphology non-invasively, EggVision provides a practical
and humane alternative to the mass culling of male chicks — a common but
controversial practice in the poultry industry.

---

## ✨ Features

- 🐣 **Egg Classification** – Detect and classify egg type (chicken or quail) using CoreML
- ⚧️ **Gender Prediction** – Predict chick gender using Shape Index formula
- 📡 **LiDAR Scanning** – Automatically measure egg dimensions using ARKit + SceneKit
- ✍️ **Manual Input** – Enter Shape Index values manually as an alternative
- 🎨 **Clean UI** – Intuitive SwiftUI interface designed for ease of use

---

## 🧮 Gender Prediction Logic

EggVision uses a **rule-based gender prediction system** based on threshold
values from Kayadan & Uzun (2023). No separate machine learning model is
used for gender classification.

### Formula
Shape Index (SI) = Short Axis / Long Axis

| Result | Prediction |
|--------|-----------|
| SI > 0.50 | 🔴 Likely **Female** |
| SI ≤ 0.50 | 🔵 Likely **Male** |

> Measurements can be taken **automatically** using LiDAR or entered
> **manually** by the user.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|-----------|---------|
| Swift / SwiftUI | UI and app logic |
| CoreML | Egg type classification |
| ARKit | LiDAR scanning and spatial tracking |
| SceneKit | 3D dimension measurement |
| Rule-based system | Chick gender prediction |

---

## 🚀 Getting Started

### Requirements

- macOS with **Xcode 15** or later
- **iPhone Pro** model with LiDAR sensor
  - iPhone 13 Pro, 14 Pro, or 15 Pro

### Installation

1. **Clone the repository**
```bash
   git clone https://github.com/H-Shahriar/EggVision.git
```

2. **Open in Xcode**
```bash
   cd EggVision
   open EggVision.xcodeproj
```

3. **Connect your device**
   - Plug in your LiDAR-enabled iPhone
   - Select your device as the build target
   - Click **Run** ▶️

---

## 📸 Screenshots

<p align="center">
  <img src="eggvision/Assets.xcassets/AppIcon.appiconset/appstore.png" width="150"/>
</p>

> 📁 App screenshots coming soon — will be added to a `/screenshots` folder.

---

## 👤 Credits

| Role | Details |
|------|---------|
| Developer | Hasan Shahriar |
| Sponsor | Harmony Harvesty Farm |
| Institution | University of Canberra, 2025 |
| Research Basis | Kayadan & Uzun (2023) |

---

## 📄 License

MIT License — Copyright (c) 2024–2025

Permission is hereby granted, free of charge, to any person obtaining a
copy of this software to deal in the Software without restriction,
including the rights to use, copy, modify, merge, publish, distribute,
sublicense, and/or sell copies of the Software, subject to the following
conditions:

- The above copyright notice and this permission notice shall be included
  in all copies or substantial portions of the Software.
- Neither the name of the copyright holder nor contributors may be used
  to endorse products derived from this software without prior written
  permission.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND.
