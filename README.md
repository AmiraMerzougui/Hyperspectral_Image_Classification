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
│ └── salinas/ # Salinas dataset files
│
├── notebooks/
│ └── salinas_random_forest.ipynb
│
└── README.md

## Tools & Libraries

- Python 3  
- NumPy  
- SciPy  
- scikit-learn  
- matplotlib  
- seaborn  
- Jupyter Notebook  

## How to Run

### Option 1: Run Locally

1. Clone the repository:
notebooks/salinas_random_forest.ipynb

2. Navigate to the project directory:
cd Hyperspectral_Image_Classification

3. Download the Salinas dataset :
https://zenodo.org/records/15771735
download Salinas_corrected.mat and Salinas_gt.mat

4. Place the dataset files inside:
data/salinas/

5. Install required dependencies:

pip install numpy scipy scikit-learn matplotlib seaborn jupyter

6. Launch Jupyter Notebook:

jupyter notebook

7. Open and run:

notebooks/salinas_random_forest.ipynb
### Option 2: Run on Google Colab

Open the notebook using the Colab link below and run all cells:

[Open Notebook in Google Colab](https://colab.research.google.com/drive/1WmsZd-O59oyO85Jcn3Ro0ABAPtnAkfYf?usp=sharing)



## Future Work

- Dimensionality reduction (PCA, ICA)  
- Support Vector Machines (SVM)  
- Deep Learning models (CNN, 3D-CNN)  
- Spatial-spectral feature extraction  
- Hyperparameter optimization  



