# Project Name - Skin Cancer Variant detection
    To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Objective
    - Build a CNN Model to detect Melonoma
    - Melonoma is a type of Caner that can be deadly if not detected early
    - Melonoma accounts for 75% of skin cancer deaths
    - Evaluate images and alert the dermatologists about the presence of melanoma and reduce of manual effort needed in diagnosis
- What is the background of your project?
- What is the business probem that your project is trying to solve?
    -  multiclass classification model using a custom convolutional neural network in TensorFlow. 
    - 9 Classes of skin cancer present in the database.
    	Class	No. of Image	percent(%)
        0	melanoma	439	20.0
        1	pigmented benign keratosis	462	21.0
        2	nevus	358	16.0
        3	basal cell carcinoma	377	17.0
        4	actinic keratosis	115	5.0
        5	squamous cell carcinoma	181	8.0
        6	vascular lesion	139	6.0
        7	seborrheic keratosis	78	3.0
        8	dermatofibroma	95	4.0
     - Impact of class imbalance , class rebalancing strategy and improve classification accuracy.
    
- What is the dataset that is being used?
    The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Four training options for the CNN has been tried out in this assignment
    - CNN 
    - CNN with dropouts
    - CNN with data augmentation
    - CNN with class rebalancing using augmentor
- Overfitting seen when the CNN is built with the provided data-set. The  valdation accuracy was seen in the range of 50%
- Slight improvement was seen when the CNN model included the dropouts and used the kera's data augmentation.
- When the Class rebalancing was performed with creation of augmented images , CNN training provided a very good validation accuracy of upto 80%
- Class rebalancing solved the overfitting problem see in all the other three training options.
- Multiple CNN Models were tried and it is seen that the Model with higher layers and parameters seems to overfit compared to lower number of layers and parameters.(Choice=2). Relative comparison between the training options for these CNN models are similar.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- python
- jupyter notebook
- tensorflow 2.
- numpy
- matplotlib
- pandas
- glob
- skimage

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
- References 
 - https://learn.upgrad.com/course/4477/segment/40020/233769/713965/3604175
 - https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000



## Contact
Created by [@sshrinivasbhat] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->