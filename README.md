# Comparative Analysis of Several Deep Learning CNN Architecture Models in Identifying Types and Health of Coral Reefs

This repository contains the documentation and code for my thesis on the comparative analysis of several deep learning CNN architectures (MobileNetV2, DenseNet, ResNet-152, and VGG19) in identifying the types and health levels of coral reefs. The goal of this research is to develop a classification system for coral reef types and health levels using deep learning techniques.

## Repository Structure
```
/Code # Jupyter notebooks for data preprocessing, training, and testing
/Predict Code # Code to test the model with sample image
README.md # This file
```
## Dataset

The dataset used in this study consists of 507 images for coral reef type classification and 520 images for coral reef health level classification. The images were collected from various sources, including:

- StructuredRMAS database
- Kaggle
- Google Images
- Direct capture in coral reef habitats (Thousand Islands)

The dataset is divided into training and testing sets with a ratio of 80:20.

## Methodology

The study employs several deep learning CNN architectures, including MobileNetV2, DenseNet, ResNet-152, and VGG19. The models were trained to classify coral reef types (Boulder, Branching, and Table) and health levels (Level 1 to Level 6).

### Data Preprocessing
- Images were resized and normalized.
- Data augmentation techniques were applied to increase the diversity of the training data.

### Model Training
- The models were trained using the Adam optimizer with a learning rate of 0.001.
- Training was conducted for 20 epochs with a batch size of 8.

### Evaluation Metrics
- Accuracy, Precision, Recall, and F1-Score were used to evaluate the models.

## Results

The best accuracy for coral reef type classification was achieved using the DenseNet architecture with an accuracy of 100%. For coral reef health level classification, the DenseNet architecture also achieved the highest accuracy of 55%.

| Model       | Coral Reef Type Accuracy | Coral Reef Health Level Accuracy | Training Time per Epoch |
|-------------|--------------------------|----------------------------------|-------------------------|
| MobileNetV2 | 98%                      | 26%                              | 5 seconds               |
| DenseNet    | 100%                     | 55%                              | 13 seconds              |
| ResNet-152  | 66%                      | 22%                              | 12 seconds              |
| VGG19       | 81%                      | 24%                              | 24 seconds              |

## Conclusion

The DenseNet architecture performed the best in both coral reef type and health level classification tasks. However, the accuracy for health level classification was lower due to the limited amount of data and lack of variation. Future work could focus on increasing the dataset size and applying more advanced data augmentation techniques.

## Contact

For any inquiries, please contact [Muhammad Aidan Daffa J](mailto:Muhammad.aidan@ui.ac.id).
