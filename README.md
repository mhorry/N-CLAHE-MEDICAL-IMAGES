# N-CLAHE Lung Medical Images
A Repository of N-CLAHE histogram equalized Lung medical images (CXR, CT and Ultrasound) for Training of Deep Learning Models

One of the key challenges in building machine learning models for medical images is the variability in the quality of the images within and between sources, especially where certain conditions (such as COVID-19) are primarily located at a single sources such as https://github.com/ieee8023/covid-chestxray-dataset, https://github.com/jannisborn/covid19_pocus_ultrasound and https://github.com/UCSD-AI4H/COVID-CT.

We have taken these images and applied N-CLAHE as described in the following paper:

Koonsanit, Kitti & Thongvigitmanee, Saowapak & Pongnapang, Napapong & Thajchayapong, Pairash. (2017). Image enhancement on digital x-ray images using N-CLAHE. 1-4. 10.1109/BMEiCON.2017.8229130. 

We don't want our AIs to be mistrained by systematic differences in brightness/contrast and other attributes associated with the image source rather than the clinical conditions that we are interested in so we are developing a pipeline that normalizes the images through normalization and histogram equalization.  Future enhancement will be a U-Net based segmentation.
