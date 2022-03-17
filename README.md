# Breast tumor detection using CNN model

## Tecnologies 

## The Data

## Model Design 
I have used 2 CNN layers with 8-16 filters followed by Max polling and batch normalization. 
    For the fully connected layer I used 2 dense layers 64 node each added drop out Layer after each layer with a dropout rate of 0.5.
<div align="center">
    <p>
    model summery
    </p>
    <img src="results\summary.jpg" width="30%" title="model summery">
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