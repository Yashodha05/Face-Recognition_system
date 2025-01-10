# Face Recognition Project

This project implements a real-time face recognition system using a pre-trained model created with **Google Teachable Machine**, integrated with **TensorFlow** and **OpenCV** for live webcam input. The model predicts the identity of a person in the webcam feed and outputs the confidence score of the prediction.

## **About the Model**

The face recognition model (`k1.h5`) was trained using Google Teachable Machine, a user-friendly platform for creating machine learning models without deep technical expertise. Here's how the model was created and used:

1. **Data Collection**:
   - Images of 2 individuals  were captured and uploaded to Google Teachable Machine.
   - Each class corresponds to a unique individual category.

2. **Training**:
   - The model was trained to classify images into 2 categories:
     - Individual 1
     - Individual 2
   - The training process used a convolutional neural network (CNN) architecture for feature extraction and classification.
     

3. **Output**:
   - The trained model was exported as `keras.h5`, a Keras-compatible file format.
   - Labels for the categories were saved in `labels.txt`.

## **Features**
- **Real-Time Face Recognition**: Identifies faces captured through a webcam.
- **Confidence Score**: Displays the confidence percentage of the prediction for each class.
- **User-Friendly**: Designed to be accessible for beginners in machine learning and computer vision.

## **How It Works**

1. **Input Data**:
   - Captures live webcam frames using **OpenCV**.
   - Each frame is resized to `224x224` pixels to match the input dimensions of the model.

2. **Preprocessing**:
   - The image is normalized to a range of `[-1, 1]` for compatibility with the trained model.

3. **Prediction**:
   - The preprocessed image is passed to the TensorFlow model.
   - The model predicts the class (identity) with the highest confidence score.

4. **Output**:
   - The predicted class and confidence score are displayed on the console.
   - The live webcam feed is displayed in a separate window.

**Technical Requirements**

 **Dependencies**
- **TensorFlow**: For loading and using the pre-trained model.
- **OpenCV**: For capturing webcam images in real time.
- **NumPy**: For handling image data as arrays.
  
- **Install these dependencies via the provided `requirements.txt` file:**
- ```bash
pip install -r requirements.txt

- **Installation Guide:**

**Step 1: Clone the Repository**
git clone https://github.com/your-username/internship-projects.git
cd internship-projects

## How to Use This Project
1. Download the ZIP file.
2. Extract the contents.
3. Follow these instructions to run the project.

**Google Teachable Machine**

1.Search for Google teachable machine

![Screenshot (20)](https://github.com/user-attachments/assets/6828381b-0160-4959-93e8-a6cbbf42d98a)
2. click on the particular link.

![Screenshot (21)](https://github.com/user-attachments/assets/c3e1fcdd-12f4-46e6-beb6-e9e88c2540d8)


**Step 2: Install Dependencies**
pip install -r requirements.txt

**Step 3: Run the Script**
Ensure your webcam is connected.
Execute the Python script:
bash
Copy code
python main.py
The webcam feed will open in a new window. The predicted class and confidence score will appear in the terminal.
Press the Esc key to exit.

**Model Details**
Model File: k1.h5

Format: TensorFlow's Keras model.
Input Dimensions: (224, 224, 3) (Height, Width, RGB Channels).
Classes: 2  individuals .
Labels File: labels1.txt

Contains the names of the classes.

**Contact**
If you have any questions or suggestions, feel free to reach out via GitHub issues.
---

### **How to Use This README**

1. Copy the above content into your `README.md` file.
2. Replace `https://github.com/your-username/internship-projects.git` with the actual link to your GitHub repository.
3. Save the file and upload it to your repository.

This README provides a comprehensive explanation of your project and will be helpful for beginners or anyone interested in using or extending your work. Let me know if you need further tweaks!
**
  

