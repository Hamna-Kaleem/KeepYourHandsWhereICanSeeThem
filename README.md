# KeepYourHandsWhereEyeCanSeeThem

This repository contains **American Sign Language Recognition** code with **Transfer Learning** to build deep learning models using keras. Three state of the art CNN architectures i.e. **VGG16, Resnet50, InceptionV3** is selected to perform single hand alpha-numeric sign detection on ASL Dataset. **Data augmentation** techniques are also used to compare the results of selected models. Accuracy of the models are compared among the models on the basis of best test accuracy of the model on given dataset and on augmented dataset.

**Dataset** contains RGB-D data of static hand gestures performed by 5 different signers and letter X and Z is excluded due to the dynamic nature of their sign character, so total number of classes is 24. This is Kaggle dataset with useablity factor of 7.5.

**Transfer Learning** : VGG16, InceptionV3, Resnet50 is used. Softmax and dense layer is added at the end of the model to predict six classes of given data.

**Data Augmentation** : Horizontal, Vertical flip set to True, scaling is set to 01% and rotation of 90 degree is applied.

**Customized Dataset** : For better test results, we also run CNN architectures on Customized Dataset. This dataset contain American Sign Lnaguage characters, total of 6 different classes were chosen for testing i.e. A,E,H,M,N,O

![Screenshot](https://github.com/Hamna-Kaleem/KeepYourHandsWhereICanSeeThem/blob/main/customize.png?raw=true)

**Best Results** : VGG19 has the best test accuracy with 99% accurate classification results.

![Screenshot](https://github.com/Hamna-Kaleem/KeepYourHandsWhereICanSeeThem/blob/main/vgg19.png?raw=true)

**Strange Shift in Accuracy** : Resnet50 become victim of overfitting but still show high testing accuracy with augmented data i.e. approximately 96.86% and without augmentation model was unable to perform well in testing phase and had testing accuracy just 5.01% with the highest test loss of 76.47

![Image](https://github.com/Hamna-Kaleem/KeepYourHandsWhereICanSeeThem/blob/main/resnet50.png?raw=true)
