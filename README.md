# UMID-Urine-Microscopic-Image-Dataset

Analysis of urine sediment particles from microscopic images play a vital role in the diagnosis of kidney diseases. The patient's urine is subjected to centrifuging and the sediment(solid) part of the urine is taken in a glass slide and observed under the microscope. The clinical examination of the urine sediment requires skilled technicians who has expertise in identifying the cells from images. The trained technicians then count the number of various cells by visual inspection, which is labor-intensive, time-consuming and dependent on the technician.

We present a dataset comprising of 367 annotated microscopic images of urine sediments of dimensions (1280,720). The images consists of many types of cells. We are classifying cells from only 3 classes - RBCs, pus cells/WBCs and epithelial cells. Most of the cells in the dataset are annotated with bounding boxes around them using the Microsoft Visual Object Tagging Tool (VoTT). We also used point annotations for annotating the cells which are present in clusters as drawing boxes over overlapping cells is a difficult task. The validation set is taken as 10% of all the training samples. The testing set is taken as 15% of the images.  

This dataset can be used to train deep learning models for cell detection and counting to assist in the diagnosis of kidney related diseases from urine samples. 

The RBCs are smaller, rounded and have well-defined sharp boundaries resembling a cup shaped structure. The pus cells are generally rounded and grainy in texture with no well-defined borders. The epithelial cells are irregular in shape, larger in size and generally contains a nucleus. The number of different cells in the data are listed in table:

| cell type | Training Set | Validation Set | Testing Set |
| --------- | ------------ | -------------- | ----------- |
|           | 268 images   | 38 images      | 61 images   |
| rbc | 1297 | 150 | 246 |
| pus | 1110 | 114 | 161 |
| epithelial | 642 | 82 | 96 |
| Total | 3049 | 346 | 503 |

We have a total of 3898 cell annotations in all the sets.

We have some cells which cannot be classified into any of the 3 classes and are labelled as missedlabel.
| cell type | Training Set | Validation Set | Testing Set |
| --------- | ------------ | -------------- | ----------- |
| missedlabel | 39 | 5 | 24 |

The Training Set of 268 images has annotations of cells as well as cluster of cells (Group Annotations). The Validation and Testing sets also has clusters of cells but these cells are annotated individually for computing the performance of the models.

Table populated in the order: Number of clusters (Total Number of cells in clusters) 

| cell type | Training Set | Validation Set | Testing Set |
| --------- | ------------ | -------------- | ----------- |
| rbc | 21 (51) | 6 (16) | 9 (21) |
| pus | 81 (327) | 15 (45) | 16 (44) |
| epithelial | 70 (295) | 14 (47) | 15 (52) |
| Total | 172 (673) | 35 (108) | 40 (117) |


For baseline (excluding images having cluster of cells), we have a total of 158 images and 1424 instances of cells. The split-up is as follows:

| cell type | Baseline Training Set | Training set without clusters |
| --------- | ------------ | ---------- |
| rbc | 993 | 1246 |
| pus | 302 | 783 |
| epithelial | 129 | 347 |
| Total | 1424 | 2376 |
