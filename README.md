# Face Recognition Project

This project implements a real-time face recognition system using a pre-trained model created with Google Teachable Machine, integrated with TensorFlow and OpenCV for live webcam input. The model predicts the identity of a person in the webcam feed and outputs the confidence score of the prediction.

## **About the Model**

The face recognition model (keras.h5) was trained using Google Teachable Machine, a user-friendly platform for creating machine learning models without deep technical expertise. Here’s how the model was created and used:

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

- **Installation Guide:**

**Step 1: Clone the Repository**

git clone https://github.com/your-username/Face-Recognition_system.git
cd Face-Recognition_system

**Step 2: Install Dependencies**

Make sure Python is installed on your system. To install the required Python libraries, open the python terminal and run:

pip install -r requirements.txt

**## How to Use This Project**

**1.Download the Required Files:**

Clone the repository as explained above.
Ensure you have the keras.h5 model and labels.txt files in the project directory.

**2.Set Up Google Teachable Machine:**

1.Visit Google Teachable Machine.

![Screenshot (20)](https://github.com/user-attachments/assets/6828381b-0160-4959-93e8-a6cbbf42d98a)

2. click on the particular link.

![Screenshot (21)](https://github.com/user-attachments/assets/c3e1fcdd-12f4-46e6-beb6-e9e88c2540d8)

3. Click on New Image Project.

![Screenshot (22)](https://github.com/user-attachments/assets/c92d6321-aebe-4fcd-ad2f-f3109661f336)

4. Add samples for each class (e.g., Individual 1 and Individual 2).

![Screenshot (23)](https://github.com/user-attachments/assets/7437bcd4-3d88-4daa-ae33-d69b1922f314)

5.Train the model and Export the trained model as a .h5 file.

<img width="615" alt="image" src="https://github.com/user-attachments/assets/45c22669-5e37-4898-bb06-3d914b50446e" />

6.Download the model and save it in your project directory.

<img width="634" alt="image" src="https://github.com/user-attachments/assets/033643a3-97f6-45f4-8fe6-b36a744f0956" />


**Step 2: Install Dependencies**

pip install -r requirements.txt

**Step 3: Run the Script**

Ensure your webcam is connected.

<img width="197" alt="image" src="https://github.com/user-attachments/assets/9930948c-f5d1-4073-9e9d-3e1a5a32c85a" />

Execute the Python script:
bash
Copy code
python main.py

<img width="955" alt="image" src="https://github.com/user-attachments/assets/89ff0f5f-5682-44d8-9f2c-9d970c1c8a83" />

The webcam feed will open in a new window. The predicted class and confidence score will appear in the terminal.

Press the Esc key to exit.

<img width="956" alt="image" src="https://github.com/user-attachments/assets/1f668b05-5983-4707-a7d6-c83d52e4a6bd" />


**Output of the model**

The model will display live webcam footage and overlay the predicted class with its confidence score in real time.
Example Output:


<img width="350" alt="image" src="https://github.com/user-attachments/assets/ba656742-3cd8-40ba-a3b3-992cfe62906a" />

**Model Details:**

**1.Model File:** k1.h5

**2.Format:** TensorFlow's Keras model.

**3.Input Dimensions:** (224, 224, 3) (Height, Width, RGB Channels).

**4.Classes:** 2 individuals.

**5.Labels File:** labels1.txt
   -Contains the names of the classes.

**Troubleshooting Guide**

**1.Issue:** Webcam feed not displaying.

**Solution:** Ensure your webcam is connected and not being used by another application.

**2.Issue:** Missing dependencies.

**Solution:** Run pip install -r requirements.txt again to install all required libraries.

**3.Issue:** Low confidence scores.

**Solution:** Re-train the model with more diverse images for better accuracy.


**Contact**
If you have any questions or suggestions, feel free to reach out via GitHub issues.
---

### **How to Use This README**

1. Copy the above content into your `README.md` file.
2. Replace `https://github.com/your-username/Face-Recognition_system.git` with the actual link to your GitHub repository.
3. Save the file and upload it to your repository.

This README provides a comprehensive explanation of your project and will be helpful for beginners or anyone interested in using or extending your work. Let me know if you need further tweaks!
**
  

