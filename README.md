# Using-Convolutional-Neural-Networks-CNN-to-Detect-a-Smile

## Data Source
The data is given in the 'datasets.zip'. If you are using Colab, you should run the code  
*"!rm -rf datasets.zip*  
*!rm -rf datasets*   
*import io*      
*from google.colab import files as colab_files*    
*uploaded = colab_files.upload()*    
*!unzip datasets.zip"*  to load the data.        
If you are using Jupyter Notebook, you should unzip the file for later use. [Dataset](https://github.com/sarahzhao21/Using-Convolutional-Neural-Networks-CNN-to-Detect-a-Smile/blob/e217e29e2ca488d39aff6a2ebd72d59abe9b32f6/datasets.zip)

## Introduction
Neural Network has enabled machines to view the world as humans do, perceive it in a similar manner and use the knowledge for complicated tasks such as Image/Video recognition, Image Analysis/Classification and Natural Language Processing, etc. The Convolutional Neural Network is an advanced algorithm that widely used on image recognition and classification.   
In this study, I used CNN deep learning model to implement the image recognition in order to recognize a smile face from all kinds of countenances. There are more than 3000 images in the train dataset and more than 1200 images in the validation dataset. The aim of this project is to use Keras algorithm to build CNN models, train the model by the train dataset and evaluate the model by the validation dataset.[The details and python codes are recorded here](https://github.com/sarahzhao21/Using-Convolutional-Neural-Networks-CNN-to-Detect-a-Smile/blob/e217e29e2ca488d39aff6a2ebd72d59abe9b32f6/Detect%20a%20smile%20in%20a%20image%20by%20CNN.ipynb).     
Here is the structure of the CNN Networks in this study:   
![CNN structure of this project](https://github.com/sarahzhao21/Using-Convolutional-Neural-Networks-CNN-to-Detect-a-Smile/blob/963f2c0392bde663ba3c097eef7d9c1eea373afd/CNN%20Structure%20Catoon.png)

## Conclusion
The number of epoches was set to 100. With "Relu" as the activation function, the validation accuracy is more than 0.87 but the overfitting started to occur when the number of epochs is great than 10. If I changed the activation function to "Tanh", the validation accuracy can reach 0.86, but the overfitting started to occur when the number of opochs is greater than 8.   
We can see that the structure of the neural networks works well, and we need to be careful about the number of epoches to get the best classification results.


