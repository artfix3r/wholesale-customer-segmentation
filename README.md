# Wholesale Customer Segmentation

Unsupervised machine learning project that identifies distinct customer segments
from a wholesale distributor dataset using K-Means and Hierarchical Clustering.

---

## 📌 Project Overview

This project applies clustering techniques to group wholesale customers based on
their annual spending across six product categories. The goal is to uncover
hidden patterns in purchasing behavior to support targeted business strategies.

---

## 📂 Dataset

- **Source:** Wholesale Customers Dataset (UCI Machine Learning Repository)
- **Samples:** 440 customers
- **Features used:** `Fresh`, `Milk`, `Grocery`, `Frozen`, `Detergents_Paper`, `Delicassen`
- **Dropped columns:** `Channel`, `Region` (not used for modeling)

---

## 🔧 Workflow

1. **Data Preparation**
   - Load and inspect the dataset
   - Check for missing values
   - Drop non-relevant columns (`Channel`, `Region`)
   - Standardize features using `StandardScaler`

2. **K-Means Clustering**
   - Fit models for K = 2 to 15
   - Use the **Elbow Method** to identify optimal K
   - Apply final K-Means model and assign cluster labels

3. **Hierarchical Clustering**
   - Generate a **Dendrogram** to visualize cluster structure
   - Determine optimal number of clusters visually

---

## 🛠️ Technologies

| Tool | Purpose |
|------|---------|
| Python | Core language |
| Pandas | Data manipulation |
| Scikit-learn | KMeans, StandardScaler |
| Matplotlib / Seaborn | Visualization |
| SciPy | Dendrogram (hierarchical clustering) |

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/wholesale-customer-segmentation.git
   cd wholesale-customer-segmentation
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch the notebook:
   ```bash
   jupyter notebook wholesale_customer_segmentation_kmeans.ipynb
   ```

---

## 📊 Results

- Optimal number of clusters identified via Elbow Method
- Customers successfully grouped into meaningful segments
- Dendrogram confirmed cluster structure from hierarchical analysis

---

## 👤 Author

**Yusif İmamverdiyev**  
[GitHub](https://github.com/artfi3r) 

---

## 📜 License

This project is licensed under the MIT License.
