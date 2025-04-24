🥚 EggVision
EggVision is an iOS-based capstone project that classifies egg types (chicken or quail) and predicts the gender of unhatched chicks for chicken eggs using LiDAR-based shape analysis. It offers a humane and efficient solution to reduce the mass culling of male chicks in the poultry industry by analyzing egg morphology.

––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––

Features

Detect and classify egg type (chicken or quail) using CoreML
Predict chick gender for chicken eggs using Shape Index
Automatically measure egg dimensions using LiDAR and SceneKit
Manual input option for Shape Index-based predictions
Clean SwiftUI interface
––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––

Gender Prediction Logic
This app uses a rule-based gender prediction system based on the threshold values from Kayadan & Uzun (2023). No separate machine learning model is used for gender classification.

Formula:
Shape Index (SI) = Short Axis / Long Axis

If SI > 0.50 → Likely Female
If SI ≤ 0.50 → Likely Male

Measurements can be taken automatically using LiDAR or entered manually by the user.

––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––

Getting Started

Requirements:

macOS with Xcode 15 or later
iPhone Pro model with LiDAR (e.g., iPhone 13 Pro, 14 Pro, 15 Pro)
Instructions:

Clone the repository
git clone https://github.com/H-Shahriar/EggVision.git
Open the project in Xcode
Connect your LiDAR-enabled iPhone and run the app
––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––

Screenshots

Home Screen

screenshots/home.png
Egg Classification Result

screenshots/type-classification.png
LiDAR Scan in Progress

screenshots/lidar-scan.png
Gender Prediction Output

screenshots/gender-result.png
(If you want to add screenshots, please name and organize them inside a /screenshots folder in the repo.)

––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––

Tech Stack

Swift / SwiftUI
CoreML for egg type classification
ARKit + SceneKit for LiDAR scanning
Custom rule-based gender prediction system
––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––

Credits
Developed by Hasan Shahriar
Sponsored by Harmony Harvesty Farm
Capstone Project – University of Canberra, 2025
Based on the research: Kayadan & Uzun (2023)
