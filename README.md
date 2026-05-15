# Part 2: CNN-Based Computer Vision Project

##  Problem Statement
This project focuses on building a Convolutional Neural Network (CNN) for image classification.  
The dataset contains images of surface conditions and defects such as:

- Dent
- Scratch
- Stain
- Normal

The goal is to automatically classify each image into one of these categories.

---

##  Problem Type
**Image Classification**

Each image belongs to exactly one class, so this is a classification problem.  
There are no bounding boxes or pixel-level annotations, so it is NOT object detection or segmentation.

---

##  Dataset Description
The dataset consists of:
- Images grouped into folders:
  - dent/
  - scratch/
  - stain/
  - normal/
- A `labels.csv` file mapping image filenames to their classes

---

##  Dataset Exploration
- Number of classes: 4
- Classes: dent, scratch, stain, normal
- Images per class analyzed using value counts
- Sample images visualized
- Image dimensions checked
- Dataset imbalance analyzed

---

##  Image Preprocessing
The following preprocessing steps were applied:

- Resizing all images to 128×128 pixels
- Normalizing pixel values (0–1 range)
- Label encoding of class names
- Train-test split (80/20)
- Data augmentation (rotation, zoom, horizontal flip)

---

##  CNN Model Architecture

The model includes:

- Convolution Layer (feature extraction)
- ReLU Activation (non-linearity)
- Max Pooling Layer (dimension reduction)
- Flatten Layer (convert to vector)
- Dense Layer (learning patterns)
- Output Layer (Softmax for classification)

---

##  Model Training & Evaluation
The model was trained using TensorFlow/Keras.

### Results include:
- Training accuracy & loss
- Validation accuracy & loss
- Test accuracy
- Confusion matrix
- Sample predictions

---

##  CNN Concepts Explained

###  Convolution
Extracts features like edges, textures, and shapes from images.

###  Pooling
Reduces image size while keeping important information.

###  ReLU
Introduces non-linearity and improves learning efficiency.

###  Why CNN?
CNNs are designed for image data and automatically learn spatial features better than traditional neural networks.

---

##  Business Use Case
This model can be used in **manufacturing industries** for automated defect detection.

It helps to:
- Detect defective products
- Reduce manual inspection
- Improve quality control
- Save time and cost

---

##  Technologies Used
- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Seaborn