# NOTE1: The Data is from the AffectNet.
Please DOWNLOAD from the link: 
http://mohammadmahoor.com/affectnet/
and Cite the following: 
Ali Mollahosseini, Behzad Hasani and Mohammad H. Mahoor, "AffectNet: A Database for Facial
Expression, Valence, and Arousal Computing in the Wild," in IEEE Transactions on Affective Computing,
vol. 10, no. 1, pp. 18-31, 1 Jan.-March 2019, doi: 10.1109/TAFFC.2017.2740923.'


# NOTE2: The Data and Code Here is under review in IEEE journal. 
The information transmitted, including any attachments, is intended only for the person or entity to which it is addressed and may contain confidential and/or privileged material. 
Any review, retransmission, dissemination or other use of, including academiccal and personal use,  or taking of any action in reliance upon, this information by persons or entities other than the intended recipient is prohibited, 
and all liability arising therefrom is disclaimed. If you received and seen this in error, please contact the sender and delete the material from any computer.




# AffectNetC25

- Each Image was Annotated by 25 International Participants.<br>
  
|Experiment Set I |800 Confusing Images |25 Participants |
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
|Arousal and Valence Dimension|
| range = {-1.00,  -0.75,  -0.50,  -0.25,  0.00,  0.25,  0.50,  0.75,  1.00}|

-----------------------------------------
# Our Model 
- EXP: Expression, ARO: Arousal, VAL: Valence
- MV : Majority Vote, CV : Crowd Vote
  
|MODEL  | Data| EXP, ARO, VAL| LINK | NOTE|
|:------------- |:-------------|:------------- |:----------|:----------|
|ResNet50 Fine-tuned | AffectNetC25 MV|EXP, ARO, VAL|[LINK](https://drive.google.com/drive/folders/1hsxtU8t2keXSq7Z-d-RaYN0P14tCNbh4?usp=drive_link) | TensorFlow |
|ResNet50 Crowd Layer (MW, VW, VW+B) | AffectNetC25 CV| EXP | [LINK](https://drive.google.com/drive/folders/1oDMCFqxT547wcsQ_ecdF4NjbkBvgoDbC?usp=drive_link) | TensorFlow |
|ResNet50 Crowd Layer (S+B) | AffectNetC25 CV|ARO, VAL| [LINK](https://drive.google.com/drive/folders/11lLKZAHkXPlyZU_4lAA3aobOYwBiwQc1?usp=drive_link)| TensorFlow |
|EMONET Fine-tuned | AffectNetC25 MV| ARO, VAL| [LINK](https://drive.google.com/drive/folders/1DzaPYztd7VvIwefJDNVkRJLSqOv1Uc1u?usp=drive_link) | Pytorch |
|EfficientNet B2 | AffectNet| ARO, VAL| [LINK](https://drive.google.com/drive/folders/1k8eeeYMPUBdSO5dFgE38Pn_Fr2ygTGPr?usp=drive_link)| Pytorch |
|EfficientNet AFEW  | AffectNet|ARO, VAL| [LINK](https://drive.google.com/drive/folders/1ZihvEAEr_1HxPExT3RYW1mwFPVIsYvTC?usp=drive_link)| Pytorch |
|EfficientNet VGAF | AffectNet|ARO, VAL| [LINK](https://drive.google.com/drive/folders/1w7j8gEZMYvWiOizGMcY6NLT6BhcdZlJS?usp=drive_link)| Pytorch |




---
# Reference
|MODEL  | LINK |
| ------------- | ------------- |
| ResNet50  |[LINK](https://www.tensorflow.org/api_docs/python/tf/keras/applications/resnet50/ResNet50) |
| Crowd Layer  |[LINK](https://github.com/fmpr/CrowdLayer) |
| EfficientNet (B2, AFEW, VGAF)  |[LINK](https://github.com/av-savchenko/face-emotion-recognition) |
| EMONET  |[LINK](https://github.com/face-analysis/emonet) |
| DAN  |[LINK](https://github.com/yaoing/DAN) |
