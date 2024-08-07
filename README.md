# CodSoft Internship 🚀

This project is the first of three projects I am working on during my internship at Codsoft. The internship provides an opportunity to apply theoretical knowledge to real-world problems, enhance technical skills, and gain valuable industry experience.


## SMS Spam Prediction Machine Learning Project 📱🤖

This project is the first of three projects undertaken during my internship at Codsoft. It focuses on building a machine learning model to predict SMS spam messages. The dataset used for training and evaluation is imported from Kaggle. The project leverages various technologies such as numpy, pandas, os, and nltk for data manipulation and natural language processing.

![alt text](/SpamSms/image.png)

## Table of Contents

1. [Project Overview](#project-overview)
2. [Technologies Used](#technologies-used)
3. [Setup and Installation](#setup-and-installation)
4. [Dataset](#dataset)
5. [Data Preprocessing](#data-preprocessing)
7. [Results](#results)

## Project Overview 📝

The objective of this project is to classify SMS messages as spam or not spam using machine learning techniques. The project involves data preprocessing, feature extraction, model training, and evaluation.

## Technologies Used 🛠️

- **Python**: The primary programming language used.
- **numpy**: For numerical operations.
- **pandas**: For data manipulation and analysis.
- **os**: For handling file paths and directories.
- **nltk**: For natural language processing tasks.

## Setup and Installation ⚙️

1. Clone the repository to your local machine:
    ```bash
    git clone https://github.com/ayusharma03/sms-spam-prediction.git
    ```

2. Navigate to the project directory:
    ```bash
    cd sms-spam-prediction
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Ensure you have the necessary NLTK data:
    ```python
    import nltk
    nltk.download('stopwords')
    nltk.download('punkt')
    ```

## Dataset 📊

The dataset used in this project is sourced from Kaggle. It contains a collection of SMS messages labeled as spam or not spam.

You can refer to the link [Dataset](https://kaggle.com/datasets/uciml/sms-spam-collection-dataset/code) 

To load the dataset, the following code is used:
```python
import os
for dirname, _, filenames in os.walk('/kaggle/input'):
    for filename in filenames:
        print(os.path.join(dirname, filename))
        
df1 = pd.read_csv("/"relative_path"/spam.csv", encoding='latin1')
```

## Data Preprocessing 🧹

Data preprocessing involves cleaning the text data, tokenizing, removing stop words, and vectorizing the text. The `nltk` library is used extensively for these tasks.


## Results 📈

I've got a 0.9524% accuracy on the test dataset, highlighting the effectiveness of the model in identifying spam messages.


---

Feel free to reach out if you have any questions or suggestions. Happy coding! 💻