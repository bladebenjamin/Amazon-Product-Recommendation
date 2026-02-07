📦 Amazon Product Recommendation System
🎯 Project Overview
As a Data Science Manager at Amazon, I spearheaded the development of a recommendation engine to tackle "information overload." By analyzing millions of user-product interactions, this system identifies hidden patterns in consumer behavior to provide highly personalized product suggestions.

## 💾 Dataset
The dataset consists of **7.8 Million reviews** of electronic products.
* **Direct Data Link:** [Download ratings_Electronics.csv (304 MB)](https://drive.google.com/file/d/1XahZcR287ke7j48I7-oj0KzmmwSSvA3Y/view?usp=sharing)
* **Attributes:** `userId`, `productId`, `Rating`, `timestamp`.

> **Note:** Due to GitHub's file size limitations (100MB), the raw `.csv` is hosted externally. Please download and place it in your local directory to run the notebook.

🛠️ Technical Implementation
We implemented a tiered recommendation strategy:

Rank-Based (Popularity): For new users with no history (Cold Start).

Collaborative Filtering: User-User and Item-Item similarity using Cosine Similarity.

Matrix Factorization (SVD): Leveraged the Surprise library to decompose the interaction matrix into latent features, significantly reducing RMSE.

📈 Key Results
Best Model: Optimized SVD.

Performance: Achieved superior precision at top-k recommendations compared to baseline popularity models.

Scalability: The item-item collaborative filtering approach was designed to scale across massive datasets, mirroring Amazon's production-level real-time requirements.

🚀 How to Run
Clone the repo: git clone https://github.com/your-username/Amazon-Product-Recommendation.git

Install dependencies: pip install -r requirements.txt

Download the data from the link above and place it in the root directory.

Open Amazon Product Recommendation System.ipynb in Jupyter or Google Colab.
