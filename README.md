# breast_models_repository

## Introduction & Motivation ##
The purpose of this repository is to provide the research community with a repository of multiple anatomically realistic breast models, including benign and malignant tumorous tissues, which can be used for the improvement and validation of Microwave Imaging (MWI) systems.
The developed models include the dielectric properties of breast tissues and tumours at 3, 6 and 9 GHz, suitable for MW applications, such as diagnosis and therapy, leveraging the simulation and experimental MWI testing field.  
Currently, this repository includes 84 3D anatomically realistic numerical models of breast tissues with a total of 18 tumours (6 benign and 12 malignant) obtained from breast Magnetic Resonance Imaging (MRI) scans of 14 patients.

## Repository Structure ##
We provide two folders, one for the benign tumour exam and the other for the malignant tumour exam. Both folders contain:
- Breast_mask, a mask of the breast region;
- Tumour_mask, a mask of the tumour;
- Label_map_simple, a lab map including tumour (label -3), skin (label -2), muscle (label -1), background (label 0), fat+fibroglandular (label 1);
- Label_map_detailed, a lab map including tumour (label -3), skin (label -2), muscle (label -1), background (label 0), fat_high (label 7), fat_median (label 6), fat_low (label 5), transition (label 4), fibroglandular_high (label 3), fibroglandular_median (label 2), fibroglandular_low (label 1) - the labels low, median and high refer to the voxel intensities;
- T1-w_Dixon-I_pre-processed, an in-phase image after bias correction, data normalisation, and background subtraction;
- Conductivity_(3,6 or 9)GHz, map with the estimated conductivity values for (3, 6 or 9) GHz.
- Permittivity_(3,6 or 9)GHz, map with the estimated relative permittivity values for (3, 6 or 9) GHz.

## Exams ##
| ID | No. Benign tumours | No. Malignant Tumours | Size of Tumours (mm) |
|:--:|:------------------:|:---------------------:|:--------------------:|
| 01 |         1          |           0           | (6.9x6.9x5.2)        |
| 02 |         0          |           1           | (80.9x74.9x56.2)     |
| 03 |         0          |           1           | (8.5x11.2x9.2)       |
| 04 |         1          |           1           |Benign(14.0x11.1x6.5) Malignant(9.7x8.7x8.6)|
| 05 |         2          |           0           |Bigger(19.1x19.6x18.2) Smaller(15.5x15.3x13.7)|
| 06 |         0          |           1           |(12.8x13.5x14.4)      |
| 07 |         0          |           1           |(8.4x12.4x10.5)       |
| 08 |         0          |           1           |(18.8x19.1x20.2)      |
| 09 |         2          |           0           |Bigger(9.7x7.8x5.4) Smaller(6.1x5.7x5.6)|
| 10 |         0          |           1           |(23.1x24.0x23.2)      |
| 11 |         0          |           1           |(33.2x32.6x29.9)      |
| 12 |         0          |           2           |Bigger(11.2x8.9x6.8) Smaller(10.0x10.1x7.7)|
| 13 |         0          |           1           | (12.5x10.9x12.5)     |
| 14 |         0          |           1           |(11.2x11.0x10.3)      |

## Compatibility ##
All files are provided in MHA format. The files were created with the original resolution of the MRI scans.

## MRI Acquisition ##
Women were imaged in a prone position in a 3.0T MAGNETON Vida clinical MR scan (Siemens Healthineers, Erlangen – Germany) with a dedicated coil (Siemens Breast 18 coil) for the breast. This study was approved by the Scientific and Ethical Commission of Hospital da Luz – Lisboa, under references CES/44/2019/ME (19/09/2019) and CES/34/2020/ME (06/11/2020).

## Cite Us ##
If you use some of these models, please cite us with:

Pelicano, A.C.; Gonçalves, M.C.T.; Godinho, D.M.; Castela, T.; Orvalho, M.L.; Araújo, N.A.M.; Porter, E.; Conceição, R.C. Development of 3D MRI-Based Anatomically Realistic Models of Breast Tissues and Tumours for Microwave Imaging Diagnosis. Sensors 2021, 21, 8265. https://doi.org/10.3390/s21248265
