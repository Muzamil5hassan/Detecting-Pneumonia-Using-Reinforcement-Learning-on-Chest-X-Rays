# 🫁 Detecting Pneumonia Using Reinforcement Learning on Chest X-Rays

This project is a web-based application that leverages Reinforcement Learning and Deep Learning to detect pneumonia from chest X-ray images. It uses a trained TensorFlow model and provides a user-friendly interface for image upload, prediction, and user history tracking.
##  Features

- ✅ **User Authentication** – Secure login & registration system.
-  **Image Upload** – Upload chest X-ray images for diagnosis.
-  **AI Prediction** – Pneumonia detection using a TensorFlow-trained model.
-  **User History** – Tracks previous image uploads and results.
-  **Clean UI** – Responsive web interface with a seamless user experience.

# Model Setup Instructions

To use this project, you need to download a pre-trained model from the given Google Drive link and place it in the `models` directory. Follow the steps below to set it up correctly:

##  Model Setup Instructions

To run this project, you need to download the pre-trained model using the provided Google Drive link and place it in the correct directory.

###  1. Download the Model
   - Click [here](https://drive.google.com/file/d/1EcHJP_wJo_eq1PUNVMN79wKLQkm2e3yx/view?usp=drive_link) to open the Google Drive link.
   - Click the **Download** button to save the file to your local system.

###  2. Create the `models` Directory
   - Navigate to the root directory of this project.
   - Create a folder named `models` if it does not already exist.
     ```bash
     mkdir models
     ```

###  3. Move the Model File
   - Move the downloaded model file into the models folder:
     ```bash
     mv /path/to/downloaded/model models/
     ```
     Replace `/path/to/downloaded/model` with the actual path where you downloaded the file.

### ✅ 4. Verify Model Placement
   - Ensure that the model file is correctly placed in the `models` directory by listing the folder's contents:
     ```bash
     ls models
     ```
     You should see the downloaded model file in the output.

###  Application UsageUsage

##  1. Update app.py with Model Path
   - Open the `app.py` file in a text editor.
   - Locate line 8, which contains the following code:
     ```python
     tf.keras.models.load_model("")
     ```
   - Update the empty string with the relative path to the model file. For example:
     ```python
     tf.keras.models.load_model("models/your_model_file.keras")
     ```
     Replace `your_model_file.keras` with the actual name of the model file you downloaded.

##  2. Run the Flask Server
   - Open a terminal and navigate to the root directory of this project.
   - Run the following command to start the server:
     ```bash
     python app.py
     ```

##  3. Access the Web App
   - Once the server is running, follow the instructions displayed in the terminal to access the application in your web browser.

