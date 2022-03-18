# Breast tumor detection using CNN model

 Early detection of breast canser helps in reducing the number of early deaths.
I designed a CNN deep-learning model that classifies the ultrasound images into one of the three classes: normal, benign, and malignant. The model has scored an over all accuracy of 60.5%  on a test set of 330 ultrasound images.

## Tecnologies 

- Tesnsorflow v2 , keras
- numpy
- pandas
- matplotlib

## The Data
<p>
The number of patients is 600 female patients. The dataset consists of 780 images with an average image size of 500*500 pixels. The images are in PNG format. The ground truth images are presented with original images. The images are categorized into three classes, which are normal, benign, and malignant.
</p>

[for more details](https://scholar.cu.edu.eg/?q=afahmy/pages/dataset)

###### Al-Dhabyani W, Gomaa M, Khaled H, Fahmy A. Dataset of breast ultrasound images. Data in Brief. 2020 Feb;28:104863. DOI: 10.1016/j.dib.2019.104863.

#### Data Pipeline & Augmentation
- Generated 1/3 of the data by flipping and rotation of the images by  random set of angles 

- Downsized the input images and normalized it to (32,32,3)
## Model Design 
<p>
I have used 2 CNN layers with 8-16 filters followed by Max polling and batch normalization. 
    For the fully connected layer I used 2 dense layers 64 node each added drop out Layer after each layer with a dropout rate of 0.5.
</p>
<div align="center">
    <p>
    model summery
    </p>
    <img src="results\summary.jpg" width="45%" title="model summery">
</div>

## OUPUT 

<p>
    The following images represents the model performabce on a subset of Ultrasound images. The model has scorred an accuracy ranges between 60-65% 
</p>


<div align="center" >
<table align="center"  >
  <tr align="center" >
     <td>model correct prediction for benign case</td>
     <td>model correct prediction for malignant case</td>
     <td>model wrong prediction for normal case</td>
  </tr>
  <tr align="center" >
    <td><img src="results\benign.jpg" title="benign"></td>
    <td><img src="results\malignant.jpg" title="benign"></td>
    <td><img src="results\normal.jpg" title="benign"></td>
  </tr>
 </table>
 </div>