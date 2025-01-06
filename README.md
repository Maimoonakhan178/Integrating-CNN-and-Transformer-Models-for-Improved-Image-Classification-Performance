# Skin Cancer Classification Using Ham10000 Dataset

## Overview  
This project focuses on classifying skin cancer using the [Ham10000 dataset](https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000). The dataset contains 7 classes of skin lesions with highly imbalanced distributions. To address this, we implemented data preprocessing strategies to ensure balanced class representation, avoiding overfitting and bias.

## Dataset  
The Ham10000 dataset consists of over 10,000 dermoscopic images categorized into 7 classes. The dataset's imbalance posed a significant challenge:
- Some classes had more than 2,000–3,000 images.
- Others had only 100–200 images.

### Balancing Strategy  
To address the class imbalance:  
1. **Threshold**: Set at 500 images per class.  
2. **Downsampling**: Classes with more than 500 images were downsampled to the threshold.  
3. **Augmentation**: Classes with fewer than 500 images were augmented using techniques such as rotation, flipping, and scaling to reach the threshold.  

These methods ensured balanced class distributions, reducing overfitting and bias.

---

## Hybrid Model Architecture  
The model leverages a **ResNet-Transformer Hybrid** architecture to achieve state-of-the-art results:  
- **ResNet**: Efficient local pattern detection, crucial for identifying subtle features in medical images.  
- **Transformer**: Global dependency modeling, capturing relationships between features for robust classification.  

This hybrid architecture enhances both accuracy and feature representation, making it particularly effective in complex tasks like medical imaging.

---

## Results  
The following results were achieved on the Ham10000 dataset:  
1. **ResNet + Transformer (Hybrid Model)**:  
   - **Accuracy**: 98%  
   - **Key Strengths**: Superior feature representation and robust performance.  

2. **Benchmark FixCap Model**:  
   - **Accuracy**: 96%  

The hybrid model demonstrates the potential of combining architectural strengths for medical image classification.

---

## Key Insights  
- Balancing the dataset through a mix of downsampling and augmentation mitigated class imbalance and enhanced model generalization.  
- Combining ResNet’s local pattern detection with Transformer’s global dependency modeling significantly improved classification accuracy.  
- Collaborative architectures represent the future of deep learning, particularly in domains requiring high precision, like medical imaging.

---


