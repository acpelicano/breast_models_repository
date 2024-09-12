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
| ID |  BMI  |Diagnosis|  R  |Right Breast (No. of tumours)|Left Breast (No. of tumours)| Size of Tumours (mm) |
|:--:|:-----:|:-------:|:---:|:---------------------------:|:--------------------------:|:--------------------:|
| 01 | 20.76 |    -    |     |Benign = 2 Malignant = 0    | Benign = 0 Malignant = 0   |Right Breast: L=(6.8x7.6x7.2); S=(6.9x6.9x5.2) |
| 02 | 26.99 |    ILC  |R.r=2.26; R.l=2.03|Benign = 0 Malignant = 2    | Benign = 0 Malignant = 1   |Right Breast: M=(8.4x7.6x7.4); S=(8.1x6.8x8.1) & Left Breast: L=(80.9x74.9x56.2) |
| 03 | 25.40 |    IC   |R.r=2.04; R.l=1.97|Benign = 0 Malignant = 1    | Benign = 0 Malignant = 0   |Right Breast: (8.5x11.2x9.2)       |
| 04 | 23.37 |    IC   |R.r=2.07; R.l=2.09|Benign = 1 Malignant = 1    | Benign = 0 Malignant = 0   |Right Breast: Benign(14.0x11.1x6.5); Malignant(9.7x8.7x8.6)|
| 05 | 23.87 |    F    |R.r=1.84; R.l=1.97|Benign = 2 Malignant = 0    | Benign = 0 Malignant = 0   |Right Breast: L=(19.1x19.6x18.2); S=(15.5x15.3x13.7)|
| 06 | 25.00 |    IC   |     |Benign = 0 Malignant = 0    | Benign = 0 Malignant = 1   |Left Breast: (12.8x13.5x14.4)      |
| 07 | 20.44 |    IC   |R.r=1.78; R.l=1.86| Benign = 0 Malignant = 0    | Benign = 0 Malignant = 1   |Left Breast: (8.4x12.4x10.5)       |
| 08 | 25.61 |    -    |     | Benign = 0 Malignant = 0    | Benign = 0 Malignant = 1   |Left Breast: (18.8x19.1x20.2)      |
| 09 | 21.67 |   -     |     | Benign = 2 Malignant = 0    | Benign = 0 Malignant = 0   |Right Breast: L=(9.7x7.8x5.4); S=(6.1x5.7x5.6)|
| 10 | 31.24 |    IC   |     | Benign = 0 Malignant = 1    | Benign = 0 Malignant = 0   |Right Breast: (23.1x24.0x23.2)     |
| 11 | 30.30 |   IC    |     | Benign = 0 Malignant = 0    | Benign = 0 Malignant = 1   |Left Breast: (33.2x32.6x29.9)      |
| 12 | 29.14 |   IC    |     | Benign = 0 Malignant = 2    | Benign = 0 Malignant = 0   |Right Breast: L=(11.2x8.9x6.8); S=(10.0x10.1x7.7)|
| 13 | 24.24 |  IC     |R.r=1.83; R.l=1.84| Benign = 0 Malignant = 1    | Benign = 0 Malignant = 0   |Right Breast: (12.5x10.9x12.5)     |
| 14 | 25.78 |   IC    |R.r=1.68; R.l=1.68| Benign = 0 Malignant = 1    | Benign = 0 Malignant = 0   |Right Breast: (11.2x11.0x10.3)     |
| 15 | 24.46 |   ILC   |     | Benign = 0 Malignant = 0    | Benign = 0 Malignant = 1   |Left Breast: (27.7x24.9x19.7)      |
| 16 | 24.14 |  -      |R.r=2.19; R.l=2.34| Benign = 0 Malignant = 0    | Benign = 0 Malignant = 1   |Left Breast: (11.5x12.1x14.8)      |
| 17 | 28.13 |   -     |R.r=2.09; R.l=2.11| Benign = 0 Malignant = 0    | Benign = 1 Malignant = 0   |Left Breast: (7.9x7.3x6.3)         |
| 18 | 29.36 |    -    |     | Benign = 2 Malignant = 0    | Benign = 0 Malignant = 0   |Right Breast: L=(49.0x36.6x35.1); S=(8.5x7.9x9.0)|
| 19 | 27.68 |    IC   |     | Benign = 0 Malignant = 0    | Benign = 0 Malignant = 1   |Left Breast: (29.56x30.01x19.33)   |
| 20 | 25.15 |     -   |     | Benign = 1 Malignant = 0    | Benign = 0 Malignant = 0   |Right Breast: (13.8x15.8x12.6)     |
| 21 | 24.54 |      -  |     | Benign = 0 Malignant = 1    | Benign = 0 Malignant = 0   |Right Breast: (11.4x11.4x10.6)     |
| 22 | 24.00 |    ILC  |     | Benign = 0 Malignant = 0    | Benign = 0 Malignant = 1   |Left Breast: (7.1x7.3x5.4)         |
| 23 | 30.12 |    IC   |     | Benign = 0 Malignant = 1    | Benign = 0 Malignant = 0   |Right Breast: (47.1x29.5x39.2)     |
| 24 | 22.60 |   IP    |R.r=2.07; R.l=2.11| Benign = 0 Malignant = 0    | Benign = 2 Malignant = 0   |Left Breast: L=(8.1x7.1x6.2); S=(5.4x5.4x5.0)|
| 25 | 25.80 |       - |     | Benign = 0 Malignant = 1    | Benign = 0 Malignant = 0   |Right Breast: (21.8x25.3x25.9)     |
| 26 | 24.65 |   IC    |     | Benign = 0 Malignant = 0    | Benign = 0 Malignant = 1   |Left Breast: (30.9x26.7x28.3)      |
| 27 | 24.13 |     IC  |     | Benign = 0 Malignant = 1    | Benign = 0 Malignant = 0   |Right Breast: (46.2x38.1x44.7)     |
| 28 | 22.51 |    -    |     | Benign = 0 Malignant = 0    | Benign = 1 Malignant = 0   |Left Breast: (16.2x19.3x16.1)     |
| 29 | 27.61 |    -    |     | Benign = 1 Malignant = 0    | Benign = 0 Malignant = 0   |Right Breast: (9.6x11.3x6.4)       |
| 30 | 43.18 |     -   |     | Benign = 2 Malignant = 0    | Benign = 3 Malignant = 0   |Right Breast:XL=(13.8x16.6x8.6); L=(13.2x15.7x11.4) & Left Breast: M=(10.0x10.8x7.9); S=(9.6x8.3x10.5); XS=(10.3x9.0x8.1)|
| 31 | 25.95 |      -  |     | Benign = 0 Malignant = 0    | Benign = 1 Malignant = 0   |Left Breast: (7.1x6.5x3.9)        |
| 32 | 24.02 |    F    |R.r=1.63; R.l=1.74| Benign = 0 Malignant = 0    | Benign = 1 Malignant = 0   |Left Breast:(6.9x6.8x8.2)        |
| 33 | 22.99 |       - |     | Benign = 0 Malignant = 0    | Benign = 0 Malignant = 1   |Left Breast: (15.2x17.4x13.7)     |
| 34 | 25.86 |      -  |     | Benign = 0 Malignant = 0    | Benign = 1 Malignant = 0   |Left Breast: (6.9x6.9x6.9)        |
| 35 | 21.88 |   IC    |     | Benign = 0 Malignant = 1    |Benign = 0 Malignant = 0    |Right Breast: (18.3x23.5x18.9)     |
| 36 | 31.18 |   IC    |     | Benign = 0 Malignant = 0     | Benign = 0 Malignant = 1   |Left Breast: (11.4x11.5x10.9)     |
| 37 | 25.97 |     -   |     | Benign = 0 Malignant = 0     |  Benign = 2 Malignant = 0  |Left Breast: L=(7.5x6.5x5.1); S=(6.4x3.2x5.8)    |
| 38 | 23.73 |      -  |     | Benign = 1 Malignant = 0     | Benign = 0 Malignant = 0   |Right Breast: (7.0x6.7x5.6)    |
| 39 | 19.28 |       - |     | Benign = 0 Malignant = 0     | Benign = 1 Malignant = 0   |Left Breast: (5.6x6.3x5.0)    |
| 40 | 23.12 |    IC   |     | Benign = 0 Malignant = 1    |Benign = 0 Malignant = 0    |Right Breast: (10.9x15.0x9.7)    |
| 41 | 21.72 |    IC   |R.r=1.33; R.l=1.52|  Benign = 2 Malignant = 1    |Benign = 2 Malignant = 0    |Right Breast: Malignant=(30.9X43.8X40.1); Benign XL=(19.4x26.8x28.7); Benign XS=(8.7x10.3x10.1) & Right Breast: Benign L=(23.6x20.2x19.7); Benign S=(12.3x15.8x14.0)|
| 42 | 21.45 |     -   |     | Benign = 1 Malignant = 0     |Benign = 0 Malignant = 0     |Right Breast: (9.1x9.1x7.6)    |
| 43 | 31.25 |     IC  |R.r=1.67; R.l=1.68| Benign = 0 Malignant = 0     |Benign = 0 Malignant = 1     |Left Breast: (16.7x17.3x15.9)  |
| 44 | 21.45 |     IC  |R.r=1.34; R.l=1.52| Benign = 0 Malignant = 1     |Benign = 0 Malignant = 0     |Right Breast: (42.5x37.4x29.0)  |
| 45 | 23.67 |     IC  |R.r=1.79; R.l=1.82| Benign = 0 Malignant = 2     |Benign = 1 Malignant = 0     |Right Breast: Malignant L=(34.9x43.3x39.8); Malignant S=(9.40x7.81x6.51) & Left Breast: Benign=(7.4x9.3x8.1)  |
| 46 | 34.38 |    IC   |     | Benign = 2 Malignant = 0     |Benign = 1 Malignant = 2     |Right Breast:Benign L=(9.2x10.8x9.5); Benign M=(9.2x10.3x9.4) & Left Breast: Malignant L=(40.3x41.8x21.1); Malignant S=(9.6x9.1x10.0); Benign S=(8.1x8.2x8.0) |
| 47 | 21.48 |      -  |R.r=1.55; R.l=1.63| Benign = 0 Malignant = 0     |Benign = 2 Malignant = 0    |Left Breast: L=(13.8x17.2x18.2); S=(7.4x6.9x6.3)  |
| 48 | 24.97 |  -      |R.r=2.15; R.l=2.29| Benign = 1 Malignant = 0     |Benign = 1 Malignant = 0    |Right Breast: L=(9.0x11.6x7.9) & Left Breast: S=(10.2x10.2x8.2)  |
| 49 | 20.96 |       - |     | Benign = 0 Malignant = 1      |Benign = 0 Malignant = 0    |Right Breast: (17.5x23.6x23.1)  |
| 50 | 35.16 |       - |R.r=2.48; R.l=2.52| Benign = 1 Malignant = 0      |Benign = 0 Malignant = 0    |Right Breast: (10.8x8.5x10.3)  |
| 51 | 24.09 |      -  |R.r=1.58; R.l=1.65| Benign = 1 Malignant = 0      | Benign = 0 Malignant = 0   | Right Breast: (6.9x8.1x8.7)  |
| 52 | 31.63 |       - |R.r=2.30; R.l=2.34| Benign = 2 Malignant = 0      |Benign = 1 Malignant = 0    |Right Breast: L=(16.1x19.4x11.8);M=(8.5x11.0x10.0) & Left Breast: S=(7.9x7.1x6.9)  |
| 53 | 22.66 |     IC  |     | Benign = 0 Malignant = 2      | Benign = 0 Malignant = 0   | Right Breast: L=(30.7x32.3x22.1); S=(4.8x5.7x4.8)  |
| 54 | 25.86 |        -|     | Benign = 0 Malignant = 0     |Benign = 1 Malignant = 0     |Left Breast: (6.8x6.1x5.7)   |
| 55 | 21.88 |    PC   |     | Benign = 0 Malignant = 1     | Benign = 0 Malignant = 0    |Right Breast: (20.9x20.8x15.7)   |

BMI = Body Mass Index;
XS - extra small size;
S - small size;
M - medium size;
L - large size;
XL - extra large size;

F = Fibroadenoma; IC = Invasive Carcinoma; IP= Intraductal Pappiloma; ILC = Invasive Lobular Carcinoma; PC = Pappilary Carcinoma

R = ratio between fibroglandular and fatty tissues. (R.r and R.l indicate the ratio for the right and left breast, respectively)



## Compatibility ##
All files are provided in MHA format. The files were created with the original resolution of the MRI scans.

## MRI Acquisition ##
Women were imaged in a prone position in a 3.0T MAGNETON Vida clinical MR scan (Siemens Healthineers, Erlangen – Germany) with a dedicated coil (Siemens Breast 18 coil) for the breast. This study was approved by the Scientific and Ethical Commission of Hospital da Luz – Lisboa, under references CES/44/2019/ME (19/09/2019) and CES/34/2020/ME (06/11/2020).

## Cite Us ##
If you use these models, please cite us:

Pelicano, A.C.; Gonçalves, M.C.T.; Godinho, D.M.; Castela, T.; Orvalho, M.L.; Araújo, N.A.M.; Porter, E.; Conceição, R.C. Development of 3D MRI-Based Anatomically Realistic Models of Breast Tissues and Tumours for Microwave Imaging Diagnosis. Sensors 2021, 21, 8265. https://doi.org/10.3390/s21248265

and

Pelicano, A.C.; Gonçalves, M.C.T.; Castela, T.; Orvalho, M.L.; Araújo, N.A.M.; Porter, E.; Conceição, R.C.; Godinho, D.M. Repository of MRI-derived models of the breast with single and multiple benign and malignant tumors for microwave imaging research. PLoS One 2024, 19(5):e0302974. https://doi.org/10.1371/journal.pone.0302974.

