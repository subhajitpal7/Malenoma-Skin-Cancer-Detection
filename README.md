# Melanoma Detection
> To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
## Table of Contentss
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Model Building and Prediction](#model-building-and-prediction)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## Data Understanding:
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

- The data set contains the following diseases :
>> Actinic keratosis
>> Basal cell carcinoma
>> Dermatofibroma
>> Melanoma
>> Nevus
>> Pigmented benign keratosis
>> Seborrheic keratosis
>> Squamous cell carcinoma
>> Vascular lesion


## Model Building and Prediction
- Data Reading/Data Understanding
- Dataset Creation
> - Creating training and validation data, define batch size and resize images.
- Dataset visualisation
> - Visualizing nine different classes present in dataset.
- Model Building & training
> - Created CNN Model to train and predict the nine different classes.
> - (0,1) rescalling used on RGB images.
> - Initial run on 20 epochs.
> - Observed model performance.
- Chose an appropriate data augmentation strategy to resolve underfitting/overfitting 
- Model Building & training on the augmented data :
> - Created CNN Model to train and predict the nine different classes.
> - (0,1) rescalling used on RGB images.
> - Initial run on 20 epochs.
> - Observed model performance.
- Class distribution:
> - seborrheic keratosis class have least number of samples which is 77.
> - pigmented benign keratosis (462 Samples), melanoma (438 Samples), basal cell carcinoma (376 Samples), and nevus (357 Samples) classes dominates the data in terms proportionate number of samples.
- Handling class imbalances
- Model Building & training on the rectified class imbalance data :
> - Created CNN Model to train and predict the nine different classes.
> - (0,1) rescalling used on RGB images.
> - Initial run on 30 epochs.
> - Observed model performance.
> - Initial run on 50 epochs.

## Conclusions
- Final CNN model Architecture:
<img src="/images/architecture.png" alt="Image" title="Model-Architecture">

- Model performance with 30 epochs : 
> 1. Class rebalancing and augmentation helps achieving the better training and validation accuracy.
> 2. Model overfitting and underfitting issue is resolved now.
> 3. We have achieved better model accuracy with maximum of 87% training accuracy and 78% of validation accuracy.
> 4. Also, overall loss is reduced it is around 0.3 for training and 0.6 for validation.
<img src="/images/30Epoch.png" alt="Image" title="Model Performance 20 Epoch">
- Model performance with 50 epochs : 
> 1. Overall model accuracy increases, now we have 90% training accuracy and 80% validation accuracy.
> 2. Model performs better with higher iteration value that is high epoch.
> 3. Overall loss is also reduced to for training 0.3 and validation 0.5.


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- library - PYTHON
- library - PANDAS
- library - NUMPY
- library - MATPLOTLIB
- library - TENSORFLOW
- library - KERAS
- library - AUGMENTOR



<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->


## Contact
Created by [@Subhajitpal7] - feel free to contact me!
