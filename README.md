# DeepLabV3-Drone-Imagery
This repository contains all the files I created or modified for my master thesis. It should be noted that using DeepLab without being able to read the source code is very difficult. There is not much documentation, especially for training on custom data.

DeepLab uses a unique input format called TFRecords. Unfortunately, there is no straightforward way to convert data into this format. It is highly recommended to read Mike Heavers' repository for the creation of TFRecords https://github.com/heaversm/deeplab-training.git. However, all the data has already been prepared for conversion in the Damage and Material Folder. The TFRecord files have also been created.

I included all python files that had to be modified in the Important Files folder. These files had to be modified to be used for multi-class detection on custom classes. Additionally, frozen models for material and damage detection have been stored. A few result examples can be found in the Result Image Example folder.

The repository contains two .ipynb files. These files can be opened in Google Colab. It is recommended to use Google Chrome when using these files. "DeeplabV3+ Drone Imagery.ipynb" contains the main code for training machine learning models. After training, a frozen model can be exported and used to run inferences. "Create Labeled Dataset.ipynb" is a script that has been written to run automatic inferences on images using the frozen model.


![Alt text](https://github.com/ktruong-civ/DeepLabV3-Drone-Imagery/blob/master/Result%20Image%20Examples/Material/DJI_0258%20156.jpg "Optional title")
![Alt text](https://github.com/ktruong-civ/DeepLabV3-Drone-Imagery/blob/master/Result%20Image%20Examples/Damage/DJI_0258%20217.jpg "Optional title")

