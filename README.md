# Abnormal-Event-Detection

This repository has two folders: one for the Spatio Temporal Autoencoder for abonormal event classification and another for time series analysis on pose estimation. Both tasks revove around the Avenue dataset. 


## Spatio Temporal Autoencoder 
This model is based on the paper at the link <https://arxiv.org/pdf/1701.01546.pdf>
However, some changes were made to the model and loss fucntions. Specifically, I changed the loss function from mean squared error into categorial cross-entropy as I thought it was appropriate since we are prediciting categories of abnormal events. 

First the model is described as the one in the paper: 
![alt text](https://media.springernature.com/original/springer-static/image/chp%3A10.1007%2F978-3-319-59081-3_23/MediaObjects/450610_1_En_23_Fig1_HTML.gif)
After preprocessing the data running `python preprocessing.py /source/to/dataset/ fps`, this model was then trained on the Avenue dataset for 32 epochs by running `python train_model.py`

