# Anti Spoofing Project
This project is a anti spoofing project made for detecting real and fake faces. one of the requirements of a face detection algorithm is to detect if the face is real or not (for example if its printed image on paper, etc.)
Two methods is used for this purpose:
## 1) Feature Extraction:
In this method every image is converted to feature vector using its HOG, LBP histogram and this feature vector is given to a SVM for classification. the results of this method was so effective with high accuracy.
## 2) Deep Learning:
In this method a deep learning model is used for classification. The model consist of 3 parts: spatial transformer layer, InceptionV3 with weights of image net, two dense layers for classification.
The second part of this model (InceptionV3) is freezed and did not trained during training the model. The accuray of model during training reached 90% on validation data set.
you can download the trained deep model from this link:
https://drive.google.com/file/d/1ga6l3FXcqKPrcvTKBpkLeaoCvLt8DbEn/view?usp=sharing
## Data Set
data set used for training the model is CASIA-FASD data set you can get it from this link:
https://paperswithcode.com/dataset/casia-fasd
