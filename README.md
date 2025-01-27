# SONAR Mine vs Rock Prediction using Logistic Regression

This project uses sonar data to classify whether the sonar reading represents a **Mine** or **Rock** using a **Logistic Regression** model. The dataset contains features derived from sonar signals, and the task is to predict whether the object detected is a mine or a rock. Logistic Regression was chosen as the model for its simplicity and effectiveness in binary classification problems. The dataset contains 208 rows and 60 features.

To run this project, you need to have Python installed along with some libraries. Use the following command to install the necessary dependencies:

```bash
pip install -r requirements.txt
```

First, clone the repository using the following commands:

```bash
git clone https://github.com/yourusername/sonar-mine-vs-rock.git
cd sonar-mine-vs-rock
```

Ensure the dataset `SONAR_rock_VS_mine_Dataset.csv` is available in the project directory.

Run the main script to train the model and make predictions using:

```bash
python sonar_mine_vs_rock.py
```

The repository is structured as follows:

```
sonar-mine-vs-rock/
│
├── README.md                  # Project documentation
├── sonar_mine_vs_rock.py       # Main script for training and predictions
├── sonar_data.csv              # Dataset for classification
└── requirements.txt            # Python dependencies
```

The dataset consists of continuous numerical features extracted from sonar signals and a binary target variable:
- **Features**: 60 numerical columns representing sonar data.
- **Label**: 'R' for Rock and 'M' for Mine.

Example rows from the dataset:

| Feature 1 | Feature 2 | ... | Feature 60 | Label |
|-----------|-----------|-----|------------|-------|
| 0.0200    | 0.0371    | ... | 0.0032     | R     |
| 0.0453    | 0.0523    | ... | 0.0044     | R     |
| 0.0262    | 0.0582    | ... | 0.0078     | R     |

The model achieved the following results:
- **Training Accuracy**: 84.34%
- **Test Accuracy**: 69.05%

The project demonstrates a simple implementation of logistic regression for binary classification. Future improvements may include:
- Trying more advanced machine learning models such as Random Forests, Support Vector Machines, or Neural Networks.
- Using hyperparameter tuning or cross-validation to optimize the model's performance.
- Implementing feature scaling or dimensionality reduction techniques like PCA.

This project is licensed under the MIT License. For more details, refer to the LICENSE file in the repository.

Acknowledgments: The dataset used in this project was obtained from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Connectionist+Bench+(Sonar,+Mines+vs.+Rocks)).
