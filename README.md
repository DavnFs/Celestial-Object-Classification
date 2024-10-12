# Celestial Object Classification

This project classifies celestial objects (e.g., stars, galaxies, and quasars) using a dataset of astronomical features. The project leverages data preprocessing, visualization, and machine learning models to predict the class of an object.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Model Performance](#model-performance)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The aim of this project is to classify different types of celestial objects based on their astronomical data. The classification task involves distinguishing between **stars**, **galaxies**, and **quasars** using various features extracted from observations.

This project involves:
- Data exploration and visualization
- Building a machine learning model for classification
- Evaluating the model performance

## Dataset
https://www.kaggle.com/datasets/diraf0/sloan-digital-sky-survey-dr18

The dataset contains features related to celestial objects, such as:
- Magnitude in different filters
- Redshift
- Spectral information

Classes in the dataset:
- **Star**
- **Galaxy**
- **QSO (Quasar)**

## Installation

To run this project, you need to have Python installed. The main libraries required include:

- `pandas`
- `plotly`
- `scikit-learn`
- `matplotlib`
- `numpy`

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/DavnFs/Celestial-Object-Classification.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Celestial-Object-Classification
   ```
3. Run the Jupyter notebook to explore the code and visualize results:
   ```bash
   jupyter notebook Classification.ipynb
   ```

## Results

The project visualizes the data distribution of different celestial classes and builds a classification model. You can visualize the number of objects in each class and the accuracy of the classification model through the plots generated in the notebook.

## Model Performance

The table below shows the performance of various machine learning models tested on the dataset:

| Model               | Accuracy | F1 Score | Precision | Recall |
|---------------------|----------|----------|-----------|--------|
| Neural Network       | 0.8591   | 0.857084 | 0.856733  | 0.8591 |
| Ensemble Stacking    | 0.8461   | 0.842662 | 0.842770  | 0.8461 |
| SVM                  | 0.8368   | 0.830335 | 0.834345  | 0.8368 |
| Kernel SVM           | 0.8368   | 0.830335 | 0.834345  | 0.8368 |
| KNN                  | 0.8136   | 0.806301 | 0.807546  | 0.8136 |
| Decision Tree        | 0.7953   | 0.795347 | 0.795425  | 0.7953 |
| Naive Bayes          | 0.6023   | 0.605971 | 0.622790  | 0.6023 |

### Key Observations:
- **Neural Network** achieved the best overall performance with the highest accuracy, F1 Score, and precision.
- **Ensemble Stacking** and **SVM** models performed quite well, with only slight differences compared to the Neural Network.
- **Naive Bayes** had the lowest performance, indicating it might not be well-suited for this particular dataset.

## Contributing

Feel free to open issues or submit pull requests if you find bugs or have suggestions for improvements.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
