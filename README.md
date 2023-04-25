# AngioKey : Coronary-Angiogram-Keyframes-Extraction

This is the official repository for the paper "Angiokey: A Deep Learning Method for Extracting Keyframes from Coronary Angiograms" submited in Computer Methods and Programs in Biomedicine.

I have to say that this code was inspired from https://github.com/RGivisiez/Blood-Vessel-Segmentation.

I made some of the following changes:

- Load images has been adapted to the structure of our dataset;
- We didn't train the U-net, we loaded a pretrained model;
- The test is done on our personal dataset to produce the frame masks (Ground Truth).

# usefulness :

This project can be used to automatically generate groundtruths of medical images. It was tested on a sample of coronary frames extracted from angiographic videos. Then it offers keyframes extraction from each video.

The project will be useful to automatically manage a large dataset ensuring better performance.

# Authors: 
Hounaida Moalla & Aiman Ghrab

# Previous works
Previous work has been presented in 

Moalla, H.; Ghrab, A.; Ben Hamed, B.; Bahloul, A.; Hammami, R. and Abid, L. (2023). Automatic Coronary Angiogram Keyframe Extraction.  In Proceedings of the 12th International Conference on Pattern Recognition Applications and Methods, ISBN 978-989-758-626-2, ISSN 2184-4313, pages 582-589.

In this work, we have applied the method of filters on the frames for extraction of keyframes.

# Citation

@software{Hounaida_and_all_2023,
  authors = {Hounaida Moalla and Aiman Ghrab},
  doi = {10.5281/zenodo.1234},
  month = {04},
  title = {{Coronary-Angiogram-Keyframes-extraction}},
  url = {https://github.com/HounaidaM/Coronary-Angiogram-Keyframes-extraction},
  version = {v1.4.23},
  year = {2023}
}

# Environment
Python, Keras, Kaggle cloud

# Dataset
The full dataset was collected from exams performed by a single catheterization laboratory during the period between January 2018 and December 2021.
Dataset consisted of 3159 angiographic study: a total of 37209 coronary angiograms was extracted. We used a sample of 45 angiograms to extract a total of
1434 frames of size 512 x 512 pixels.
A sample of the dataset is put in the "oneSampleCoro" section above.
All zipped dataset is put in the "all_dataSet_deep" section above.

# Model
The used model is U-net from @https://arxiv.org/abs/1505.04597 

# Trained models
Section Models contains models traindes with 150, 200 and 300 epochs. 
