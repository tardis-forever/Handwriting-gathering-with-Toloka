# Handwriting image dataset collection
This is an example of simple handwriting images gathering pipeline implemented using Yandex.Toloka and Yandex.Disk API

The goal for this project is to collect images of handwritten text for a dataset that could be used to train and evaluate HTR models.

Furthermore, you can later enhance this dataset with extra bounding boxes for separate lines or words, using [this tutorial](https://github.com/Toloka/toloka-kit/blob/main/examples/1.computer_vision/object_detection/image_segmentation.ipynb) from `toloka-kit` as an example.

Main code is provided in [handwriting-gathering.ipynb](handwriting-gathering.ipynb). With provided data and images one can re-run the whole pipeline for French. Code can be reused for any other language provided sample training photos are collected for training and the project#1 instructions are translated to that language (optionally, you can use English instructions that are also provided). 

### Structure:

- [data/](data) contains sample sentences that can be reused instead of scraping
- [instructions/](instructions) contains instructions for the projects and images for them
- [img/](img) contains illustrations for the notebook
- [corpus.py](corpus.py) contains sample class for Wikipedia dump sentence extraction
- [requirements.txt](requirements.txt)  contains all the requirements for the pipeline
- [handwriting-gathering.ipynb](handwriting-gathering.ipynb) contains main code for the pipeline
