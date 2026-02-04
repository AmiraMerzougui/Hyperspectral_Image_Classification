# Hyperspectral Image Classification – Salinas Dataset

This project implements a complete machine learning pipeline for hyperspectral image classification using the Salinas dataset.  
The objective is to perform pixel-wise land-cover classification based on spectral signatures using classical machine learning techniques.

The project is developed as a first step toward advanced hyperspectral analysis and future deep learning approaches.

## Dataset

- Salinas Hyperspectral Dataset  
- Sensor: AVIRIS (Airborne Visible/Infrared Imaging Spectrometer)  
- Spatial size: 512 × 217 pixels  
- Spectral bands: 204  
- Ground truth classes: 16  

Each pixel is represented by a 204-dimensional spectral vector.

## Methodology

The implemented pipeline follows these steps:

1. Load hyperspectral cube and ground truth labels  
2. Reshape cube into pixel-wise samples  
3. Remove background pixels  
4. Feature scaling using StandardScaler  
5. Train/Test split  
6. Train Random Forest classifier  
7. Evaluate performance  
8. Generate full-scene classification map  

## Model

- Algorithm: Random Forest Classifier  
- Library: scikit-learn  

## Results

- Test Accuracy ≈ 95%  
- Confusion matrix generated  
- Pixel-wise classification map generated for the entire scene  

These results demonstrate strong performance using a classical machine learning approach.

## Project Structure
Hyperspectral_Image_Classification/
│
├── data/
├── notebooks/
├── models/
├── results/
├── README.md
└── requirements.txt

## Tools & Libraries

- Python 3  
- NumPy  
- SciPy  
- scikit-learn  
- matplotlib  
- seaborn  
- Jupyter Notebook  


## How to Run

1. Clone the repository to your local machine:

git clone <repo_url>

2. Navigate to the project folder:

cd Hyperspectral_Image_Classification


3. Install required dependencies:

pip install -r requirements.txt

mathematica
Copier le code

4. Launch Jupyter Notebook:

jupyter notebook

arduino
Copier le code

5. Open and run:

notebooks/salinas_random_forest.ipynb


## Future Work

- Dimensionality reduction (PCA, ICA)  
- Support Vector Machines (SVM)  
- Deep Learning models (CNN, 3D-CNN)  
- Spatial-spectral feature extraction  
- Hyperparameter optimization  



