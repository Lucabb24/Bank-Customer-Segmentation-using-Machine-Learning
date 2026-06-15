# Bank-Customer-Segmentation-using-Machine-Learning
# Project Overview
This project focused on an customer segmentation analysis for a banking institution. Using a dataset of 800 bank clients, the goal of this analysis was to identify distinct customer profiles based on their financial behavior and demographics[cite: 4]

## Tools Used
* **Python (Google Colab / Jupyter):** Data exploration, statistical analysis, feature scaling, and advanced clustering modeling[cite: 4].
* **Scikit-Learn:** Data preprocessing via `StandardScaler` and model evaluation using Silhouette Scores and the Elbow Method[cite: 4].

# Key Insights 
**Total Dataset Size:** 800 Clients[cite: 4]
**Optimal Segment Count (K):** 4 Clusters[cite: 1]
**Clustering Evaluation:** K-Means Silhouette Score of ~0.505, Agglomerative Clustering Score of ~0.490[cite: 1]

### Product & Behavior Performance:
* **The Young & Digitally Active** cluster showed high mobile login rates and high transaction frequencies but retained lower account balances[cite: 4]. *Strategy:* Target with digital banking perks, gamified loyalty programs, and low-fee accounts.
* **The High-Net-Worth / Premium** cluster consisted of an older demographic with substantial monthly incomes, massive account balances, and high savings rates[cite: 4]. *Strategy:* Deliver premium private banking services, wealth management, and long-term investment funds.
* **The Credit-Reliant** cluster was identified as an underperforming or higher-risk area, showing a significantly high loan-to-income ratio combined with low savings[cite: 4]. *Strategy:* Introduce debt consolidation offers and apply tighter credit risk mitigation.

### Regional & Team Performance:
Using demographic variables as descriptive markers rather than cluster inputs, further customer insights were extracted:
* **Stable Core (Mid-Market)** clients exhibited steady, average income levels across different city sizes, maintaining a reliable number of bank products[cite: 4]. *Strategy:* Deploy standard cross-selling for insurance products and credit cards.
* **Demographic Filtering** confirmed that utilizing behavioral metrics rather than basic metryczkowe data (`gender`, `city_size`) prevents algorithmic noise and yields cleaner segments[cite: 4].

## Machine Learning Showcase
The full code is available in the `Bank_Customer_Segmentation.ipynb` file[cite: 2]. It includes concepts such as:
* Data standardization using `StandardScaler` to normalize varied financial metrics[cite: 4].
* `KMeans(n_clusters=4)` and `AgglomerativeClustering(n_clusters=4)` to programmatically divide the client base[cite: 1, 4].
