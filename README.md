# DeepLabV3-Drone-Imagery

DeepLab uses a unique input format called TFRecords. Unfortunately, there is no straightforward way to convert data into this format. It is highly recommended to read Mike Heavers' repository for the creation of TFRecords. However, all the data has already been prepared for conversion in the Damage and Material Folder. The TFRecord files have also been created.

I included all the python files that had to be modified in the File Changes folder. These files had to be modified to be used for multi-class detection on custom classes.

The repository contains two .ipynb files. These files can be opened in Google Colab. It is recommended to use Google Chrome when using these files. "DeeplabV3+ Drone Imagery.ipynb" contains the main code for training machine learning models. After training, a frozen model can be exported and used to run inferences. "Create Labeled Dataset.ipynb" is a script that has been written to run automatic inferences on images using the frozen model.
