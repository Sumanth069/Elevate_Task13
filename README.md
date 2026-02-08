# Elevate_Task13
Applied PCA to reduce feature dimensions of the MNIST/Digits dataset, analyzed explained variance, and compared classification accuracy using Logistic Regression on original vs reduced data.

This project demonstrates the use of Principal Component Analysis (PCA) to reduce the dimensionality of image datasets while preserving maximum variance. PCA is applied to handwritten digit images, and the impact of dimensionality reduction on classification performance is evaluated using Logistic Regression.

The project helps understand the trade-off between feature compression and model accuracy, which is crucial in real-world machine learning systems.

🛠️ Tools & Technologies

Python

Scikit-learn

Matplotlib

NumPy

Pandas

Alternative Techniques: OpenCV PCA

📂 Dataset

Primary: Sklearn Digits Dataset

Alternative: MNIST Dataset

Dataset Details

Digits dataset contains 8×8 grayscale images

Images are flattened into 64-dimensional feature vectors

Total samples: 1797

The dataset is loaded directly using Scikit-learn (no manual download required).

🔍 Project Workflow

Load handwritten digits dataset

Flatten images into feature vectors

Apply StandardScaler for feature normalization

Perform PCA with different component counts (2, 10, 30, 50)

Analyze explained variance ratio

Plot cumulative explained variance

Generate reduced datasets using PCA

Train Logistic Regression on:

Original dataset

PCA-reduced datasets

Compare model accuracy

Visualize 2D PCA projection

📈 Results & Observations

PCA significantly reduces feature dimensions with minimal accuracy loss

Higher components retain more variance and better accuracy

Very low dimensions (e.g., 2D) cause information loss

PCA improves computational efficiency

Typical Accuracy Comparison
Dataset	Accuracy
Original (No PCA)	~97–98%
PCA (50 components)	~96–97%
PCA (30 components)	~94–95%
PCA (10 components)	~90–92%
PCA (2 components)	~60–65%

📁 Reduced Dataset

digits_pca_2.csv
digits_pca_10.csv
digits_pca_30.csv
digits_pca_50.csv


Each file contains:

PCA-transformed features

Corresponding class labels

# Output

<img width="509" height="221" alt="Image" src="https://github.com/user-attachments/assets/46af7b46-58d3-4f66-9bc0-fa8446ed2c73" />

<img width="806" height="555" alt="Image" src="https://github.com/user-attachments/assets/9ab44a91-0b3a-4c50-8beb-fb9cc0471f08" />

<img width="660" height="686" alt="Image" src="https://github.com/user-attachments/assets/7efc94b8-871e-4a97-b42a-bef67a88924e" />

<img width="755" height="689" alt="Image" src="https://github.com/user-attachments/assets/e699eefd-3cab-4a5b-bfa6-d3d4c634a72b" />



