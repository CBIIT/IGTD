# Image Generator for Tabular Data (IGTD): Converting Tabular Data into Images for Deep Learning Using Convolutional Neural Networks

## Description

Image Generator for Tabular Data (IGTD) is an algorithm for transforming tabular data into images. The algorithm assigns each feature to a unique pixel position in the image representation. The algorithm assigns similar features to neighboring pixels, and assigns dissimilar features to pixels that are far apart. As a result of these assignments, the algorithm generates an image for each sample, in which the pixel intensity reflects the value of the corresponding feature in the sample. One of the most important applications for the generated images is to build convolutional neural networks (CNNs) based on the image representations in subsequent analysis. A publication about the IGTD algorithm is available at https://www.nature.com/articles/s41598-021-90923-y.

## User Community
Users interested in the following subjects:
- Primary: machine learning; computational data modeling
- Secondary: bioinformatics; computational biology

## Usability

To use the software package in this repository,  users must meet the following criteria:
* Possess the basic skills to program and run Python scripts. 
* Able to process the input data into the data format accepted by the package. 
* Understand the input parameters of the IGTD algorithm, so that they can set the parameters appropriately to execute the algorithm.

## Uniqueness

IGTD is a novel algorithm for transforming tabular data into images. Compared with existing methods for converting tabular data into images, IGTD has several advantages. 
- IGTD does not require prior knowledge about the features. Thus, users can use it even without domain knowledge. 
- IGTD generates compact image representations, in which each pixel represents a unique feature. Deep learning based on compact image representations usually requires less memory and time to train the prediction model.
- IGTD has been shown to generate compact image representations promptly, which also better preserve the feature neighborhood structure. 
&#x1F534;_**(Question: Can we specify who or what showed it, to avoid the passive "has been shown" wording?)**_
- CNNs trained on IGTD images achieve a better (or similar) prediction performance than both CNNs trained on alternative image representations and prediction models trained on the original tabular data. 
- IGTD provides a flexible framework that users can extend to accommodate diversified data and requirements. In this flexible framework, users can choose size and shape of the image representation.  

## Components

The Scripts folder in this repository includes the following Python scripts: 
* IGTD_Functions.py provides all the functions used by the IGTD algorithm. It provides comments explaining the input and output of each function.
* Example_Run.py provides examples showing how to run the IGTD algorithm for demonstration purposes.

The Data folder in this repository includes a small dataset for demonstrating its utility, which is a gene expression dataset including 100 cancer cell lines and 1600 genes. 

## Technical Details

Refer to this [README](.README.md) and the [Scripts](./Scripts) folder.
