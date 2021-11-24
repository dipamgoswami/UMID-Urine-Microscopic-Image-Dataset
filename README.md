# UMID-Urine-Microscopic-Image-Dataset [https://arxiv.org/abs/2111.10374]

Analysis of urine sediment particles from microscopic images play a vital role in the diagnosis of kidney diseases. The patient's urine is subjected to centrifuging and the sediment(solid) part of the urine is taken in a glass slide and observed under the microscope. The clinical examination of the urine sediment requires skilled technicians who has expertise in identifying the cells from images. The trained technicians then count the number of various cells by visual inspection, which is labor-intensive, time-consuming and dependent on the technician.

We present a dataset comprising of 367 annotated microscopic images of urine sediments of dimensions (1280,720). The images consists of many types of cells. We are classifying cells from only 3 classes - RBCs, pus cells/WBCs and epithelial cells. Most of the cells in the dataset are annotated with bounding boxes around them using the Microsoft Visual Object Tagging Tool (VoTT). We also used point annotations for annotating the cells which are present in clusters as drawing boxes over overlapping cells is a difficult task. The validation set is taken as 10% of all the training samples. The testing set is taken as 15% of the images.  

This dataset can be used to train deep learning models for cell detection and counting to assist in the diagnosis of kidney related diseases from urine samples. 

The RBCs are smaller, rounded and have well-defined sharp boundaries resembling a cup shaped structure. The pus cells are generally rounded and grainy in texture with no well-defined borders. The epithelial cells are irregular in shape, larger in size and generally contains a nucleus.

