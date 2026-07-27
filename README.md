# Machine Learning Portfolio

A collection of machine-learning projects in **Python**, spanning the full workflow: collecting data from
the web, classical models on tabular data, and deep learning on tabular and image data. Built with
**scikit-learn** and **TensorFlow / Keras**. Each notebook is self-contained and keeps its saved outputs
(plots, model summaries, metrics), so it can be read without re-running.

## Projects

| # | Notebook | Task | Key techniques |
|---|----------|------|----------------|
| 1 | [`01_web_scraping_ecommerce.ipynb`](01_web_scraping_ecommerce.ipynb) | Collect product data from a website | requests, BeautifulSoup, DOM parsing, pandas, Excel export |
| 2 | [`02_tabular_classification_census_income.ipynb`](02_tabular_classification_census_income.ipynb) | Predict income bracket | Random Forest, Gradient Boosting, Logistic Regression, pipelines, GridSearchCV |
| 3 | [`03_neural_network_tuning_keras_tuner.ipynb`](03_neural_network_tuning_keras_tuner.ipynb) | Neural net on the same tabular data | Feed-forward NN, Keras Tuner hyperparameter search, dropout, early stopping |
| 4 | [`04_cnn_image_classification.ipynb`](04_cnn_image_classification.ipynb) | Image classification from scratch | CNN (Xception-inspired), data augmentation |
| 5 | [`05_image_classification_transfer_learning.ipynb`](05_image_classification_transfer_learning.ipynb) | Flower classification, two approaches | Custom CNN vs DenseNet121 transfer learning, confusion matrix, F1 |
| 6 | [`06_convolutional_autoencoder_denoising.ipynb`](06_convolutional_autoencoder_denoising.ipynb) | Image denoising | Convolutional autoencoder (encoder–decoder) |

## Data collection

**1 — Web scraping.** A scraper using requests and BeautifulSoup that extracts structured product data from
an e-commerce site, gathers the results of a search into a pandas DataFrame, and exports a filtered subset
to Excel.

## Classical machine learning

**2 — Tabular classification (census income).** An end-to-end pipeline: cleaning, feature engineering, a
`ColumnTransformer` for scaling and one-hot encoding, and a comparison of Random Forest, Gradient Boosting
and Logistic Regression, each tuned with `GridSearchCV`.

## Deep learning

**3 — Neural network tuning (Keras Tuner).** A feed-forward network on the same census data, with its layer
sizes, dropout and learning rate searched automatically by Keras Tuner — the deep-learning counterpart to
project 2.

**4 — Convolutional neural network (CNN).** A small Xception-style CNN built from scratch to classify images
into two classes, with data augmentation and inference on a new image.

**5 — Transfer learning (CNN vs DenseNet121).** A flower classifier built two ways — a custom CNN and a
DenseNet121 pretrained on ImageNet — compared with learning curves, confusion matrices and classification
reports. The richest project of the set.

**6 — Convolutional autoencoder (denoising).** An encoder–decoder network trained to reconstruct clean
images from noisy ones on CIFAR-10.

## Tech stack
Python · scikit-learn · TensorFlow / Keras · Keras Tuner · BeautifulSoup · NumPy · pandas · Matplotlib · seaborn

## Data
The datasets are not included in the repository. CIFAR-10 downloads automatically via Keras; the census,
image and scraped data came from university coursework. Some notebooks use Google Colab paths (`/content/...`)
that may need adjusting to run locally.

## About
These projects come from the machine-learning and Big Data Analytics courses of my Master's in Statistical
Methods and Applications at Sapienza University of Rome, cleaned up and organised here as a portfolio.
