# Image-Forgery-Detection
The methodology employed in this study aims to develop an image forgery detection model
using machine learning techniques. The study uses a dataset of manipulated images that includes
a variety of image forgery techniques such as copy-move, splicing, and removal. The dataset is
divided into training and testing sets for model development and evaluation, respectively.
1. Data Preprocessing: The first step in the methodology is data preprocessing, which
involves converting the input images into a suitable format that can be used for training
and testing the machine learning models. The input images are converted to grayscale and
resized to a fixed size to ensure that all images have the same dimensions.
2. Feature Extraction: The next step is feature extraction, which involves extracting
meaningful features from the input images that can be used to distinguish between
genuine and forged images. The code uses two feature extraction techniques: Local
Binary Patterns (LBP) and Gray-Level Co-occurrence Matrix (GLCM).
2.1. LBP: Local Binary Patterns is a texture descriptor that extracts local texture
patterns from an image. It defines a local neighbourhood around each pixel and
calculates a binary pattern based on the pixel intensities in the neighbourhood.
2.2. GLCM: Gray-Level Co-occurrence Matrix is a statistical method that analyzes the
spatial relationships between pixels in an image. It calculates the frequency of
occurrence of pairs of pixel intensities at a given distance and direction.
3. Model Training: The extracted features are used to train three different machine learning
models: Support Vector Machine (SVM), Random Forest Classifier (RFC), and
Convolutional Neural Network (CNN).
3.1. SVM: The Support Vector Machine is a supervised learning algorithm used for
classification and regression analysis. It separates data points into different classes
by finding a hyperplane that maximally separates the classes in the feature space.
3.2. RFC: The Random Forest Classifier is an ensemble learning algorithm that creates
a set of decision trees and combines them to make a final prediction. It uses
bootstrap aggregating (bagging) to randomly sample the data and features and
averages the predictions of multiple decision trees to improve accuracy.
3.3. CNN: The Convolutional Neural Network is a deep learning architecture that is
specifically designed for image analysis. It consists of multiple layers, including
convolutional layers, pooling layers, and fully connected layers. The network
learns to extract features from the input images and uses these features to classify
the images.
4. Model Evaluation: Once the models are trained, they are evaluated using two metrics:
accuracy and F1-score. Accuracy measures the percentage of correctly classified images,
while the F1 score measures the balance between precision and recall.
5. Ensemble Learning: Finally, the predictions of the three models are combined using an
ensemble learning approach to improve overall accuracy. The final prediction is based on
a weighted average of the predictions of the individual models.
