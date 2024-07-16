# IMDb Sentiment Classification

## Project Overview

This project focuses on binary sentiment classification of IMDb movie reviews using Gensim. The goal is to classify each review as either positive or negative. The dataset is balanced, containing 25,000 reviews in total, with 12,500 positive and 12,500 negative reviews.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Requirements](#requirements)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Dataset

The dataset used in this project is the IMDb dataset, which is widely used for binary sentiment classification tasks. It contains 25,000 reviews, equally divided into positive and negative sentiments. The dataset file is stored in a compressed tar.gz archive.

Dataset path: `aclImdb_v1.tar.gz`

## Requirements

To run this project, you need to have the following libraries installed:

- Python 3.x
- spaCy
- Gensim
- scikit-learn
- pandas
- Jupyter

You can install the required libraries using the following command:

```sh
pip install spacy gensim scikit-learn pandas jupyter
```

Additionally, you need to download the spaCy language model:

```sh
python -m spacy download en_core_web_sm
```

## Project Structure

The project structure is as follows:

```
imdb-sentiment-classification/
│
├── data/
│   ├── aclImdb_v1.tar.gz
│
├── notebooks/
│   ├── imdb_sentiment_analysis.ipynb
│
├── README.md
└── requirements.txt
```

- `data/` contains the dataset file.
- `notebooks/` contains the Jupyter Notebook for data exploration, preprocessing, training, and evaluation.
- `README.md` is this file.
- `requirements.txt` lists all the required dependencies.

## Usage

1. **Extract the dataset**:

   Extract the `aclImdb_v1.tar.gz` file into the `data/` directory.

2. **Run the Jupyter Notebook**:

   Open the Jupyter Notebook to preprocess the data, train the model, and evaluate its performance:

   ```sh
   jupyter notebook notebooks/imdb movies.ipynb 
   ```

3. **Follow the Notebook**:

   Follow the steps in the notebook for data exploration, preprocessing, model training, and evaluation.

## Results

The model performance is evaluated based on accuracy, precision, recall, and F1-score. Both the Random Forest and Gradient Boosting models were tested, and the results were as follows:

- **Random Forest**: Achieved perfect scores with precision, recall, and F1-score all at 1.00.
- **Gradient Boosting**: Also achieved perfect scores but correctly predicted 80.9% of the data, slightly outperforming the Random Forest model.

## Contributing

Contributions to this project are welcome. If you have any improvements or suggestions, please create a pull request or open an issue.

## License

This project is licensed under the MIT License.

---

Feel free to modify this template according to your specific project details and preferences.
