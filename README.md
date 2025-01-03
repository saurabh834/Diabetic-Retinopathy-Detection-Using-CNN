# Diabetic Retinopathy Web App
Webapp for classification of Diabetic Retinopathy from retinal images using flask and keras.


## Diabetic Retinopathy
Diabetic retinopathy is an eye condition that can cause vision loss and blindness in people who have diabetes. It affects blood vessels in the retina.

 <p align="center">
  <img src="[[https://ars.els-cdn.com/content/image/1-s2.0-S2772442524000054-gr6.jpg](https://www.researchgate.net/publication/363858079/figure/fig5/AS:11431281147393709@1681610800275/Typical-model-architecture-for-Diabetic-Retinopathy-detection.png)](https://www.mdpi.com/applsci/applsci-13-05685/article_deploy/html/images/applsci-13-05685-g001-550.jpg)">
</p>
## Data Description

Dataset consists of retina images taken using fundus photography under a variety of imaging conditions.

A clinician has rated each image for the severity of diabetic retinopathy on a scale of 0 to 4:

    0 - No DR

    1 - Mild

    2 - Moderate

    3 - Severe

    4 - Proliferative DR

## About the Model used for prediction
### Densely Connected Convolutional Networks or DenseNet 

Dense Convolutional Network (DenseNet), which connects each layer to every other layer in a feed-forward fashion. Whereas traditional convolutional networks with L layers have L connections - one between each layer and its subsequent layer.

A more efficient model variant DenseNet-BC (DenseNet-Bottleneck-Compressed) networks are trained. Using the DenseNet-BC-121-32 model as the base model.

Advantages of DenseNet-BC are:
 - Reduced number of parameters
 - Similar or Better performance
 - Better accuracy
 
 Dense Net architecture as shown in the original paper which shows the connections from each layer to every other layer:
 
 <p align="center">
  <img src="https://ars.els-cdn.com/content/image/1-s2.0-S2772442524000054-gr6.jpg">
</p>

## Requirements Insatallation
### Using conda or virtualenv
```
virtualenv venv
source /bin/activate
python3 -m pip install -r requirements.txt
```
### Direct (Not recommended)
`python3 -m pip install -r requirements.txt`

## Run the Webapp by executing 
`python3 app.py`

## Refrences
- [Diabetic Retinopathy Wikipedia](https://en.wikipedia.org/wiki/Diabetic_retinopathy)
- [Diabetic Retinopathy National Eye Institute](https://www.nei.nih.gov/learn-about-eye-health/eye-conditions-and-diseases/diabetic-retinopathy)
- [Fundus Image Dataset from Kaggle](https://www.kaggle.com/c/aptos2019-blindness-detection/data)
- [Densely Connected Convolutional Networks (DenseNets)](https://github.com/liuzhuang13/DenseNet)
