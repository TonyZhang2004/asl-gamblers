# ***asl-gamblers***
## About

This is a website created by *[Guanyu Zhang](https://github.com/TonyZhang2004)*, for collaboration with He Li and Taiye Chen, in Kaggle's **[American Sign Language competition](https://www.kaggle.com/competitions/asl-fingerspelling)** held by Google.

***NOTE***: Keep checking **Discussion** on the website for newly-asked questions by other competitors.

## Collection of some useful references with brief intro

### **[Getting Started with Kaggle workflow](https://www.kaggle.com/competitions/titanic)**

A competition for those who are new to Kaggle, predicting the survivors on Titanic, just press the "join competition" and follow the instructions to submit a prediction in ".csv" format.

### **[TensorFlow Lite](https://www.tensorflow.org/lite)**

The model to be submitted should be a **TensorFlow Lite** model.

### **[Keras](https://keras.io/)**

APIs for DL with TensorFlow.

### **[Parquet File Format](https://towardsdatascience.com/demystifying-the-parquet-file-format-13adb0206705)**

1. The data in this competition is stored with **".parquet"** format, which is well-known for **efficient storage** and **fast read speed**.
2. ***".parquet"*** is 50x faster when using ***pd.read_parquet()*** than ***".csv"*** when using ***pd.read_csv()***.

### **[MediaPipe Holistic Model](https://github.com/google/mediapipe/blob/master/docs/solutions/holistic.md)**

The source of data, could be useful for feature engineering and data preprocessing.


### **[A baseline using LSTM for ASL](https://www.kaggle.com/code/stanptown/lstm-baseline-for-starters-sign-language-eeff0f)**

Using **Long Short-Term Memory** for this competition, could modify this for improvements.

### **[XGBoost](https://xgboost.readthedocs.io/)**

A **gradient-boosting** library which implements lots of ML algorithms.

### **[LightGBM](https://lightgbm.readthedocs.io/en/stable/)**

A **gradient-boosting** library which implements lots of ML algorithms.

## Workflow of this ASL competition
### 1. Preprocess the Data

We gotta preprocess the data first (those **.parquet** files), and this may include file-reads (**Pandas** related, and some plotting library could be useful to data-visualization, such as **matplotlib** and **seaborn**), data-cleaning (fill the NaNs, abandon some outliers, etc.), and convert the parquet files to some convenient formats (such as np.arrays or tensors) for the model to take as inputs.

### 2. Fit a Model
### 3. Submit the Prediction

## Brainstorm🧠
### Guanyu Zhang

1. We gotta measure the difference between two strings in the model (the prediction and the ground truth of train data), so we might wanna use an evaluation metric that can measure this kind of difference (for example, the [Levenshtein Distance](https://en.wikipedia.org/wiki/Levenshtein_distance)).

### He Li

### Taiye Chen

