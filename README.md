# Application of data preprocessing to improve the diagnostic efficiency of chest X-ray images
Use preprocessing techniques to highlight the lung regions to classify lung diseases

## Overview
* Use Noise Removal, Diaphragm Removal and Contrast Enrichment for data preprocessing.
* Compare different pre-trained models for classify lung diseases.

## Preprocess
### Background Removal
<img src="images/bg_rm.png" width=50% height=50%>

### Diaphragm Removal
<img src="images/dp_rm.png" width=50% height=50%>

### Contrast Enrichment
<img src="images/contrast_rm.png" width=50% height=50%>

## Experiment
### NIH dataset
| Model | Without Preprocessing  | Preprocessing | 
|:-------------| :-------------: | :-------------: | 
|Dense121| 49.38 | **55.46** | 
|VGG19 | 62.91 | **64.50**  | 
|EfficientNetV2| 68.81 | **69.21** |
|ConvNeXt | 75.60 | **77.22** |

### CheXpert-small
| Model | Without Preprocessing  | Preprocessing | 
|:-------------| :-------------: | :-------------: | 
|Dense121| 65.16 | **68.39** | 
|VGG19 | **63.59** | 60.98  | 
|EfficientNetV2| 66.45 | **68.64** |
|ConvNeXt | 68.21 | **73.84** |

