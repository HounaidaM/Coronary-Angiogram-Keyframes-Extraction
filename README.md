# AngioData : A Novel Open Dataset of Coronary Artery Keyframes Extracted via Deep Learning

This is the official repository for the paper "AngioData : A Novel Open Dataset of Coronary Artery Keyframes Extracted via Deep Learning" submited in Journal of Cardiovascular Translational Research.

We're applying **AngioKey** for image segmentation, followed by extracting keyframes from the segmented images.

## AngiKey
I have to say that this code was inspired from <a href="URL_du_lien">https://github.com/RGivisiez/Blood-Vessel-Segmentation</a>.

I made some of the following changes:

- Load images has been adapted to the structure of our dataset;
- We trained the U-net model on a dataset given from <a href="URL_du_lien">https://doi.org/10.3390/app9245507</a>;
- The test is done on our personal dataset to produce the frame masks (Ground Truth).

## Keyframes extraction
The keyframe extraction work has been featured in publication <a href="URL_du_lien">https://www.scitepress.org/PublicationsDetail.aspx?ID=QhrTWXiEsD8=&t=1</a>.

# usefulness :

This project can be used to automatically generate groundtruths of medical images. It was tested on a private dataset of angiograms. We present her a sample of coronary frames extracted from angiographic videos. We segmented all frames and extracted all keyframes from each sampled video.

The project will be useful to automatically manage a large dataset ensuring better performance and extract keyframes.

# Authors: 
Hounaida Moalla & Aiman Ghrab

# Previous works
Previous work has been presented in 

Moalla, H.; Ghrab, A.; Ben Hamed, B.; Bahloul, A.; Hammami, R. and Abid, L. (2023). Automatic Coronary Angiogram Keyframe Extraction.  In Proceedings of the 12th International Conference on Pattern Recognition Applications and Methods, ISBN 978-989-758-626-2, ISSN 2184-4313, pages 582-589.
**doi:** <a href="URL_du_lien">https://doi.org/10.1109/INISTA59065.2023.10310496</a>

In this work, we have applied the method of filters on the frames for extraction of keyframes.

# Other uses
1- We used the segmented keyframes for classification Left/Right of frames.
H. Moalla, A. Ghrab, B. B. Hamed, A. Bahloul and L. Abid, "Exploiting Pre-trained Architectures for Dual-Stream Classification of LCA-RCA in a Private AngioData," 2023 International Conference on Innovations in Intelligent Systems and Applications (INISTA), Hammamet, Tunisia, 2023, pp. 1-6. 
**doi:** <a href="URL_du_lien">10.1109/INISTA59065.2023.10310496</a>.

2- Next step will be focuse on quantification of stenosis : detection and mesure.

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

# AngioData Dataset
The full dataset was collected from exams performed by a single catheterization laboratory during the period between January 2018 and December 2021.
Dataset consisted of 3159 angiographic study: a total of 37209 coronary angiograms was extracted. We used a sample of 45 angiograms to extract a total of
1434 frames of size 512 x 512 pixels.
A sample of the dataset is put in the "oneSampleCoro" section above.
All zipped dataset is put in the "all_dataSet_deep" section above.

# Model
The used model is U-net from <a href="URL_du_lien">https://arxiv.org/abs/1505.04597</a>. 

# Trained models
Section Models contains models traindes with 150, 200 and 300 epochs. 
