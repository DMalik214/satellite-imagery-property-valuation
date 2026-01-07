# Satellite Imagery-Based Property Valuation

## Overview
In this project, i created a complete multimodal regression model to estimate house prices. This model uses a mix of housing attributes and satellite images.

The goal is to improve traditional real estate valuation models by including environmental and neighborhood features such as road connectivity, space density, and greenery.

Unlike standard regression models, this project incorporates computer vision, gradient boosting, and interpretability methods together.

---
## Key Concepts
- Good Tabular Baseline performance using XG
- Satellite imagery accessed through latitude and longitude coordinates
- CNN embeddings (ResNet-50) to capture the visual patterns of neighborhoods
- Residual multimodal fusion prevents strong tabular signals from degrading
- Grad-CAM Explanability Method for visualizing how the model learns from images

---
## System Architecture
The final system replaces simple feature fusion with residual learning:
- XGBoost predicts the basic property price based on tabular data.

In summary, a multimodal neural network learns residual errors using:
- Tabular features
- Satellite image embeddings
- Final prediction = Base Prediction + Learned Residue 

This approach ensures that visual cues support, rather than dominate, structured predictors. 

Architecture Diagram: 
please open the link to see it.
<img width="3869" height="4735" alt="Untitled diagram-2026-01-07-092517" src="https://github.com/user-attachments/assets/c0100086-f6c8-48f1-89ef-ceacbd3d4457" />

Model Evaluation Metrics:
please open the link to see it.
<img width="3989" height="2785" alt="Untitled diagram-2026-01-07-093116" src="https://github.com/user-attachments/assets/32088c8c-02ad-4278-a785-3f29473f0b80" />
