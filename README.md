# breast_models_repository

## Introduction & Motivation ##
The purpose of this repository is to provide the research community with a repository of multiple anatomically realistic breast models, including benign and malignant tumorous tissues, which can be used for the improvement and validation of Microwave Imaging (MWI) systems. The developed models were derived from 3.0T Magnetic Resonance Images (MRI) of healthy and cancer patients acquired at Hospital da Luz - Lisboa, which includes normal breast tissues (such as fat, fibroglandular, skin, and muscle tissues), and benign and cancerous breast tumours. Additionally, this repository also includes an executable file which generates models containing breast tissues dielectric properties, between 3 and 10 GHz (with a step of 0.01 GHz).
Currently, the dataset comprises anatomically realistic numerical models of breast tissues of 55 patients with a total of 84 tumours (46 benign and 38 malignant).

## Repository Structure ##
We provide one folder per patient, containing:

- Label_map_simple: a label map including benign tumour (label -4), malignant tumour (label -3), skin (label -2), muscle (label -1), background (label 0), fat (label 1);
- Label_map_detailed: a label map including benign tumour (label -4), malignant tumour (label -3), skin (label -2), muscle (label -1), background (label 0), fat_high (label 7), fat_median (label 6), fat_low (label 5), transition (label 4), fibroglandular_high (label 3), fibroglandular_median (label 2), fibroglandular_low (label 1) - the labels low, median and high refer to the voxel intensities;
- T1-w_Dixon-W_pre-processed: a Dixon water image after bias correction, data normalisation, and background subtraction.


## Exams ##
| ID |  BMI  | Right Breast | Left Breast | Size of Tumours (mm) |
|:--:|:-----:|:------------:|:-----------:|:--------------------:|
| 01 | 20.76 | Benign = 2 Malignant = 0         |           0           |Large (6.8x7.6x7.2); Small (6.9x6.9x5.2)|
| 02 | 26.99 |    0          |           3           |Large (80.9x74.9x56.2); Medium (8.4x7.6x7.4); Small (8.1x6.8x8.1)|
| 03 | 25.40 |    0          |           1           | (8.5x11.2x9.2)       |
| 04 | 23.37 |    1          |           1           |Benign(14.0x11.1x6.5); Malignant(9.7x8.7x8.6)|
| 05 | 23.87 |    2          |           0           |Large (19.1x19.6x18.2); Small (15.5x15.3x13.7)|
| 06 | 25.00 |    0          |           1           |(12.8x13.5x14.4)      |
| 07 | 20.44 |    0          |           1           |(8.4x12.4x10.5)       |
| 08 | 25.61 |    0          |           1           |(18.8x19.1x20.2)      |
| 09 | 21.67 |    2          |           0           |Large (9.7x7.8x5.4); Small (6.1x5.7x5.6)|
| 10 | 31.24 |    0          |           1           |(23.1x24.0x23.2)      |
| 11 | 30.30 |    0          |           1           |(33.2x32.6x29.9)      |
| 12 | 29.14 |    0          |           2           |Large (11.2x8.9x6.8); Small (10.0x10.1x7.7)|
| 13 | 24.24 |    0          |           1           | (12.5x10.9x12.5)     |
| 14 | 25.78 |    0          |           1           |(11.2x11.0x10.3)      |
| 15 | 24.46 |    0          |           1           |  (27.7x24.9x19.7)    |
| 16 | 24.14 |    0          |           1           |  (11.5x12.1x14.8)    |
| 17 | 28.13 |    1          |           0           |  (7.9x7.3x6.3)       |
| 18 | 29.36 |    2          |           0           |Large (49.0x36.6x35.1); Small (8.5x7.9x9.0)|
| 19 | 27.68 |    0          |           1           | (29.56x30.01x19.33)  |
| 20 | 25.15 |    1          |           0           |  (13.8x15.8x12.6)    |
| 21 | 24.54 |    0          |           1           |    (11.4x11.4x10.6)  |
| 22 | 24.00 |    0          |           1           | (7.1x7.3x5.4)        |
| 23 | 30.12 |    0          |           1           |  (47.1x29.5x39.2)    |
| 24 | 22.60 |    2          |           0           |Large (8.1x7.1x6.2); Small (5.4x5.4x5.0)|
| 25 | 25.80 |    0          |           1           | (21.8x25.3x25.9)     |
| 26 | 24.65 |    0          |           1           | (30.9x26.7x28.3)     |
| 27 | 24.13 |    0          |           1           | (46.2x38.1x44.7)     |
| 28 | 22.51 |    1          |           0           | (16.2x19.3x16.1)     |
| 29 | 27.61 |    1          |           0           | (9.6x11.3x6.4)       |
| 30 | 43.18 |    5          |           0           | XLarge (13.8x16.6x8.6); Large (13.2x15.7x11.4); Medium (10.0x10.8x7.97); Small (9.55x8.31x10.5); XSmall (10.3x9.01x8.14)|
| 31 | 25.95 |    1          |           0           | (7.1x6.5x3.9)        |
| 32 | 24.02 |    1          |           0           | (6.9x6.8x8.2)        |
| 33 | 22.99 |    0          |           1           | (15.2x17.4x13.7)     |
| 34 | 25.86 |    1          |           0           | (6.9x6.9x6.9)        |
| 35 | 21.88 |    0          |           1           | (18.3x23.5x18.9)     |
| 36 | 31.18 |    0          |           1           | (11.4x11.5x10.9)     |
| 37 | 25.97 |    2          |           0           | Large (7.5x6.5x5.1); Small (6.4x3.2x5.8)    |
| 38 | 23.73 |    1          |           0           |  (7.0x6.7x5.6)    |
| 39 | 19.28 |    1          |           0           |  (5.6x6.3x5.0)    |
| 40 | 23.12 |    0          |           1           |  (10.9x15.0x9.7)    |
| 41 | 21.72 |    4          |           1           |  Malignant (30.9X43.8X40.1); Benign XLarge (19.4x26.8x28.7); Benign Large (23.6x20.2x19.7); Benign Small (12.3x15.8x14.0); Benign XSmall (8.7x10.3x10.1)|
| 42 | 21.45 |    1          |            0          |   (9.1x9.1x7.6)    |
| 43 | 31.25 |      0        |              1        |    (16.7x17.3x15.9)  |
| 44 | 21.45 |      0        |              1        |    (42.5x37.4x29.0)  |
| 45 | 23.67 |     1        |              2        |    Malignant Large (34.9x43.3x39.8); Malignant Small (9.40x7.81x6.51); Benign (7.4x9.3x8.1)  |
| 46 | 34.38 |      3        |              2        |    Malignant Large (40.3x41.8x21.1); Malignant Small (9.6x9.1x10.0); Benign Large (9.2x10.8x9.5); Benign Medium (9.2x10.3x9.4); Benign Small (8.1x8.2x8.0)  |
| 47 | 21.48 |      2        |              0        |    Large (13.8x17.2x18.2); Small (7.4x6.9x6.3)  |
| 48 | 24.97 |      2        |              0        |    Large (9.0x11.6x7.9); Small  (10.2x10.2x8.2)  |
| 49 | 20.96 |      0        |              1        |    (17.5x23.6x23.1)  |
| 50 | 35.16 |      1        |              0        |      (10.8x8.5x10.3)  |
| 51 | 24.09 |      1        |              0        |       (6.9x8.1x8.7)  |
| 52 | 31.63 |      3        |              0        |     Large (16.1x19.4x11.8); Medium (8.5x11.0x10.0); Small  (7.9x7.1x6.9)  |
| 53 | 22.66 |      0        |              2        |      Large (30.7x32.3x22.1); Small (4.8x5.7x4.8)  |
| 54 | 25.86 |      1        |              0        |      (6.8x6.1x5.7)   |
| 55 | 21.88 |      0        |              1        |     (20.9x20.8x15.7)   |

BMI = Body Mass Index

## Compatibility ##
All files are provided in MHA format. The files were created with the original resolution of the MRI scans.

## MRI Acquisition ##
Women were imaged in a prone position in a 3.0T MAGNETON Vida clinical MR scan (Siemens Healthineers, Erlangen – Germany) with a dedicated coil (Siemens Breast 18 coil) for the breast. This study was approved by the Scientific and Ethical Commission of Hospital da Luz – Lisboa, under references CES/44/2019/ME (19/09/2019) and CES/34/2020/ME (06/11/2020).

## Cite Us ##
If you use some of these models, please cite us with:

Pelicano, A.C.; Gonçalves, M.C.T.; Godinho, D.M.; Castela, T.; Orvalho, M.L.; Araújo, N.A.M.; Porter, E.; Conceição, R.C. Development of 3D MRI-Based Anatomically Realistic Models of Breast Tissues and Tumours for Microwave Imaging Diagnosis. Sensors 2021, 21, 8265. https://doi.org/10.3390/s21248265
