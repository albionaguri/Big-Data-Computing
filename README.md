# Fake-News-Classifier using PySpark

## Outline

* <li> <a href = "#Introduction"> Introduction </a> </li>
* <li> <a href = "#Dataset"> Dataset </a></li>
* <li> <a href = "#Preprocessing-and-Feature-Engineering"> Preprocessing and Feature Engineering </a></li>
*  <li> <a href = "#Models"> Models </a></li>
* <li> <a href = "#Experimental-results">  Experimental results </a> </li>
* <li> <a href = "#Summary-Results">  Results Summary </a>  </li>
* <li> <a href = "#Conclusion"> Conclusions and Future Scope </a></li>
* <li> <a href ="#Application"> Application </a> </li>
* <li> <a href ="#Technologies"> Technologies Used </a> </li>
* <li> <a href ="#Demo"> Demo </a> </li>



## Introduction

- The main objective of our project is to determine if a given text data by the user is fake or real.
- It consists of a binary classification problem.
- In order to automate the news qualifying procedure we implemented 4 machine learning algorithms to predict the news.

## Dataset

- The dataset we used is derived from Kaggle resource and is composed by text data.
- It consists of around 44900 training examples.
- The ratio between minority class and majority is particularly small.

## Pre-Processing and Feature Engineering 

<img width="393" alt="image" src="https://user-images.githubusercontent.com/51866742/235445652-5e1e62c0-eea5-41a9-9f28-e22bb38c3207.png">

## Models

1. Logistic Regression
2. Random Forest Classifier
3. Multilayer Perceptron Classifier
4. Transformers (Hugging Face)

## Experimenal Results

- Results are obtained from the Logistic Regression model in training and testing set.

<img width="429" alt="image" src="https://user-images.githubusercontent.com/51866742/235447157-8b17dc91-d3aa-413b-859c-aacfaa0aafd2.png">

- Results are obtained from the Random Forest model in training and testing set.

<img width="428" alt="image" src="https://user-images.githubusercontent.com/51866742/235447356-1622b746-9ea3-4478-8d0e-c1d0f48b0a96.png">

- Results are obtained from the Multilayer Perceptron model in training and testing set.

<img width="428" alt="image" src="https://user-images.githubusercontent.com/51866742/235446966-254a0b6c-e6f7-428a-82a1-f24ff705b90a.png">

## Results Summary 
<img width="345" alt="image" src="https://user-images.githubusercontent.com/51866742/235447486-f7de206f-ba30-453e-bb59-58264598fc1d.png">

## Conclusion and Future Scope

All models performed well as seen from the results in the graphics. This was due to the fact that the models were trained in the <i> whole dataset </i> including training and testing partitions. After obtaining these almost perfect results, what can be done in the future would be:
1. First step is to split the dataset into training and testing.
2. Train the model *only* with the training set, apart from the test set. In this way the model that is being trained cannot see data that belongs to the test set. 
3. After training the model, then I made predictions using the test set.
4. Since, test set was unknown to the model when training, then I assume I would have obtained slightly differences in comparison with the ones I got.

## Application 

I built a small Application that can be used to get informed if the news are real or fake. The used model in our specific case is Transformers. 
Then, I saved all the models, so we can adapt the Application for using each of them. 

### Technologies used: 

- Flask
- React.js
- Docker

## Demo 

<div>
  <img width="431" alt="image" src="https://user-images.githubusercontent.com/51866742/235449299-bc9bb57a-6eec-4d8a-b33f-8402e4f25965.png">

  <img width="433" alt="image" src="https://user-images.githubusercontent.com/51866742/235449405-1091fc64-6da3-4c76-8ca6-4f0787ef95ea.png">
  <img width="431" alt="image" src="https://user-images.githubusercontent.com/51866742/235449531-a13e5a8a-77b7-4564-8e07-b47000509efb.png">
  <img width="428" alt="image" src="https://user-images.githubusercontent.com/51866742/235449583-e3ee31d7-c503-4079-a334-9ed520ff9d04.png">
</div>
<hr>
<div>
  <img width="431" alt="image" src="https://user-images.githubusercontent.com/51866742/235449795-b3127bae-0c78-45e7-a2da-01b0cdc912f5.png">
  <img width="428" alt="image" src="https://user-images.githubusercontent.com/51866742/235449848-2b40df91-677f-4300-8c38-1df0acfc0ca5.png">

</div>






