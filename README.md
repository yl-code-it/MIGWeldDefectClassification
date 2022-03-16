# MIGWeldDefectClassification
These weld images are prepared for academic course project usage purpose. Any commercial usage, please contact the author before any downloads. 

"GOOD" folder contains 900 OK welds
"BAD" folder contains 108 NOK welds - welds that are considered as defects. Most are porosity defect type. 

Machine Learning 3253 - Term Project - Classifying Good/Bad Weld Images using Transfer Learning in Keras

Yu Lin, Soumitra Dinda, Senda Chinganzi, and Qi (Quincy) Zhang

1- Upload local weld images into Colab by choosing the zipped folder. This dataset has 2 classes (Good, and Bad). Images for each class are stored in its own folder.

2- The images have dimensions of 576x300, 8-bit depth, .BMP format. Resize all of them to 150x150.

3- Split images to 75-25% for training and test. Make sure you have the same distribution of Good/Bad weld types between train and test datasets.

4- Use a VGG16 model (pre-trained on ImageNet)

5- Remove the top layers (fully connected layers)

6- Add your own fully connected layers (one with 256 nodes using ‘relu’ activation and output layer with 2 nodes (2 classes - Good/Bad welds) and ‘softmax’ activation)

7- First, freeze all layers of VGG16, train (fine-tune) and evaluate the model. You need to pick the right hyper-parameters for your training (try with different ones)

8- Second, unfreeze the last block of VGG16 (block5), re-train and evaluate the model

9- Third, enable all blocks of VGG16 to re-train and evaluate the model
