# Milestone-Food101-


<p align="center">
  <img src="https://github.com/docum5/Milestone-Food101-/blob/main/food101.jpeg?raw=true" />
</p>

## The Problem 
Recent growth in nutrition-related diseases globally has increased awareness of healthy nutritional habits. Healthy diets reduce the risks of reactions to food intolerance, weight problems, malnutrition and some forms of cancer. There are several applications in existence with which we can manually keep track of what we eat and identify food items before consumption. These applications, however, require that previous experience with the food item for easy identification. An important question, however, is: what happens if we see a food item for the first time and need to identify it? Automated tools of food identification will be of help in such cases. The advent of Convolutional Neural Networks (CNN) and deep learning-based architectures have opened opportunities for the realization of such automatic tools. Indeed, a lot of mileage has already been made in neural networks based image food classification. However, there are still gaps in the accuracy of existing methods implemented. The recent state of the art results is ~76,3% for top-1 accuracy and 94,6% for top-5 accuracy. In response, I propose a technique based on a pre-trained EfficientNetB0 architecture that achieves the following accuracy on the test set:

## Goal
To beat the original results of the [Food101](https://data.vision.ee.ethz.ch/cvl/datasets_extra/food-101/) paper and beating [DeepFood](https://www.researchgate.net/publication/304163308_DeepFood_Deep_Learning-Based_Food_Image_Recognition_for_Computer-Aided_Dietary_Assessment), a 2016 paper that used a Convolutional Neural Network trained for 2-3 days to achieve 77,4% top-1 accuracy.

## Project Main Steps:

- Use TensorFlow Datasets to Download Data
- Exploring the Food101 data from TensorFlow Datasets
- Plot an image from TensorFlow Datasets
- Create preprocessing functions for our data
- Batch & prepare datasets
- Create modelling callbacks
- Build feature extraction model
- Fit the feature extraction model
- [View training results on TensorBoard](https://tensorboard.dev/experiment/5sNyi2UKSJiYszbqp0pu9A/#scalars)

## Modeling

### 1. Feature Extraction



| Epoch | Accuracy |
|-------|----------|
| 1     | 67.9%    |
| 2     | 69.3%    |
| 3     | 71.5%    |


### 2. Fine-tuning
| Epoch | Accuracy |
|-------|----------|
| 1     | 77.6%    |
| 2     | 77.9%    |
| 3     | 78.8%    |
| 4     | 78.95%   |
| 5     | 80.35%   |

### Final model

| Final Evaluate |        |
|----------------|--------|
| Accuracy       | 79.85% |


## Conclusion

We Built a feature extraction from EfficientNetB0 model and achieved 70,87 % accuracy after three epochs and tried fine-tuning the model, and the accuracy increased to 79,85%. This beats the original results of the Food101 paper, With an average accuracy of 50.76%, and beating the DeepFood, a 2016 paper that used a Convolutional Neural Network trained for 2-3 days to achieve 77.4% top-1 accuracy.


## Technologies Used

![](https://forthebadge.com/images/badges/made-with-python.svg)

[<img target="_blank" src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/440px-NumPy_logo_2020.svg.png" width=150>](https://numpy.org/) [<img target="_blank" src="https://camo.githubusercontent.com/aeb4f612bd9b40d81c62fcbebd6db44a5d4344b8b962be0138817e18c9c06963/68747470733a2f2f7777772e74656e736f72666c6f772e6f72672f696d616765732f74665f6c6f676f5f686f72697a6f6e74616c2e706e67" width=200>](https://www.tensorflow.org/) [<img target="_blank" src="https://matplotlib.org/stable/_static/logo2.svg" width=100 height=50>](https://matplotlib.org/)
