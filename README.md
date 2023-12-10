# Memotion Analysis: Meme Sentiment Classification

## Abstract

This project delves into meme sentiment classification, employing machine learning and deep learning models to analyze and categorize sentiments expressed in meme content. The dataset comprises 6992 meme images sourced from Kaggle, providing a diverse collection with five distinct sentiment labels—Very Positive, Positive, Neutral, Negative, and Very Negative. The multilabel nature of the dataset allows for a nuanced understanding of sentiments, capturing a spectrum of emotions and opinions in the images.

## Table of Contents

- [Architecture](#architecture)
- [About Dataset](#about-dataset)
- [Model Performance](#model-performance)
- [Usage](#usage)
- [Future Work](#future-work)
- [Contributing](#contributing)
- [License](#license)

## Architecture

The project employs various machine learning and deep learning models, including Random Forest, KNN, Extra Tree Classifier, Stochastic Gradient Descent, Multinomial Naive Bayes, Logistic Regression, Vit-sbert bilstm, and Inception ResNet-V2.

## About Dataset

The dataset consists of 6992 meme images, each labeled with one or more of the sentiment categories—Very Positive, Positive, Neutral, Negative, and Very Negative. The "Text OCR" column contains raw Optical Character Recognition (OCR) output, and the "Text Corrected" column likely presents a version of the text that has been manually or automatically corrected for accuracy. The "Overall Sentiment" column is the target variable for sentiment analysis.

## Model Performance

- *Vit-sbert bilstm Model:*
  - Accuracy: 43.56%
  - F1 Score: 36.04%
  - Discussion: The Vit-sbert bilstm model exhibits moderate performance, suggesting limitations in capturing diverse and nuanced sentiment in memes.

- *Random Forest, KNN, Extra Tree Classifier:*
  - Accuracy: $\sim$73%
  - F1 Score (Macro): $\sim$64%
  - ![Accuracy Plot](accuracy6.jpeg)
  - Discussion: Tree-based models like Random Forest, KNN, and Extra Tree Classifier outshine other methodologies, showcasing robustness in capturing intricate, non-linear relationships in meme text data.

- *Stochastic Gradient Descent Classifier:*
  - Accuracy: 49.56%
  - F1 Score (Weighted): 46.45%
  - Discussion: The Stochastic Gradient Descent Classifier demonstrates limitations in accurately categorizing meme sentiments, facing challenges in handling diverse and unconventional expressions.

- *Multinomial Naive Bayes Classifier, Logistic Regression:*
  - Accuracy: $\sim$51%
  - F1 Score (Weighted): $\sim$41%
  - Discussion: Models like Multinomial Naive Bayes and Logistic Regression exhibit constrained performance, struggling to capture diverse sentiments in memes.

- *Inception ResNet-V2:*
  - Accuracy: 47.13%
  - F1 Score: 30.19%
  - Discussion: The Inception ResNet-V2 architecture faces challenges in meme sentiment analysis, struggling to extract meaningful features from meme text data.

These metrics provide insights into the performance of each model. While some models showcase higher accuracy and F1 scores, their ability to comprehend nuanced sentiments within memes varies. The discussion further highlights the challenges and limitations faced by different methodologies in effectively capturing the complex nature of meme sentiments.

## Usage

To reproduce the experiments:
1. Clone the repository.
2. Set up the required environment and dependencies.
3. Run the code to train and evaluate models.
4. Interpret the results and metrics provided.

## Future Work

...

## Contributing

If you'd like to contribute to the project, please follow the guidelines in the [CONTRIBUTING.md](CONTRIBUTING.md) file.

## License

This project is licensed under the [MIT License](LICENSE).
