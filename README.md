# Sephora Best Seller Prediction

A machine learning project that classifies Sephora products into bestseller tiers (High / Medium / Low) using a Decision Tree classifier. Built to explore how product engagement metrics — ratings, review volume, and popularity — can be used to identify top-performing products in the beauty industry.

## Dataset
[Sephora Products and Skincare Reviews](https://www.kaggle.com/datasets/nadyinky/sephora-products-and-skincare-reviews) by nadyinky on Kaggle — 8,494 products across 27 columns, with customer reviews split across multiple CSVs. The file names (`product_info.csv`, `reviews_0-250.csv`, etc.) and dimensions match exactly.
CSVs not included in this repo due to GitHub's file size limits; download and place in `archive/`.

## How it works
- Bins continuous features (rating, reviews, loves_count) into Low/Medium/High categories
- Creates a rule-based `bestseller_potential` target label
- Trains a Decision Tree (`max_depth=4`) on an 80/20 split

## Results
100% accuracy — expected, since the target is derived directly from the input features.

## Stack
Python · pandas · scikit-learn · matplotlib

## Run it
1. Download the dataset from Kaggle → place in `archive/`
2. Open and run `Untitled.ipynb`
