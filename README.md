$$ Project: Deep Learning-Based Face Recognition with Adversarial Patch Defense $$


This repository implements a deep learning model for face recognition while addressing potential adversarial attacks that could deceive the system.

Key Features:

Dataset Preparation:
Utilizes Dataset_Creation.ipynb to generate well-structured train, validation, and test datasets containing face images.
Employs MTCNN face detection (Face_extraction.ipynb) to accurately extract faces from images, handling potential cases where detection fails. Excluded images are logged for further analysis.
Face Recognition Model:
Leverages a custom-built ResNet56 architecture for robust face recognition.
Integrates a mechanism to handle "unknown" faces using confidence scores as thresholds. Faces falling below the threshold are identified as unknown.
Adversarial Patch Defense:
Explores adversarial patch generation using both targeted and untargeted attacks to test the model's resilience.
Aims to improve model robustness against these attacks in future iterations.
Getting Started:

Prerequisites:

Python 3.x (with recommended libraries: TensorFlow, OpenCV, MTCNN)
Familiarity with deep learning concepts and image processing
Cloning the Repository:

Bash
git clone https://github.com/<your_username>/face-recognition-adversarial-patch-defense.git
Use code with caution.
content_copy
Setting Up the Environment:

Create a virtual environment (recommended) and install required dependencies:
Bash
pip install -r requirements.txt
Use code with caution.
content_copy
Running the Project:

Note: Due to security concerns, the data (faces_train, faces_valid, faces_test) cannot be shared. However, the provided instructions assume you have prepared these datasets yourself.

Dataset Preparation and Face Extraction:

Run Dataset_Creation.ipynb to create the datasets as described above.
Execute Face_extraction.ipynb to extract faces using MTCNN.
Face Recognition Training:

Train the ResNet56 model using your custom training script or a deep learning framework like TensorFlow.
Experiment with hyperparameter tuning to optimize model performance.
Unknown Face Handling:

Modify your training script or model inference code to incorporate a confidence score threshold for identifying unknown faces.
Choose a suitable threshold based on your dataset and desired balance between accuracy and false negatives.
Adversarial Patch Generation (Optional):

Explore adversarial patch generation using methods like Fast Gradient Sign Method (FGSM) or Carlini-Wagner Attack (C&W).
This is an advanced topic; it's recommended to research these methods before attempting them.
Future Work:

Continuously evaluate and improve the model's accuracy and robustness against adversarial attacks.
Explore more sophisticated adversarial patch generation techniques and corresponding defense mechanisms.
Integrate the face recognition model into a real-world application, considering ethical implications and user privacy.
Contributing:

We welcome contributions to this project! Feel free to submit pull requests with bug fixes, improvements, or new features. Please ensure your code adheres to best practices and includes clear documentation.
