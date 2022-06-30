# breast_models_repository

## Introduction & Motivation ##
Currently, this repository includes 6 anatomically realistic 3D numerical models of breast tissues and tumours of 2 patients obtained from breast Magnetic Resonance Imaging (MRI) scans. We chose to analyse one benign and one malignant breast tumour exams. The benign tumour corresponds to a standard benign infra-centimetric tumour of rounded shape and the selected malignant tumour is an invasive tumour of irregular shape, with approximately 8 cm along its major axis, and extremely heterogenous regarding voxels intensities.
The developed models include the dielectric properties of breast tissues and tumours between 3 and 10 GHz, suitable for MW applications, such as diagnosis and therapy, leveraging the simulation and experimental MicroWave Imaging (MWI) testing field.  
The purpose of this repository is to provide the research community with a repository of multiple anatomically realistic breast models, including benign and malignant tumorous tissues, which can be used for the improvement and validation of MWI systems.

## Repository Structure ##
We provide two folders, one for the benign tumour exam and the other for the malignant tumour exam. Both folders contain:
- Breast_mask, a mask of the breast region;
- Tumour_mask, a mask of the tumour;
- Label_map_simple, a lab map including tumour (label -3), skin (label -2), muscle (label -1), background (label 0), fat+fibroglandular (label 1);
- Label_map_detailed, a lab map including tumour (label -3), skin (label -2), muscle (label -1), background (label 0), fat_high (label 7), fat_median (label 6), fat_low (label 5), transition (label 4), fibroglandular_high (label 1), fibroglandular_median (label 2), fibroglandular_low (label 3);
- T1-w_Dixon-I_pre-processed, an in-phase image after bias correction, data normalisation, and background subtraction;
- Conductivity_(3,6 or 9)GHz, map with the estimated conductivity values for (3, 6 or 9) GHz.
- Permittivity_(3,6 or 9)GHz, map with the estimated relative permittivity values for (3, 6 or 9) GHz.

## Exams ##
| ID | No. Benign tumours | No. Malignant Tumours |
|:--:|:------------------:|:---------------------:|
| 01 |         1          |           0           |
| 02 |         0          |           1           |
| 03 |         0          |           1           |
| 04 |         1          |           1           |
| 05 |         2          |           0           |
| 06 |         0          |           1           |
| 07 |         0          |           1           |
| 08 |         2          |           1           |
| 09 |         0          |           0           |
| 10 |         0          |           1           |
| 11 |         0          |           1           |
| 12 |         0          |           2           |
| 13 |         0          |           1           |

## Compatibility ##
All files are provided in MHA format. The files were created with the original resolution of the MRI scans.

## MRI Acquisition ##
Women were imaged in a prone position in a 3.0T MAGNETON Vida clinical MR scan (Siemens Healthineers, Erlangen – Germany) with a dedicated coil (Siemens Breast 18 coil) for the breast. This study was approved by the Scientific and Ethical Commission of Hospital da Luz – Lisboa, under references CES/44/2019/ME (19/09/2019) and CES/34/2020/ME (06/11/2020).

## Cite Us ##
If you use some of these models, please cite us with:

Pelicano, A.C.; Gonçalves, M.C.T.; Godinho, D.M.; Castela, T.; Orvalho, M.L.; Araújo, N.A.M.; Porter, E.; Conceição, R.C. Development of 3D MRI-Based Anatomically Realistic Models of Breast Tissues and Tumours for Microwave Imaging Diagnosis. Sensors 2021, 21, 8265. https://doi.org/10.3390/s21248265
