# ReturnSense Unsupervised Return Pattern Analyzer

ReturnSense is an advanced Natural Language Processing (NLP) dashboard built inside an interactive Jupyter Notebook. It uses unsupervised machine learning to ingest thousands of raw customer reviews or complaint texts and mathematically clusters them into distinct, human-readable "Return Themes". 

This dashboard is built for presentation, demonstrating the ability to turn unstructured complaint data into targeted business analytics.

## Core Features
- **Multi-industry Configurations:** Works out-of-the-box with E-commerce electronics, Clothing retail, and Software App reviews via a simple toggle.
- **NLTK Lemmatization Engine:** Normalizes complex variations (e.g., *charging, chargers, charged* becomes *charge*) for highly accurate keyword extraction.
- **Dynamic K-Means Clustering:** Uses the Silhouette Score to mathematically validate and locate the optimal number of natural fault patterns without human bias.
- **Anti-Collision Theme Generation:** Algorithmically builds concise Cluster Themes while actively filtering out overlapping keywords.
- **Fault-Tolerant Demo Mode:** Automatically detects missing `.csv` datasets and generates realistic mock data on the fly, ensuring live presentations never crash.

## Getting Started

1. Clone the repository.
2. Install the requirements:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn nltk jupyter
   ```
3. Boot up the notebook:
   ```bash
   jupyter notebook ReturnSense.ipynb
   ```

### Adding Datasets
By default, the notebook runs perfectly using the built-in generator. To run ReturnSense on real data:
1. Create a folder named `Dataset/` in the root directory.
2. Download datasets from Kaggle (e.g., *Consumer Reviews of Amazon Products*, *Womens E-Commerce Clothing Reviews*).
3. Place the `.csv` files in the `Dataset/` folder.
4. Open the notebook and change the `DATASET_MODE` variable in Cell #2 to match your CSV!
