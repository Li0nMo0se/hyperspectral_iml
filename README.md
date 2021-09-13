# Machine learning applied to hyperspectral images

## Authors:

* louis.guo
* raphael.ramelet
* ilan.guenet

## Goals

In this project, the goal is to develop a classification pipeline of hyperspectral images. There are two given hyperspectral images given. Those hyperspectral images were acquired by the AVIRIS sensor. The specifications are 224 bands between 0.4μm to 2.5μm with a 10nm band width.

On these images, there are 16 different categories and a classifier classifying the pixels of the images must be found. The classifier must be the most accurate and the most generic. Deep learning is also forbidden (for educational purposes).

Many experiments will be performed in order to find the best classifiers with preprocessing, transformers, and searching of the best classifier.

## Table of content:

* Load data
* Preprocessing
  * Gaussian blur
* Transformers
  * Reshape inputs
  * Standard Scaler
  * Dimension reduction (PCA)
  * SelectKBest
* Classification API
    * Grid search with cross-validation
    * Evaluation
* Multiclass classification
    * With other VS without other
        * LinearSVC
        * RandomForest
    * Indiana classification (bench)
        * LinearSVC (One Versus All)
        * RandomForest (Inherently multiclass)
        * K-nearest neighbors (Inherently multiclass)
        * SVC (One Versus One)
        * Recap of indiana classifiers
    * Salinas classification
        * SVC (One Versus One)
        * RandomForest (Inherently multiclass)
        * Recap of salinas classifiers
* Impact of the gaussian blur
* Performance of the best classifier
* Tasks distribution

## Resources:

* Pre-processing of hyperspectral images. Essential steps before image analysis by Maider Vidal ([link](https://www.researchgate.net/publication/236244862_Pre-processing_of_hyperspectral_images_Essential_steps_before_image_analysis))
* Scikit-learn documentation ([link](https://scikit-learn.org/stable/))
* IML course from EPITA

