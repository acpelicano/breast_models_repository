# breast_models_repository

## Introduction & Motivation ##
This repository includes 6 anatomically realistic 3D numerical models of breast tissues and tumours of 2 patients obtained from breast Magnetic Resonance Imaging (MRI) scans. We chose to analyse one benign and one malignant breast tumour exams. The benign tumour corresponds to a standard benign infra-centimetric tumour of rounded shape and the selected malignant tumour is an invasive tumour of irregular shape, with approximately 8 cm along its major axis, and extremely heterogenous regarding voxels intensities.
The developed models include the dielectric properties of breast tissues and tumours between 3 and 10 GHz, suitable for MW applications, such as diagnosis and therapy, leveraging the simulation and experimental MicroWave Imaging (MWI) testing field.  
The purpose of this repository is to provide the research community with the first available repository of realistic breast tissues, as well as tumorous tissues, which can be used for the improvement and validation of MWI systems.

## Repository Structure ##
We provide two folders, one for the benign tumour exam and the other for the malignant tumour exam. Both folders contain:
- Breast_mask, a mask for the breast region;
- Label_map_simple, a lab map including tumour (label -3), skin (label -2), muscle (label -1), background (label 0), fat+fibroglandular (label 1);
- Label_map_simple, a lab map including tumour (label -3), skin (label -2), muscle (label -1), background (label 0), fat_high (label 1), fat_median (label 2), fat_low (label 3), transition (label 4), fibroglandular_high (label 5), fibroglandular_median (label 6), fibroglandular_low (label 7);
- T1-w_Dixon-I_pre-processed, an in-phase image after bias correction, data normalisation, and background subtraction;
- Conductivity_(3,6 or 9)GHz, map with the estimated conductivity values for (3, 6 or 9) GHz.
- Permittivity_(3,6 or 9)GHz, map with the estimated relative permittivity values for (3, 6 or 9) GHz.

## Compatibility ##
All files are provided in MHA format. The files were created with the original resolution of the MRI scans.

## MRI Acquisition ##
Women were imaged in a prone position in a 3.0T MAGNETON Vida clinical MR scan (Siemens Healthineers, Erlangen – Germany) with a dedicated coil (Siemens Breast 18 coil) for the breast. This study was approved by the Scientific and Ethical Commission of Hospital da Luz – Lisboa, under references CES/44/2019/ME (19/09/2019) and CES/34/2020/ME (06/11/2020).

## Cite Us ##
If you use some of these models, please cite us with:

Ana Catarina Pelicano, Maria C. T. Gonçalves, Daniela M. Godinho, Tiago Castela, M. Lurdes Orvalho, Nuno A. M. Araújo, Emily Porter, and Raquel C. Conceição, “Development of 3D MRI-based anatomically realistic numeri-cal models of breast tissues and tumours for Microwave Imag-ing diagnosis” (under review in Sensors, 2021).
