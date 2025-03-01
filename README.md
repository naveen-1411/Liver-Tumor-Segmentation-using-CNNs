# Liver-Tumor-Segmentation-using-CNNs

This project segments tumors in the Liver using 2 cascaded CNNs. We use 3D-IRCADb 01 as our dataset. View the Thesis for more details about the model, dataset, methodology and results.

There are 3 notebooks in this project

3d-ircadb-01_util.ipynb Responsible for renaming files, merging masks and augmenting the dataset

liver_CNN.ipynb The first CNN, it uses a CNN to segment the Liver and extract the ROI

tumor_CNN_final.ipynb The second CNN, it segments the tumors using a CNN after masking other organs using the extracted ROI from the first CNN

There is the models directories which contains the trained models

liver_model_final_resunet.h5 which is the first CNN trained for 20 epochs
tumor_weights_final_50epochs.h5 which is the second CNN trained for 50 epochs
tumor_weights_final_100epochs.h5 which is the second CNN trained for 100 epochs
Dependencies
I used Anaconda for package management but pip will work all the same

Tensorflow-GPU
Keras (Tensorflow) already comes with Tensorflow
Numpy
OpenCV
Matplotlib
Pydicom
Jupyter Notebook
Scipy
Scikit-learn
PIL
Seaborn
Imageio
Dataset Structure
The structure of the dataset should be as follows ( if you don't want to change the code 😀 )
