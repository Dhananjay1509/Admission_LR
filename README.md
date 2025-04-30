# University Admission Prediction System

[![Streamlit](https://img.shields.io/badge/Streamlit-1.29.0-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://streamlit.io/)
[![Pandas](https://img.shields.io/badge/pandas-2.1.4-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/numpy-1.26.2-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![Scikit-learn](https://img.shields.io/badge/scikit--learn-1.6.1-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.13.2-7db0bc?style=for-the-badge&logo=python&logoColor=white)](https://seaborn.pydata.org/)

A machine learning-based web application that predicts university admission chances based on various academic parameters using Linear Regression.

![Admission Prediction](https://tse1.mm.bing.net/th?id=OIP.h2gG87iB1-mfwYJfMMEepQHaCD&pid=Api&P=0&h=180)

## Features

- Interactive web interface built with Streamlit
- Real-time prediction of admission chances
- Comprehensive data analysis and visualization
- Model evaluation metrics
- Feature importance analysis
- User-friendly input forms
- Detailed parameter explanations

## Technical Details

### Model Performance
- R-squared Score: Indicates how well the model fits the data
- Mean Squared Error (MSE): Measures prediction accuracy
- Root Mean Squared Error (RMSE): Standard deviation of prediction errors
- Cross-validation scores: Validates model performance across different data splits

### Analysis Components
- Correlation analysis using heatmaps
- Distribution analysis of features
- Feature importance visualization
- Residual analysis
- Q-Q plots for normality testing

## Prediction Parameters

The system considers the following factors:
- GRE Score (0-340)
- TOEFL Score (0-120)
- University Rating (0-5)
- Statement of Purpose (SOP) strength (0-5)
- Letter of Recommendation (LOR) strength (0-5)
- CGPA (0-10)
- Research Experience (0 or 1)

## Project Structure

```
Admissionlr/
├── main.py                    # Main Streamlit application
├── AdmissionPredModel.ipynb   # Model development notebook
├── finalized_model.pickle     # Trained machine learning model
├── scaler_model.pickle        # Data scaler for preprocessing
├── requirements.txt           # Project dependencies
└── README.md                  # Project documentation
```

## Installation

1. Create a virtual environment:
```bash
python -m venv Admission
```

2. Activate the virtual environment:
```bash
# On Windows
Admission\Scripts\activate 

# On Unix or MacOS
source Admission/bin/activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

## Usage

1. Start the application:
```bash
streamlit run main.py
```

2. Navigate through the application:
   - Home: Introduction to the system
   - Predict Admission: Enter your academic parameters
   - About: Detailed information about parameters

3. For prediction:
   - Enter your academic scores and ratings
   - Click the predict button
   - View your predicted admission chances

## Model Development

The model was developed using:
- Linear Regression algorithm
- Feature scaling using StandardScaler
- Cross-validation for model validation
- Comprehensive error metrics
- Multicollinearity analysis using VIF

## Dependencies

- Python 3.x
- streamlit
- pandas
- numpy
- scikit-learn
- seaborn
- matplotlib
- statsmodels

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Dataset source: Graduate Admission Dataset
- Streamlit for the web framework
- Scikit-learn for machine learning tools
