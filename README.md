
This repository is as a fork of "Segmentation of Intracellular Structures in Fluorescence Microscopy Images by Fusing Low-Level Features".

---

### 1. Overview

This work focuses on the fluorescence microscopy images (FLMIs) segmentation using deep learning techniques. We have found out that the low level features are playing enssential roles in segmenting FLMIs and a proper fusion operator can dramatically improve the performance of a general-purpose model in this task. In this repository, we provide with our implementations to improve the segmentation models in segmenting FLMIs.

(1) Dependencies

This implementation requires the following libraries:

* PyTorch version 1.2.0
* Python version 3.7
* OpenCV version 4.5.1

(2) Training

* To train the model, save the paths of the images and masks in a **_.txt** file and put it into the dictionary **datasets**, then run **trainer__(model).py** for different models.

* The loss funcitons are in **models/optimize.py**

* Most models are trained with 30 epochs.

（3）Evaluation

* To test the performance, please run **inference.py** to get different metrics scores such as IOU, F1 and others. 

* Then run **inference_img.py** to get the segmentations. 

* In addition, you can run **inference_unet.py** to get the performance of the modified-UNet.

### 5. Contributing 
Codes and datasets for this project are developped at CBMI Group (Computational Biology and Machine Intelligence Group, National Laboratory of Pattern Recognition, INSTITUTE OF AUTOMATION, CHINESE ACADEMY OF SCIENCES).

