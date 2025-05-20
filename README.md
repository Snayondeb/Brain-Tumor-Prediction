# Brain-Tumor-Prediction
A deep learning project on Brain Tumor Prediction using Convolutional Neural Networks (CNNs) — achieving a model accuracy of 96.77% on MRI image classification. 



## 🧠 **Theory of CNN and Its Application in Brain Tumor Prediction**

### 🔍 What is a Convolutional Neural Network (CNN)?

A **Convolutional Neural Network (CNN)** is a type of deep learning model specifically designed to work with **grid-like data**, such as images. It is highly effective in **image recognition, classification, and medical imaging tasks** due to its ability to automatically and adaptively learn spatial hierarchies of features.

---

### 📐 **Key Layers in CNN:**

1. **Input Layer**
   Takes in the image data (e.g., 224x224x3 for colored images).

2. **Convolutional Layer**
   Applies multiple **filters** (kernels) that slide over the image and capture important features like edges, textures, or patterns.

3. **Activation Layer (ReLU)**
   Introduces non-linearity to help the network learn complex patterns.

4. **Pooling Layer (MaxPooling)**
   Downsamples feature maps to reduce dimensionality and computational load while retaining essential features.

5. **Flatten Layer**
   Converts 2D feature maps into a 1D vector before feeding into fully connected layers.

6. **Fully Connected (Dense) Layers**
   Perform final decision-making by combining all the learned features.

7. **Output Layer**
   Uses **sigmoid** (for binary classification) or **softmax** (for multi-class classification) to output prediction probabilities.

---

### 🧬 **How CNN is Used in Brain Tumor Prediction**

The task of **brain tumor detection** from MRI images can be seen as a **binary classification problem** — predicting whether an image shows a tumor or not.

#### ✅ **Step-by-Step Workflow:**

1. **Dataset Collection**

   * MRI images of brains with and without tumors.
   * In your case, sourced from **Navoneel Chakrabarty**.

2. **Data Preprocessing**

   * Resize all images to a standard size (e.g., 224x224).
   * Normalize pixel values (e.g., using `preprocess_input()`).
   * Augment data (rotation, flipping) to improve generalization.

3. **Model Construction**

   * Use a CNN or a pretrained model like **MobileNet**, **ResNet**, etc.
   * Layers automatically extract low-level to high-level features from MRI scans.

4. **Training**

   * Feed MRI images into the model.
   * The CNN learns to distinguish tumor vs no-tumor patterns based on labeled data.

5. **Validation & Testing**

   * Evaluate model on unseen images to check generalization.
   * In your case, the model achieved **96.77% accuracy**.

6. **Prediction**

   * Input a new MRI image, and the model predicts "Yes Tumor" or "No Tumor" with high confidence.
   * Your model is giving **100% correct prediction responses** for both classes in test samples.

---

📌 Why CNN is Effective for Medical Imaging:

* **Automatic Feature Extraction**: No need for manual diagnosis or handcrafted features.
* **Robust to Noise and Variations**: Learns essential patterns even with diverse image conditions.
* **Scalable**: Works efficiently on large datasets and real-world images.

---

### 🧠 Real-World Impact:

Brain tumor detection using CNNs can **support radiologists** by providing a second opinion, **reduce diagnosis time**, and **improve accuracy** — especially in regions with limited medical infrastructure.


