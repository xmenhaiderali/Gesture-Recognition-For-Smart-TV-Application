# Gesture Recognition for Smart TV Application
> This project was performed to develop a cool feature for TV application which can recognise five different gestures performed by the user which will help users control the TV without using a remote

> The project pipelines include Data Generator and CNN models with different architecture. Different CNN architecture tried are:
    - Simple Conv3D + MaxPooling3D Model
    - Multiple Conv3D + MaxPooling3D Model
    - Conv2D + RNN(GRU)
    - Conv2D + RNN(LSTM)

* Simple Conv3D + MaxPooling3D Model

1) The training accuracy is 20.66% and validation accuracy is 23% which resembles simple conv3d is an underfit model which means modern is learning out of data we can add some more layers to avoid underfitting

2) The validation loss 1.6076 which can further decreased to avoid underfitting.

* Multiple Conv3D + MaxPooling3D Model

1) As we can see from Training and Validation Accuracy, Training accuracy came as 83.56% with validation accuracy as 65% which has removed the underfitting validation accuracy can be further improved by doing few techniques like data augmentation and training for large no of epochs.

2) As we can see from Training loss it is very close to zero but not exactly zero. As the epochs increase validation loss reached towards training loss which is around 1.19(val_loss)

* Conv2D + RNN(GRU)

1) In this Conv2D , RNN (GRU) has been used in convolutiona architecture.

2) As we can see from Training and Validation Accuracy, Training accuracy came as 96.23% with validation accuracy as 62% which has removed the underfitting validation accuracy can be further improved by doing few techniques like data augmentation and training for large no of epochs.

3) As we can see from Training loss it is very close to zero but not exactly zero. As the epochs increase validation loss reached towards training loss which is around 1.33(val_loss)

Hence, if we compare Multiple Conv3D + MaxPool3D with Conv2D + RNN(GRU) , Multiple Conv3D + MaxPool3D outperforms other models(Multiple Conv3D + MaxPool3D , Conv2D + RNN(GRU)) in terms of accuracies, overfitting and underfitting.

* Conv2D + RNN(LSTM)

1) In this Conv2D , RNN (LSTM) has been used in convolutiona architecture.

2) As we can see from Training and Validation Accuracy, Training accuracy came as 92.46% with validation accuracy as 67% which has removed the underfitting validation accuracy can be further improved by doing few techniques like data augmentation and training for large no of epochs.

3) As we can see from Training loss it is very close to zero but not exactly zero. As the epochs increase validation loss reached towards training loss which is around 1.0806(val_loss)

> All these CNN models have been tried on cropped images but cropping images decreased accuracy of models and validation loss also increased.

> Hence, if we compare Multiple Conv3D + MaxPool3D , Conv2D + RNN(GRU) & Conv2D + RNN(LSTM) , Conv2D + RNN(LSTM) outperforms other models in terms of accuracies, validation loss, overfitting and underfitting.Also, the weight initialization have been done using he-uniform technique.

Conclusion : Conv2D + RNN(LSTM) we will use for Gesture Recognition TV Application.


## Table of Contents
* [Technologies Used](#Python, CNN, RNN)
* [Conclusions](#Attached in Word file on git repository)


## Project Information
- Built Generator pipeline to generate training and validation data
- Used multiple CNN models to experiment on data
- Provided conclusion for best model