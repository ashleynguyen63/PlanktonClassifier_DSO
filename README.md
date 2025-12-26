# Plankton Classifier with Metadata Integration

## Contributors
Ashley Nguyen, Christopher Kverne, Emily Hong, Ethan Feldman, Lorraine Yang


## Overview
This project develops a machine learning pipeline to classify plankton species from imaging data. Unlike traditional image-only models, this classifier leverages **environmental metadata** (e.g., water temperature, salinity, wind speed, etc.) to improve accuracy. Metadata is incorporated through a **Feature-wise Linear Modulation (FiLM) conditioning layer**, which conditions image features based on contextual environmental variables.  

The dataset comes from the **Woods Hole Oceanographic Institution (WHOI)** and the **Martha’s Vineyard Coastal Observatory (MVCO)**. By combining image and environmental information, the model achieves improved classification performance, particularly for visually similar plankton species.

---

## Features
- Image classification of plankton samples using various models including Res-Net **TensorFlow/Keras**  
- Integration of environmental metadata via a **FiLM conditioning layer**  
- Metadata-aware classification that improves ecological context sensitivity  
- Data pipeline for handling binary image bytes and tabular metadata in Parquet format  
- Evaluation metrics including accuracy, per-class precision/recall, and confusion matrices  
- GPU-enabled training for efficient large-scale classification  
- **Pretrained model weights available upon request**

---

## Results
- 99% classification accuracy for classes over 100
- 85% drop in missclassified images as opposed to the non-conditioned Res-Net model
