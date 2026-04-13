# Iris Flower Classification Model

## Overview
Classify iris flowers into three species (Setosa, Versicolor, Virginica) based on measurements of their petals and sepals. This project implements a machine learning classification model trained on the famous Iris dataset.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Information](#model-information)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Dataset
The model is trained on the classic Iris dataset containing 150 samples of iris flowers. Each sample has 4 features:
- **Sepal Length** (cm)
- **Sepal Width** (cm)
- **Petal Length** (cm)
- **Petal Width** (cm)

The dataset includes three iris species with 50 samples each.

## Installation

### Prerequisites
- Python 3.7 or higher
- pip package manager

### Setup
1. Clone the repository:
```bash
git clone https://github.com/priteshksahu/-Iris-Flower-Classification-Model.git
cd -Iris-Flower-Classification-Model
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

## Usage

### Training the Model
```python
from model import train_model
from data import load_iris_data

X_train, X_test, y_train, y_test = load_iris_data()
model = train_model(X_train, y_train)
```

### Making Predictions
```python
from model import load_model

model = load_model('iris_model.pkl')
predictions = model.predict([[5.1, 3.5, 1.4, 0.2]])
print(predictions)  # Output: ['Setosa']
```

## Model Information
- **Algorithm**: Support Vector Machine (SVM) / Logistic Regression / Random Forest
- **Training Set Size**: 120 samples (80%)
- **Test Set Size**: 30 samples (20%)
- **Accuracy**: ~95%+

## Project Structure
```
-Iris-Flower-Classification-Model/
│
├── data/
│   └── iris.csv                    # Iris dataset
├── model.py                        # Model definition and training
├── data.py                         # Data loading and preprocessing
├── predict.py                      # Prediction script
├── requirements.txt                # Python dependencies
├── README.md                       # This file
└── examples/
    └── sample_predictions.py       # Example usage
```

## Contributing
Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

Please ensure your code follows the existing style and includes appropriate documentation.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Author
**Pritesh Sahu**
- GitHub: [@priteshksahu](https://github.com/priteshksahu)

---

*Last updated: April 13, 2026*