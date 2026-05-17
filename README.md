# Final_Year_Project
Dataset : https://drive.google.com/drive/folders/1y3P4wLlYY6M1thjSDdeW04JqEM7-qPMV?usp=sharing
🧪 Biomedical Waste Classification using YOLOv8n
A real-time, intelligent biomedical waste classification system using  YOLOv8n, deployed on edge devices like Raspberry Pi. The system aims to automate and optimize medical waste segregation for improved public health and environmental safety.
Improper segregation of biomedical waste is a major threat to public health and the environment. This project presents an Edge-AI powered Smart Bin that classifies biomedical waste into categories like:

🔪 Sharps
🧫 Contaminated Waste
🧪 Infectious Waste
🧴 Glass/Metal Recyclables

Utilizing a high-resolution camera, the system captures real-time images and processes them using pretrained deep learning models. The model's output drives servo motors for automated waste sorting.

<img width="1998" height="814" alt="image" src="https://github.com/user-attachments/assets/053e0c46-648d-4675-bc43-d6a84de35cd8" />
<img width="1584" height="1514" alt="image" src="https://github.com/user-attachments/assets/3312173d-ee08-4671-95ec-79a26959b12b" />

🧠 Technologies Used
CNN: Custom convolutional neural network with 4.8M parameters
YOLOv8n: Real-time object detection using Ultralytics
Raspberry Pi: For edge deployment
              OpenCV

📊 Dataset
Source: "Pharmaceutical and Biomedical Waste" Kaggle dataset 
Total Images: 
Image Format: RGB, 224x224 pixels
Classes: 13 (masks, gloves, syringes, tissues, etc.)
Split: 3986 training, 1037 validation

🏗️ Model Architecture
🔹 YOLOv8n (Ultralytics)
Lightweight nano version of the YOLOv8 object detection model
Used for real-time biomedical waste detection and classification
Trained on a custom biomedical waste dataset with 640×640 input image resolution
Provides fast inference speed with low computational requirements
Suitable for deployment on embedded systems like Raspberry Pi
🔹 CNN-Based Detection Backbone
Uses Convolutional Neural Network layers for automatic feature extraction
Detects important image features such as edges, shapes, and textures
Enables accurate identification of biomedical waste objects under varying backgrounds and lighting conditions
🔹 Raspberry Pi Embedded Deployment
YOLOv8n model integrated with Raspberry Pi for edge-based real-time detection
Dedicated camera module used for live image acquisition and processing
Optimized for low-cost hardware implementation with minimal latency
🔹 Robotic Arm Integration
Detection results from YOLOv8n are used to control robotic arm movement
Automated segregation performed using predefined color-based bin allocation logic
Supports real-time biomedical waste sorting with reduced human interaction

🧪 Results
| Model   | Precision | Recall | mAP@0.5 | mAP@0.5:0.95 |
| ------- | --------- | ------ | ------- | ------------ |
| YOLOv8n | 88.60%    | 88.72% | 88.91%  | 71.73%       |

🧰 Hardware & Deployment
* Training performed using Google Colab with GPU acceleration
* Deployment implemented on Raspberry Pi for edge-based real-time detection
* Dedicated camera module used for live biomedical waste detection
* YOLOv8n model saved in PyTorch .pt format (best.pt)
* Robotic arm integrated for automated waste segregation
* Real-time inference performed using live camera feed and OpenCV

📈 Evaluation
* Model evaluated using Precision, Recall, mAP@0.5, and mAP@0.5:0.95 metrics
* Precision-Recall curve used to analyze detection accuracy
* Precision-Confidence, Recall-Confidence, and F1-Confidence curves evaluated
* Confusion matrix used for class-wise performance analysis
* Real-time biomedical waste detection tested using live video input
* Detection results visualized with bounding boxes and confidence scores

🔮 Future Work
* Integration of IoT technology for real-time monitoring and smart healthcare waste management
* Deployment of the system in hospitals, clinics, and laboratory environments
* Expansion of the biomedical waste dataset with more diverse real-world images
* Improvement in robotic arm automation and waste handling accuracy
* Implementation of cloud-based data storage and remote monitoring systems
* Enhancement of model performance using larger and more advanced AI models
* Addition of more biomedical waste categories for large-scale deployment
* Development of a fully autonomous smart biomedical waste management system

🧑‍💻 Authors
Deergha Kabdwal – deerghakabdwal@gmail.com
Manish Mehra    - manishmehra0203@gmail.com
Kanishka Pant   - kpalmora@gmail.com




