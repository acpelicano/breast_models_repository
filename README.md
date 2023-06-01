# breast_models_repository

## Introduction & Motivation ##
The purpose of this repository is to provide the research community with a repository of multiple anatomically realistic breast models, including benign and malignant tumorous tissues, which can be used for the improvement and validation of Microwave Imaging (MWI) systems. The developed models were derived from 3.0T Magnetic Resonance Images (MRI) of healthy and cancer patients acquired at Hospital da Luz - Lisboa, which includes normal breast tissues (such as fat, fibroglandular, skin, and muscle tissues), and benign and cancerous breast tumours. Additionally, this repository also includes an executable file which generates models containing breast tissues dielectric properties, between 3 and 10 GHz (with a step of 0.01 GHz).
Currently, the dataset comprises anatomically realistic numerical models of breast tissues of 33 patients with a total of 46 tumours (23 benign and 23 malignant).

## Repository Structure ##
We provide one folder per patient, containing:

- Label_map_simple: a label map including benign tumour (label -4), malignant tumour (label -3), skin (label -2), muscle (label -1), background (label 0), fat (label 1);
- Label_map_detailed: a label map including benign tumour (label -4), malignant tumour (label -3), skin (label -2), muscle (label -1), background (label 0), fat_high (label 7), fat_median (label 6), fat_low (label 5), transition (label 4), fibroglandular_high (label 3), fibroglandular_median (label 2), fibroglandular_low (label 1) - the labels low, median and high refer to the voxel intensities;
- T1-w_Dixon-W_pre-processed: a Dixon water image after bias correction, data normalisation, and background subtraction.


## Exams ##
| ID | No. Benign tumours | No. Malignant Tumours | Size of Tumours (mm) |
|:--:|:------------------:|:---------------------:|:--------------------:|
| 01 |         2          |           0           |Large (6.8x7.6x7.2); Small (6.9x6.9x5.2)|
| 02 |         0          |           3           |Large (80.9x74.9x56.2); Medium (8.4x7.6x7.4); Small (8.1x6.8x8.1)|
| 03 |         0          |           1           | (8.5x11.2x9.2)       |
| 04 |         1          |           1           |Benign(14.0x11.1x6.5); Malignant(9.7x8.7x8.6)|
| 05 |         2          |           0           |Large (19.1x19.6x18.2); Small (15.5x15.3x13.7)|
| 06 |         0          |           1           |(12.8x13.5x14.4)      |
| 07 |         0          |           1           |(8.4x12.4x10.5)       |
| 08 |         0          |           1           |(18.8x19.1x20.2)      |
| 09 |         2          |           0           |Large (9.7x7.8x5.4); Small (6.1x5.7x5.6)|
| 10 |         0          |           1           |(23.1x24.0x23.2)      |
| 11 |         0          |           1           |(33.2x32.6x29.9)      |
| 12 |         0          |           2           |Large (11.2x8.9x6.8); Small (10.0x10.1x7.7)|
| 13 |         0          |           1           | (12.5x10.9x12.5)     |
| 14 |         0          |           1           |(11.2x11.0x10.3)      |
| 15 |         0          |           1           |  (27.7x24.9x19.7)    |
| 16 |         1          |           0           |    (7.4x7.8x7.8)     |
| 17 |         0          |           1           |  (11.5x12.1x14.8)    |
| 18 |         1          |           0           |  (7.9x7.3x6.3)       |
| 19 |         2          |           0           |Large (49.0x36.6x35.1); Small (8.5x7.9x9.0)|
| 20 |         0          |           1           | (29.56x30.01x19.33)  |
| 21 |         1          |           0           |  (13.8x15.8x12.6)    |
| 22 |         0          |           1           |    (11.4x11.4x10.6)  |
| 23 |         0          |           1           | (7.1x7.3x5.4)        |
| 24 |         0          |           1           |  (47.1x29.5x39.2)    |
| 25 |         2          |           0           |Large (8.1x7.1x6.2); Small (5.4x5.4x5.0)|
| 26 |         0          |           1           | (21.8x25.3x25.9)     |
| 27 |         0          |           1           | (30.9x26.7x28.3)     |
| 28 |         0          |           1           | (46.2x38.1x44.7)     |
| 29 |         1          |           0           | (16.2x19.3x16.1)     |
| 30 |         1          |           0           | (9.6x11.3x6.4)       |
| 31 |         5          |           0           | XLarge (13.8x16.6x8.6); Large (13.2x15.7x11.4); Medium (10.0x10.8x7.97); Small (9.55x8.31x10.5); XSmall (10.3x9.01x8.14)|
| 32 |         1          |           0           | (7.05x6.46x3.91)       |
| 33 |         1          |           0           | (6.90x6.81x8.20)       |


## Compatibility ##
All files are provided in MHA format. The files were created with the original resolution of the MRI scans.

## MRI Acquisition ##
Women were imaged in a prone position in a 3.0T MAGNETON Vida clinical MR scan (Siemens Healthineers, Erlangen – Germany) with a dedicated coil (Siemens Breast 18 coil) for the breast. This study was approved by the Scientific and Ethical Commission of Hospital da Luz – Lisboa, under references CES/44/2019/ME (19/09/2019) and CES/34/2020/ME (06/11/2020).

## Cite Us ##
If you use some of these models, please cite us with:

Pelicano, A.C.; Gonçalves, M.C.T.; Godinho, D.M.; Castela, T.; Orvalho, M.L.; Araújo, N.A.M.; Porter, E.; Conceição, R.C. Development of 3D MRI-Based Anatomically Realistic Models of Breast Tissues and Tumours for Microwave Imaging Diagnosis. Sensors 2021, 21, 8265. https://doi.org/10.3390/s21248265
