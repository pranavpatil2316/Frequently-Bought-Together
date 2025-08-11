# Frequently Bought Together Recommendation System

A simple **Item-Based Collaborative Filtering** project that suggests items often bought together, similar to Amazon's "Frequently Bought Together" feature.

## Dataset
We use the [Groceries Dataset](https://www.kaggle.com/datasets/heeraldedhia/groceries-dataset) from Kaggle.
Download `groceries.csv` and place it in the project folder.

## Installation
1. Clone this repository:
```bash
git clone https://github.com/yourusername/frequently_bought_together.git
cd frequently_bought_together
````

2. Install required dependencies:

```bash
pip install -r requirements.txt
```

3. Download the dataset from Kaggle and place `groceries.csv` in this folder.

## Usage

Run the application:

```bash
python app.py
```

Example output:

```
Available products (sample): tropical fruit, whole milk, pip fruit, ...
Enter the product you bought: whole milk
If you bought whole milk, you may also like: other vegetables, rolls/buns, yogurt
```

## How It Works

* Groups transactions by customer or transaction ID.
* Creates a co-occurrence count of items bought together.
* Suggests the top N most co-purchased items for a given product.
