# Ulcer detection in WCE Images Using Convolution Neural Networks
## Reference 
This project is based on the research article: [Ulcer Detection in Wireless Capsule Endoscopy Images Using Deep CNN](https://www.researchgate.net/publication/344603682_Ulcer_detection_in_Wireless_Capsule_Endoscopy_images_using_deep_CNN)

## Overview 
Ulcer is one of the common abnormalities present in the
GastroIntestinal (GI) tract. Ulcers affect approximately 10%
of the people in the world. They are erosions in the mucosal
lining and may occur along the GI-tract.

However, traditional endoscopy techniques are quite painful
to the patient as well as endoscopy methods cannot visualize
the area of small intestine in the GI tract. Over the last decade,
Wireless Capsule Endoscopy (WCE) introduced has become
an irreplaceable tool for diagnosis of Gastro Intestinal (GI)
tract.

### What is WCE?
Wireless Capsule Endoscopy (WCE) involves a pill-sized capsule that the patient swallows. This capsule captures color images of the entire GI tract for about 8 hours. Doctors then download these 45,000–50,000 images per patient and examine the frames, a process that can take 3-4 hours. Frames with abnormalities may only comprise 5–7% of the total, making manual diagnosis time-consuming and tedious.

Previous works on ulcer detection have primarily focused on traditional endoscopy images using image processing and segmentation techniques. However, limited research exists on ulcer detection using WCE images. This project aims to address this gap using a deep Convolutional Neural Network (CNN) approach.

## Methodology
The proposed architecture employs four convolutional layers with average pooling, ReLU activation, and two dense layers to enhance the efficiency of ulcer recognition in WCE images. A large database of various types of ulcers in WCE images was used to explore the effectiveness of this method.

![image](https://github.com/DEVY4NSH/UlcerDetectionModel/assets/101127637/fe7b20a9-c028-4a52-b881-e68b2a5287ff)

### Architecture Details
- **First Convolutional Layer:** 32 kernels (3x3), followed by average pooling (2x2) and a dropout layer (0.5).
- **Second Convolutional Layer:** 64 kernels (3x3), followed by average pooling (2x2) and a dropout layer (0.5).
- **Third Convolutional Layer:** 128 kernels (3x3), followed by average pooling (2x2) and a dropout layer (0.5).
- **Fourth Convolutional Layer:** 256 kernels (3x3), followed by average pooling (2x2) and a dropout layer (0.5).
- **Fully Connected Layer:** 128 hidden units with a dropout of 0.5.
- **Output Layer:** A final dense layer with 2 units for binary classification.

The fully connected layer converts the high-level representation of the 2D feature map into a 1D feature map, aiding in the binary classification task.


## Performance Metrics
To validate the model's performance, the following metrics were used:

- **Precision:** 87.6%
- **Recall (Sensitivity):** 86.0%
- **Specificity:** 87.8%
- **F1 Score:** 86.7%


## Confusion Matrix Definitions
- **True Positive (TP):** Correctly predicted positive (ulcer).
- **True Negative (TN):** Correctly predicted negative (non-ulcer).
- **False Positive (FP):** Incorrectly predicted positive (ulcer). 
- **False Negative (FN):** Incorrectly predicted negative (non-ulcer).


## Installation and Usage
To set up the project locally, follow these steps:
- **Clone the repository:**
  git clone "https://github.com/DEVY4NSH/UlcerDetectionModel.git"
  cd UlcerDetectionModel






