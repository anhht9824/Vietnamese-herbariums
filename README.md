# Vietnamese herbariums Species Classification with EfficientNetV2

---

## Keywords

`EfficientNetV2` `Vietnamese herbariums`  `Biological characteristics`

---
Abstract
In recent years, the field of traditional medicine in Vietnam has been growing rapidly. Classifying herbariums has become crucial for both preservation and research purposes. However, traditional methods for herbarium classification require extensive domain knowledge, which limits accessibility for the general public. To address this challenge, we developed a deep learning model based on the EfficientNetV2 architecture, achieving a classification accuracy of 90.41%.

EfficientNetV2 was selected due to its balance between high performance and accuracy, and its ability to handle images of various sizes while minimizing overfitting. Although challenges such as herbarium species diversity and image quality remain, our experiments demonstrate that this model offers superior performance compared to traditional methods, paving the way for future improvements in herbarium classification.

Methodology
The project applies EfficientNetV2, a CNN model that provides both scalability and high accuracy through its innovative use of Fused-MBConv blocks. We used Adam optimization to adjust the model's parameters and data augmentation to further improve the model’s robustness.

Model Details:
Architecture: EfficientNetV2 with Fused-MBConv blocks
Learning Rate: 5 × 10^-4 (with minimum 1 × 10^-6)
Epochs: 50 (early stopping applied)
Batch Size: 32
Dropout Rate: 0.3
Optimization Algorithm: Adam
Training Process:
We froze the first 100 layers of the pre-trained EfficientNetV2 and applied fine-tuning to the remaining layers, boosting the accuracy from 90.41% to 90.64%.
Data augmentation techniques, including resizing and centercropping, were applied to ensure better generalization of the model.
Results
The model achieved 90.41% accuracy on the test set. While the accuracy was slightly improved by fine-tuning all layers, we found that freezing the initial layers led to a more efficient training process with marginal impact on accuracy.

Comparisons with ResNet50 and Xception models demonstrated the superior performance of EfficientNetV2 in classifying Vietnamese herbariums.

Model	Accuracy
EfficientNetV2	90.41%
ResNet50	88.32%
Xception	87.55%
Dataset
The dataset consists of images of Vietnamese herbariums, annotated with their corresponding genus and species. We filtered out species with fewer than 50 images to ensure sufficient data for each class. Data augmentation techniques were applied to increase the variability of the dataset.

Challenges
Diversity of Species: The dataset includes herbarium species with highly similar morphological characteristics, making classification difficult.
Image Quality: The quality and resolution of some images vary, which may impact classification performance.
Limited Data: Certain species have a limited number of available images, restricting the model’s ability to generalize.
Future Work
In future iterations of this project, we plan to:

Improve pre-processing techniques to enhance image quality and diversity.
Experiment with more advanced classification models and techniques to further increase accuracy.
Expand the dataset to include more species with a larger number of samples.
Explore alternative architectures and hyperparameter optimization strategies for improved performance.
## Contact

For any information, please contact the main author:

**Tuan Anh Hoang** at **FPT University, Vietnam**

- **Email**: anhhtse180113@fpt.edu.vn
- **GitHub**: [https://github.com/anhht9824](https://github.com/anhht9824)
