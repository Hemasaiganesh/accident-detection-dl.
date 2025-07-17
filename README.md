# Traffic Buddy 🚦  
**An Intelligent AI-Powered Traffic Forecasting and Vehicle Detection System**

Developed by:  

- U. Hema Sai Ganesh
- Yoga Venkata Nikhil Tanneeru  
- Prasanna Kumar  
Affiliation: VIT-AP University, Amaravati

---

## 📌 Overview  
**Traffic Buddy** is a machine learning-based intelligent system for real-time **traffic prediction** and **vehicle detection**.  
It combines **Support Vector Regression (SVR)** and deep learning models like **MobileNet** and **ResNet-50**  
to provide actionable traffic insights that can enhance traffic flow, reduce congestion, and improve road safety.

---

## 📊 Output Ratios & Performance Metrics

| Metric                    | Value                      |
|---------------------------|----------------------------|
| Image Size                | 180 × 180 pixels           |
| Dataset Split             | 80% Training / 20% Validation |
| Optimizer                 | Adam (Learning Rate = 0.001) |
| Loss Function             | CrossEntropyLoss with Label Smoothing (ε = 0.1) |
| Epochs                    | 5                          |
| Classification Type       | Binary (Accident / Non-Accident) |
| Final Training Accuracy   | **~98.67%**                |
| Final Validation Accuracy | **~95.42%**                |
| Final Training Loss       | **~0.045**                 |
| Final Validation Loss     | **~0.073**                 |
| Hardware Used             | CUDA-enabled GPU           |
| Pretrained Model          | ResNet-50 (transfer learning) |

---

## ⚙️ Methodology Summary

- **Data Augmentation:** Random Rotation, Horizontal Flip, Resizing  
- **Normalization:** Pixel values scaled to [-1, 1]  
- **Transfer Learning:** ResNet-50 with a custom binary classification head  
- **Training Strategy:** Adam optimizer, label smoothing for regularization  
- **Evaluation Metrics:** Accuracy, Loss, Softmax Probabilities  
- **Visualization:** Matplotlib plots for training/validation accuracy and loss  

---

## 🗃️ Dataset

- **Source:** Kaggle  
- **Structure:**

dataset/
├── Accident/
│ ├── img1.jpg
│ └── ...
└── Non-Accident/
├── img1.jpg
└── ...

- **Task:** Binary image classification

---

## 🧠 Technologies Used

- **Languages:** Python  
- **Frameworks:** PyTorch  
- **Libraries:** Matplotlib, torchvision  
- **Models:** ResNet-50 (pretrained), SVR  
- **Tools:** CUDA, Jupyter Notebook

---

## 📈 Key Takeaways

- Achieved **high accuracy** using transfer learning on a small dataset  
- Label smoothing reduced overconfidence and improved generalization  
- ResNet-50’s residual blocks helped avoid vanishing gradient problems  
- Visual analysis helped monitor convergence and prevent overfitting  

---

## 📚 References

For a detailed reference list of over 25 scholarly articles from IEEE, Springer, and Transportation Research journals, refer to the **[Conference Paper](./Conference%20Paper.pdf)** in this repository.

---

## 👏 Acknowledgements

Special thanks to **Dr. G Suma** (Faculty Advisor, VIT-AP University) for continuous guidance throughout the project.

---

## 📬 Contact

- 📧 saiganesh407@gmail.com  
- 📍 VIT-AP University, Amaravati

---


## Authors
- U Hema Sai Ganesh (VIT-AP University)
- Co-authors: Yoga Venkata Nikhil, Prasanna Kumar, Dr. G Suma
[Final Review PPT.pptx](https://github.com/user-attachments/files/21301769/Final.Review.PPT.pptx)
[Conference Paper.pdf](https://github.com/user-attachments/files/21301766/Conference.Paper.pdf)
