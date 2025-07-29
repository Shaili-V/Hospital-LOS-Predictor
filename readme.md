## Project Overview
The goal of this project is to predict the Length of Stay (LOS) for patients in a hospital, using a dataset of inpatient discharges. By using machine learning algorithms (Classic ML, Neural Networks (NN), XGBoost, Recurrent Neural Networks (RNN), and Convolutional Neural Networks (CNN)), we aim to explore how various factors--such as age, gender, type of admission, and medical conditions--afftect the length of a patient's hospital stay

## Dataset
The dataset used is the Hospital Inpatient Discharges Dataset created by Bhautik A. Mangukiya, a data scientist. It provides comprehensive, de-identified information with 33 columns and over 2.1 million rows. A smaller subset of 12 columns was primarily used for this project. The orignal dataset was found on Kaggle at this link: https://www.kaggle.com/datasets/bhautikmangukiya12/hospital-inpatient-discharges-dataset

## Steps Before Running Any Files
- Ensure a Python environment is installed on your device
- Create a virtual environment
- Install the following libraries:
    - numpy
    - pandas
    - scikit-learn
    - tensorflow
    - xgboost
    - scipy
    - missingno
    - matplotlib
    - plotly
    - seaborn
    - warnings
- Ensure that the original dataset from the Kaggle link provided is in the folder, and the datset should be renamed to "hospital_csv"

## Order to Run Files
- Run files in order of the number label or follow this list:
    - 1_data_analysis.ipynb
    - 2_data_cleaning.ipynb
    - 3_data_realizations.ipynb
    - 4_classic_ml.ipynb
    - 5_nn.ipynb
    - 6_nn2.ipynb
    - 7_nn3.ipynb
    - 8_xg_boost.ipynb
    - 9_rnn.ipynb
    - 10_cnn.ipynb
- The 2_data_cleaning.ipynb must be run before any of the subsequent files in the list in order to produce the correct, cleaned datasets.

## Other Instructions
- In the pd.read_csv("{DATASET}") line near the beginning of each of the files labeled 3-10, the "hospital_cleaned.csv" and the "hospital_los_21.csv" can be interchanged
- The "hospital_cleaned.csv" is a cleaned version of the original dataset with 12 columns kept from the original 33.
- The "hospital_los_21.csv" is the "hospital_cleaned.csv" with only rows where the "length_of_stay" column contained values of 21 days or less.