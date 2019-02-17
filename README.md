# Automated Essay Scoring
> A Deep Learning model that predicts the score of a given input essay. 

The dataset is from Kaggle ASAP competition which was provided by The Hewlett Foundation.

The **mysite** folder contains the Django app if you want an interactive demo.

### Performance
The accuracy is calculated by **Quadratic Weighted Kappa(QWK)**, which measures the agreement between two raters. The state of the art implementation in this competition achieved a **QWK score of 0.82** six years ago. My model achieves a **QWK score of 0.961**. The model architecture consists of 2 Long Short Term Memory(LSTM) layers with a Dense output layer. The final layer uses the Relu activation function. The QWK is calculated by training model on the dataset using 5-Fold Cross Validation and taking the average for all five folds.


### Performance Correction
The performance above might not be accurate. Please review [this issue](https://github.com/mankadronit/Automated-Essay--Scoring/issues/1) to know more.

<img src="https://github.com/mankadronit/Automated-Essay--Scoring/blob/master/ScreenShots/SC1.png" width="100%">
<img src="https://github.com/mankadronit/Automated-Essay--Scoring/blob/master/ScreenShots/SC2.png" width="100%">
<img src="https://github.com/mankadronit/Automated-Essay--Scoring/blob/master/ScreenShots/SC3.png" width="100%">


## Requirements
please goto `requirements.txt`

## Installation 
- Clone the repo
- Just run the **Jupyter Notebook** to train the model.
- To run the Django App cd ./ into the **mysite** folder and run ```python manage.py runserver```

## References
1. [A Neural Approach to Automated Essay Scoring](http://aclweb.org/anthology/D/D16/D16-1193.pdf) </br>
2. [Automatic Text Scoring Using Neural Networks](https://arxiv.org/pdf/1606.04289.pdf)
