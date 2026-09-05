\# Hyperspectral Plant Analysis Using Autoencoder and Fuzzy C-Means Clustering



\## 📌 Overview



This project explores \*\*hyperspectral plant data analysis\*\* using deep learning and unsupervised machine learning techniques.



The workflow uses a \*\*Convolutional Autoencoder\*\* to learn compact latent representations from hyperspectral image patches, followed by \*\*Fuzzy C-Means (FCM) clustering\*\* to group the extracted features.



The project also includes a \*\*leaf-patch filtering step\*\* to remove patches containing a large amount of non-leaf/background information and evaluates how filtering affects the clustering results.



\---



\## 🎯 Objectives



\- Preprocess hyperspectral plant cubes into fixed-size patches.

\- Learn compact feature representations using a Convolutional Autoencoder.

\- Extract 30-dimensional latent features from hyperspectral patches.

\- Apply Fuzzy C-Means clustering to the latent representations.

\- Remove patches containing insufficient leaf information.

\- Re-run clustering on the filtered dataset.

\- Visualize clusters using PCA and spectral signatures.

\- Analyze plant-to-cluster distributions.



\---



\## 🔬 Dataset Representation



The hyperspectral data consists of three plant categories:



\- \*\*Canola\*\*

\- \*\*Soybean\*\*

\- \*\*Waterhemp\*\*



Each hyperspectral cube contains:



\- \*\*224 spectral bands\*\*

\- Spatial dimensions of height × width

\- Non-overlapping \*\*64 × 64\*\* patches



The preprocessing workflow uses approximately:



\- \*\*70% training data\*\*

\- \*\*30% testing data\*\*



The extracted training patches are used for feature learning and clustering.



\---



\## 🧠 Methodology



The complete workflow is:



```text

Hyperspectral Cubes

&#x20;       ↓

Preprocessing

&#x20;       ↓

64 × 64 × 224 Patches

&#x20;       ↓

Convolutional Autoencoder

&#x20;       ↓

30-Dimensional Latent Features

&#x20;       ↓

Fuzzy C-Means Clustering

&#x20;       ↓

Cluster Analysis

&#x20;       ↓

Leaf Patch Filtering

&#x20;       ↓

Filtered Latent Features

&#x20;       ↓

Fuzzy C-Means Clustering

&#x20;       ↓

PCA / Spectral / Distribution Visualization

