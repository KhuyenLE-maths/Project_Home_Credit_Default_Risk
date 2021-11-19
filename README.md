# Project: Home Credit Default Risk

Predict if an applicant is capable to repay a loan

## Context: 

This project is inspired by a Kaggle competition https://www.kaggle.com/c/home-credit-default-risk/data

The principal purpose of this project is to visualize large datasets with different python tools to extract meaningful statistical information from the data. Besides, a variety of preprocessing techniques are also applied to deal with the missing values, outliers, and imbalance of the dataset. Finally, the cleaned data is classified based on the Adaboost method which is one of the most recent algorithms for classifying large datasets.

You can also refer to my notebook https://github.com/KhuyenLE-maths/Project_Income_Classification for further information about some popular machine learning algorithms for classifying data, as well as the comparison between them. 

Download data from Google colab: 
- Step 1: Access to your kaggle account, go to API section and create new API token, a file named "kaggle.json" will be load on your computer
- Step 2: Install kaggle on google colab and upload file "kaggle.json" as follow:
```python
!pip install kaggle

# upload file "kaggle.json"

from google.colab import files 
files.upload()  
```
- Step 3: Make a new directory named "kaggle" and copy file "kaggle.json" to this directory, then change the permission of the file. 
```python
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/

# change the permission
!chmod 600 ~/.kaggle/kaggle.json
```
(the comment ```!chmod 600```means that only the owner of the file (kaggle.json) has the acess right to read anh write on it)

- Step 4: Download the dataset
 ```python 
 !kaggle competitions download -c home-credit-default-risk
 ```
