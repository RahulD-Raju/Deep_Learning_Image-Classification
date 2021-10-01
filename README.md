# Image Classification for Object Detection in Driverless Vehicles
Prepared by Rahul D. Raju

# Abstract
The applications of deep learning are extensive and ever growing.  They include virtual assistants, chatbots, 
fraud detection, NLP, image recognition and text generation to name a few.  One area related to deep learning 
that has received a fair amount of media attention recently is the development of driverless cars.  
Though the safety and efficacy of driverless vehicles continues to be debated, its advantages are vast. 
The fundamental challenge of driverless vehicles is taking real-world activities that are designed for biological 
neural networks and transferring them to artificial neural networks.  The most important component of this challenge 
is the ability of driverless software to recognize and differentiate objects encountered during daily operations. 


# Data

Source:  University of Toronto, https://www.cs.toronto.edu/~kriz/cifar.html

Dataset:  Canadian Institute for Advanced Research(CIFAR-10)

Num. Images:  60,000

Num Labels:  10(6,000 images/label)

Labels:  airplane, automobile(ex-truck), truck, ship, bird, cat, deer, frog, horse, dog

# Methodology and Algorithms
First the convolutional archetectural shell of the MobileNet model was extracted
This was an unfrozen base, thus no pre-trained features were used.  Multiple dense layers
were added, with varying nodes and drop-out rates

# Tools
Analysis:  Tensorflow Keras, Scikit Learn, Numpy
Visualization:  Matplotlib, Seaborn

# Results Summary

 Several models were used with the best producing an accuracy of .80.
 
    precision    recall  f1-score   support

           0       0.81      0.85      0.83      1000
           1       0.90      0.89      0.90      1000
           2       0.78      0.75      0.77      1000
           3       0.64      0.65      0.65      1000
           4       0.83      0.77      0.80      1000
           5       0.66      0.75      0.70      1000
           6       0.93      0.81      0.86      1000
           7       0.83      0.85      0.84      1000
           8       0.81      0.94      0.87      1000
           9       0.95      0.82      0.88      1000

    accuracy                           0.81     10000
   macro avg       0.81      0.81      0.81     10000
weighted avg       0.81      0.81      0.81     10000
