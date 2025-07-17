Traffic Buddy 🚦
An Intelligent AI-Powered Traffic Forecasting and Vehicle Detection System
Developed by: Yoga Venkata Nikhil Tanneeru, Prasanna Kumar, U. Sai Ganesh
Affiliation: VIT-AP University, Amaravati

📌 Overview
Traffic Buddy is a machine learning-based intelligent system for real-time traffic prediction and vehicle detection using computer vision. It combines Support Vector Regression (SVR) and deep learning models like MobileNet and ResNet-50 to provide actionable traffic insights that can enhance traffic flow, reduce congestion, and improve road safety.

📊 Output Ratios & Performance Metrics
The model's training and validation results are as follows:

Metric	Value
Image Size	180 × 180 px
Dataset Split	80% Training / 20% Validation
Optimizer	Adam (LR = 0.001)
Loss Function	CrossEntropyLoss with Label Smoothing (ε = 0.1)
Epochs	5
Classification Type	Binary (Accident / Non-Accident)
Final Training Accuracy	~98.67%
Final Validation Accuracy	~95.42%
Final Training Loss	~0.045
Final Validation Loss	~0.073
Hardware Used	CUDA-enabled GPU
Pretrained Model	ResNet-50 (transfer learning)

Graphs showing accuracy and loss curves across epochs are included in the report to illustrate convergence.

⚙️ Methodology Summary
Data Augmentation: Random Rotation, Horizontal Flip, Resizing

Normalization: Pixel range scaled to [-1, 1]

Transfer Learning: ResNet-50 with custom classification head

Evaluation Metrics: Accuracy, Loss, Softmax Probabilities

Visualization Tools: Matplotlib plots for training vs validation loss and accuracy

🗃️ Dataset
Source: Kaggle

Structure:

markdown
Copy
Edit
└── dataset/
    ├── Accident/
    │   ├── img1.jpg
    │   └── ...
    └── Non-Accident/
        ├── img1.jpg
        └── ...
Binary classification with a balanced dataset.

🧠 Technologies Used
Languages: Python

Frameworks: PyTorch

Models: ResNet-50 (with Transfer Learning), SVR

Tools: Matplotlib, CUDA, DataLoader

📈 Key Takeaways
Achieved high performance on limited, domain-specific data through transfer learning.

Label smoothing improved generalization by reducing model overconfidence.

ResNet-50's skip connections helped mitigate the vanishing gradient problem during training.

Scalable design adaptable to different urban traffic conditions.

📚 References
A comprehensive list of 25+ scholarly references from IEEE, Springer, and Transportation Research journals is included in the full PDF report.
## Authors
- U Hema Sai Ganesh (VIT-AP University)
- Co-authors: Yoga Venkata Nikhil, Prasanna Kumar, Dr. G Suma
[Final Review PPT.pptx](https://github.com/user-attachments/files/21301769/Final.Review.PPT.pptx)
[Conference Paper.pdf](https://github.com/user-attachments/files/21301766/Conference.Paper.pdf)
