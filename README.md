
# 🧠 Thyroid Cancer Detection Using Deep Learning

This project presents an end-to-end pipeline for detecting thyroid cancer from ultrasound images using multiple deep learning models. The models classify images into **Benign** and **Malignant** categories based on TIRADS scores. A series of models including CNN, ResNet50, LSTM, Xception, and hybrid architectures were trained and evaluated.

---

## 📁 Folder Structure

```
ThyroidCancerProject/
├── Jupyter Notebooks/               → Jupyter Notebooks for each model and actions
├── image files/              → Original ultrasound images (as zip file)
├──benign                     →Images classified as benign before augmentation
├──malignant                  →Images classified as malignant before augmentation
├── xml files/                → XML files for raw image metadata
├── augmented_images/        → Final dataset (Benign & Malignant folders)
├── CSV files/               → Data CSVs for image labeling and TIRADS classification
├── Results/                 → Accuracy/loss graphs and visualizations
├── requirements.txt         → Python libraries used in the project
├── README.md                → Project overview and usage instructions
└── .gitignore               → Files/folders excluded from Git
```

---

## 🧪 Models Implemented

- ✅ CNN (Convolutional Neural Network)
- ✅ ResNet50
- ✅ GoogleNet
- ✅ Xception
- ✅ LSTM
- ✅ CNN + LSTM (Hybrid Model)
- ✅ GoogleNet + Xception (Hybrid Model)

Each model is trained using the same dataset and hyperparameters:
- **Epochs**: 30  
- **Batch Size**: 16  
- **Loss Function**: Binary Crossentropy  
- **Optimizer**: Adam

---

## 📊 Visualization

Model training and validation accuracy are visualized using line graphs. All results are saved in the `results/` folder and embedded within each notebook.

---

## 📦 Dataset and Preprocessing

- The dataset consists of ultrasound images categorized based on **TIRADS** scores.
- **TIRADS 0–3** → Labeled as **Benign**  
  **TIRADS 4a, 4b, 4c, 5** → Labeled as **Malignant**
- Data was augmented to improve class balance using rotation, zoom, flipping, and brightness shifts.
- Final image folders:  
  - `augmented_images/benign/`  
  - `augmented_images/malignant/`

---

## 🔗 Download Resources

Due to GitHub storage limitations, large files have been uploaded to Google Drive. Please download them before running the code.
And you can also take the reference as it contains every detail about that project.
👉 **[Download Images, XMLs, Augmented Data, and Trained Models]
(https://drive.google.com/drive/folders/1sk11WBBY14i8-HtXA1svwxpMVSTutEsQ?usp=sharing)**  


After downloading, place them in their respective folders.

---

## 🛠 How to Run

1. **Clone the Repository**
```bash
git clone https://github.com/yourusername/thyroid-cancer-detection.git
cd thyroid-cancer-detection
```

2. **Install Required Libraries**
```bash
pip install -r requirements.txt
```

3. **Open and Run Notebooks**
- Navigate to `notebooks/` and open any `.ipynb` file.
- Run cells step-by-step to view results and training graphs.

---

## 🧠 Technologies Used

- Python
- TensorFlow / Keras
- OpenCV
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook / Google Colab

---

## 🙋‍♀️ Author

**Saunak Saha**  
Email: saunak.saha321@gmail.com  
LinkedIn: https://www.linkedin.com/in/saunak-saha-273506228/ 
GitHub: https://github.com/Saunak11

---

## ⚠️ Disclaimer

This project is developed for academic purposes. It is not intended to be used for real-world medical diagnosis without expert supervision.
