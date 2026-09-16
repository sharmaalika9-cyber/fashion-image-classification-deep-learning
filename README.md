# Fashion Image Classification using Deep Learning

A Deep Learning-based image classification project that automatically identifies fashion product categories from images. The project demonstrates how an Artificial Neural Network can support product categorization in an e-commerce environment.

## 📌 Project Overview

E-commerce companies receive a large number of product images that need to be categorized before products are added to their websites.

This project uses a Deep Learning model to classify fashion product images into **10 different categories**. The model is trained using the **Fashion MNIST** dataset and implemented with **TensorFlow/Keras**.

The project also demonstrates how AI-assisted image classification can reduce repetitive manual categorization work and support faster product listing.

## 🎯 Objectives

* Understand how images can be used as input for Deep Learning.
* Build a simple Artificial Neural Network.
* Train the model on fashion product images.
* Evaluate model performance using test accuracy.
* Predict the category of unseen product images.
* Understand the business application of image classification.

## 🛠️ Tech Stack

* **Python**
* **TensorFlow / Keras**
* **NumPy**
* **Matplotlib**
* **Google Colab**
* **Fashion MNIST**

## 📊 Dataset

The project uses the **Fashion MNIST** dataset.

The dataset contains grayscale images of fashion products belonging to 10 categories:

1. T-shirt / Top
2. Trouser
3. Pullover
4. Dress
5. Coat
6. Sandal
7. Shirt
8. Sneaker
9. Bag
10. Ankle Boot

The images are prepared by scaling pixel values from **0–255 to 0–1** before training.

## 🧠 Model Architecture

The project uses a simple neural network with the following structure:

```text
Input Image
     ↓
Flatten Layer
     ↓
Dense Layer (64 neurons + ReLU)
     ↓
Output Layer (10 neurons + Softmax)
```

The final output layer contains 10 outputs because the model predicts one of the 10 fashion categories.

## 🔄 Project Workflow

```text
Fashion MNIST Dataset
        ↓
Load Images
        ↓
Explore Product Images
        ↓
Normalize Pixel Values
        ↓
Build Neural Network
        ↓
Compile Model
        ↓
Train Model
        ↓
Evaluate Test Accuracy
        ↓
Predict Product Category
        ↓
Business Interpretation
```

## ⚙️ Model Training

The model is compiled using:

* **Optimizer:** Adam
* **Loss Function:** Sparse Categorical Crossentropy
* **Metric:** Accuracy
* **Epochs:** 3
* **Validation Split:** 10%

The notebook uses three epochs to keep the classroom demonstration relatively quick.

## 📈 Evaluation

The model is evaluated using previously unseen test images.

The notebook calculates test accuracy using the model's predictions on the test dataset.

> Note: The exact accuracy can vary depending on the training run.

Accuracy alone should not be the only consideration when deploying an image-classification system. Incorrect classifications, customer experience, training-data quality, and human review should also be considered.

## 🔮 Prediction

After training, the model can predict the category of an unseen fashion image.

The project compares:

```text
Predicted Product → Model's prediction
Actual Product    → True category
```

This allows the model's classification performance to be visually inspected.

## 💼 Business Use Case

### Traditional Process

```text
Product Image
     ↓
Employee manually selects category
     ↓
Product added to website
```

### AI-Assisted Process

```text
Product Image
     ↓
Deep Learning Model
     ↓
Predicted Product Category
     ↓
Employee Review (if required)
     ↓
Product added to website
```

### Potential Business Benefits

* Faster product listing
* Reduced repetitive manual work
* More consistent product categorization
* Improved product-search experience
* Ability to process larger volumes of product images

## ⚠️ Limitations

This project uses a relatively simple neural network and the Fashion MNIST dataset. Real-world e-commerce images can be more complex because of different backgrounds, lighting conditions, camera angles, product variations, and image quality.

Therefore, additional validation and human oversight would be required before using such a system in a production environment.

## 📁 Project Structure

```text
fashion-image-classification-deep-learning/
│
├── Deep_Learning_Fashion_Classification_Name.ipynb
├── README.md
│
└── screenshots/
    └── prediction-result.png
```

The course notebook suggests placing the project under:

```text
part-a/deep-learning/
```

## 🚀 How to Run

### Option 1: Google Colab

1. Open the `.ipynb` notebook in Google Colab.
2. Run the cells sequentially.
3. The Fashion MNIST dataset will download automatically.
4. Train the model.
5. Evaluate the test accuracy.
6. Test different image numbers to view predictions.

### Option 2: Local Environment

Install the required libraries:

```bash
pip install tensorflow numpy matplotlib
```

Then open the notebook using Jupyter Notebook or JupyterLab.

## 📸 Project Output

The project generates visual outputs showing:

* Fashion product images
* Predicted product category
* Actual product category
* Model evaluation results

## 🎓 Academic Context

This project was developed as a Deep Learning practical for understanding the application of Artificial Neural Networks to image classification and connecting AI concepts with an e-commerce business scenario.

## 🔑 Key Learnings

* Deep Learning can learn patterns from images.
* Neural networks contain input, hidden, and output stages.
* Training allows a model to learn from labelled examples.
* Testing evaluates performance on unseen data.
* A trained model can predict new image categories.
* AI predictions should be evaluated with business risks and human oversight in mind.

## 👤 Author

**Your Name**

BBA FinTech & AI
Chitkara University

---

⭐ If you found this project useful, consider giving the repository a star.
