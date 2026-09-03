🐱🐶 Cat vs Dog Image Classification using CNN
📌 Project Overview

This is a personal Deep Learning project created to gain hands-on experience with Convolutional Neural Networks (CNNs) and image classification.

The goal of the project is to build a CNN model that can classify an input image as either a Cat or a Dog.

This project was developed as part of my self-learning journey in Deep Learning, Computer Vision, TensorFlow, and Keras.

🎯 Objectives
Understand the basic workflow of an image classification problem
Practice image preprocessing and dataset preparation
Build a CNN model using TensorFlow/Keras
Train and validate the model
Evaluate the model on unseen test data
Make predictions on new images
Visualize training and validation performance
🗂️ Dataset

The dataset contains images belonging to two classes:

🐱 Cats
🐶 Dogs

The dataset is organized into separate training and testing directories.

For training, the training dataset is further divided into:

80% Training data
20% Validation data

The images are resized to 128 × 128 pixels before being fed into the CNN.

Note: The dataset is not included in this repository because of its size. Please download the dataset separately and place it in the expected folder structure.

🧠 CNN Architecture

The CNN model was built using TensorFlow/Keras.

The architecture consists of:

Input Image (128 × 128 × 3)
          ↓
Rescaling (1/255)
          ↓
Conv2D (32 filters)
          ↓
MaxPooling
          ↓
Conv2D (64 filters)
          ↓
MaxPooling
          ↓
Conv2D (128 filters)
          ↓
MaxPooling
          ↓
Flatten
          ↓
Dense (128 neurons)
          ↓
Dense (2 neurons)
          ↓
Softmax
Model Configuration
Optimizer: Adam
Loss Function: Sparse Categorical Crossentropy
Evaluation Metric: Accuracy
Image Size: 128 × 128
Batch Size: 32
Epochs: 6

🔍 Prediction
After training, the model was tested on a new image that was not used during training.

The model provides:
Predicted class
Prediction confidence

Example:
Predicted animal: dogs
Confidence: 57.94906%

📊 Model Evaluation
The model was evaluated using the separate test dataset.

Test Results
Metric	Result
Test Accuracy	Add your result
Test Loss	Add your result

The notebook also includes visualizations of:
Training vs Validation Accuracy
Training vs Validation Loss
📈 Visualizations

The project includes:
Random sample images from the dataset
Training and validation accuracy curves
Training and validation loss curves
Prediction on a new image

These visualizations helped me understand how the model performed during training and how well it generalized to unseen data.

🛠️ Technologies Used
Python
TensorFlow
Keras
NumPy
Matplotlib
Jupyter Notebook
VS Code

📁 Project Structure
cat-vs-dog-cnn/
│
├── cat_vs_dog_cnn.ipynb
├── requirements.txt
├── README.md
│
└── dataset/
    ├── training_set/
    │   └── training_set/
    │       ├── cats/
    │       └── dogs/
    │
    └── test_set/
        └── test_set/
            ├── cats/
            └── dogs/

The dataset folder is excluded from the GitHub repository because of its size.

▶️ How to Run the Project
1. Clone the repository
git clone <your-github-repository-url>
2. Create a virtual environment
python -m venv venv
3. Activate the virtual environment

Windows:
venv\Scripts\activate
4. Install the required libraries
pip install -r requirements.txt
5. Add the dataset

Download the Cat vs Dog dataset and place it according to the folder structure described above.

6. Run the notebook
Open:

cat_vs_dog_cnn.ipynb
in VS Code and run the cells sequentially.

💡 Key Learnings

Through this project, I gained practical experience with:

Loading image datasets using image_dataset_from_directory()
Image resizing and normalization
Creating CNN architectures
Convolution and pooling operations
Training and validation
Model evaluation
Making predictions on unseen images
Interpreting accuracy and loss curves

Most importantly, this project helped me move from understanding CNN concepts theoretically to implementing an end-to-end image classification model.

🚀 Future Improvements
Some possible improvements for future versions include:

Data augmentation
Dropout and regularization
Hyperparameter tuning
Increasing the number of training epochs
Transfer learning using pretrained CNN models
Comparing the custom CNN with models such as MobileNet or VGG

👩‍💻 About This Project
This project is part of my personal learning journey as I continue building practical projects in Machine Learning and Deep Learning.

Thank You!
