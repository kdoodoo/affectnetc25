# AffectNetC25

- Each Image was Annotated by 25 International Participants.<br>
  
|Experiment Set I |800 Confusing Images |25 Participants  |
|:-----------------|:--------------------|:---------------|
|Experiment Set II | 800 Random Images |25 Participants  |
|Total         | 1600 Images | 50 Participants  |

- ScreenShot of Free Annotation HTML-Javascript WebAPP.
<img src="https://raw.githubusercontent.com/kdoodoo/affectnetc25/main/html_js.png" width=60% >

### 8 Expressions, Arousal and Valence
|AffectNetC25 | Expression | Arousal | Valence | 
|:-----------|:-----------|:-----------|:-----------|
| Set I |   [expression_set1_C25.csv](https://github.com/kdoodoo/affectnetc25/blob/main/AffectNetC25/expression_set1_C25.csv) |  [arousal_set1_C25.csv](https://github.com/kdoodoo/affectnetc25/blob/main/AffectNetC25/arousal_set1_C25.csv) |[valence_set1_C25.csv](https://github.com/kdoodoo/affectnetc25/blob/main/AffectNetC25/valence_set1_C25.csv) | |
| Set II | [expression_set2_C25.csv](https://github.com/kdoodoo/affectnetc25/blob/main/AffectNetC25/expression_set2_C25.csv)  | [arousal_set2_C25.csv](https://github.com/kdoodoo/affectnetc25/blob/main/AffectNetC25/arousal_set2_C25.csv) |[valence_set2_C25.csv](https://github.com/kdoodoo/affectnetc25/blob/main/AffectNetC25/valence_set2_C25.csv) | |


| Expression Code |
|:----------------------|
| Code = {'happiness': 0,'sadness': 1, 'surprise': 2, 'fear': 3, 'disgust': 4, 'anger': 5, 'contempt': 6, 'neutral': 7}  |
|Arousal Rating Dimension|
| range = {-1.00,  -0.75,  -0.50,  -0.25,  0.00,  0.25,  0.50,  0.75,  1.00}|

-----------------------------------------
# Our Model 
- EXP: Expression, ARO: Arousal, VAL: Valence
  
|MODEL  | EXP, ARO, VAL| LINK |
|:------------- |:------------- |:----------|
| ResNet50 Fine-tuned | EXP, ARO, VAL|[LINK](https://drive.google.com/drive/folders/1hsxtU8t2keXSq7Z-d-RaYN0P14tCNbh4?usp=drive_link)
|ResNet50 Crowd Layer (MW, VW, VW+B)| EXP | [LINK](https://drive.google.com/drive/folders/1oDMCFqxT547wcsQ_ecdF4NjbkBvgoDbC?usp=drive_link)
|ResNet50 Crowd Layer (S+B)|ARO, VAL| [LINK](https://drive.google.com/drive/folders/11lLKZAHkXPlyZU_4lAA3aobOYwBiwQc1?usp=drive_link)
| EMONET Fine-tuned | ARO, VAL| [LINK](https://drive.google.com/drive/folders/1DzaPYztd7VvIwefJDNVkRJLSqOv1Uc1u?usp=drive_link) |
|EfficientNet B2 Fine-tuned| ARO, VAL| [LINK](https://drive.google.com/drive/folders/1k8eeeYMPUBdSO5dFgE38Pn_Fr2ygTGPr?usp=drive_link)|
|EfficientNet AFEW Fine-tuned |ARO, VAL| [LINK](https://drive.google.com/drive/folders/1ZihvEAEr_1HxPExT3RYW1mwFPVIsYvTC?usp=drive_link)|
|EfficientNet VGAF Fine-tuned |ARO, VAL| [LINK](https://drive.google.com/drive/folders/1w7j8gEZMYvWiOizGMcY6NLT6BhcdZlJS?usp=drive_link)|




---
# Model Reference 
|MODEL  | LINK |
| ------------- | ------------- |
| ResNet50  |[LINK](https://www.tensorflow.org/api_docs/python/tf/keras/applications/resnet50/ResNet50) |
| B2, AFEW, VGAF  |[LINK](https://github.com/av-savchenko/face-emotion-recognition) |
| EMONET  |[LINK](https://github.com/face-analysis/emonet) |
| DAN  |[LINK](https://github.com/yaoing/DAN) |
