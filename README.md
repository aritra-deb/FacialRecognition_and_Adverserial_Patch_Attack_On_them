# Project: Deep Learning-Based Face Recognition with Adversarial Patch Defense 

This repository implements a deep learning model for face recognition while addressing potential adversarial attacks that could deceive the system.

## Key Features:

### Dataset Preparation:
- Utilizes `Dataset_Creation.ipynb` to generate well-structured train, validation, and test datasets containing face images.
- Employs MTCNN face detection (`Face_extraction.ipynb`) to accurately extract faces from images, handling potential cases where detection fails. Excluded images are logged for further analysis.

### Face Recognition Model:
- Leverages a custom-built ResNet56 architecture for robust face recognition.
- Integrates a mechanism to handle **"unknown"** faces using confidence scores as thresholds. Faces falling below the threshold are identified as unknown.

### Adversarial Patch Defense:
- Explores adversarial patch generation using both targeted and untargeted attacks to test the model's resilience.
- Aims to improve model robustness against these attacks in future iterations.

## Getting Started:

### Prerequisites:
- Python 3.x (with recommended libraries: TensorFlow, OpenCV, MTCNN)
- Familiarity with deep learning concepts and image processing

### Cloning the Repository:
```bash
git clone https://github.com/aritra-deb/FacialRecognition_and_Adverserial_Patch_Attack_On_them.git

