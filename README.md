# Kaggle Competition | ISIC-2024
This is my solution to the ISIC-2024 competition on Kaggle.
The solution involves an ensemble of LGBM and a CNN, particularly an EfficientNet V2 B0 pre-trained on ImageNet, and fine-tuned on the skin cancer dataset provided by the competition host.
The LGBM ensemble takes as input the metadata provided, plus the predictions of the CNN on the skin cancer dataset.

There are 3 notebooks here:
* File _train_CNN.ipynb_ contains the code to train the CNN that makes predictions on the skin cancer images, using a subset of the training set with defined proportions of negative and positive samples.
* File _train_CNN_whole_training_set.ipynb_ contains the code to train the CNN that makes predictions on the skin cancer images using the entire training set.
* File _train_LGBM_and_predict.ipynb_ contains the code to train the ensemble of LGBM on the metadata plus the predictions of the CNN on the images. It also makes predictions on the test set to send the submission.
