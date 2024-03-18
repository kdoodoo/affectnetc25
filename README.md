# AffectNetC25

|Experiment Set I |800 Confuning Images |25 Crowd  |
|:-----------------|:--------------------|:---------------|
|Experiment Set II | 800 Random Images |25 Crowd  |
|Total         | 1600 Images | 50 Participants  |


- Each Image was Annotated by 25 International Participants.<br>
- ScreenShot of Free Annotation HTML-Javascript WebAPP. 

<img src="https://raw.githubusercontent.com/kdoodoo/affectnetc25/main/html_js.png" width=75% >


---
# 8 Expressions
| Expression Code |
| :------------- |
| Code = {'happiness': 0,'sadness': 1, 'surprise': 2, 'fear': 3, 'disgust': 4, 'anger': 5, 'contempt': 6, 'neutral': 7}  |


| Set I | expression_set1_C25.csv |
| ------------- | ------------- |
| Set II | expression_set2_C25.csv |


# Arousal
|Arousal Rating Dimension|
| :------------------------- |
| range = {-1.00, -0.75. -0.50, -0.25, 0.00, 0.25, 0.50, 0.75, 1.00}|

| Set I | arousal_set1_C25.csv |
| :------------- | :------------- |
| Set II | arousal_set2_C25.csv |

# Valence
|Valence Rating Dimension|
| :------------------------- |
| range = {  -1.00, -0.75. -0.50, -0.25, 0.00, 0.25, 0.50, 0.75, 1.00}|


| Set I | valence_set1_C25.csv |
| :------------- | :------------- |
| Set II | valence_set2_C25.csv |
--
# Our Model Links
|MODEL  | EXP, ARO, VAL| LINK |
|:------------- |:------------- |:----------|
| EMONET Finetuned | ARO, VAL|[LINK](https://drive.google.com/drive/folders/1DzaPYztd7VvIwefJDNVkRJLSqOv1Uc1u?usp=drive_link) |




---
# Reference Model 
|MODEL  | LINK |
| ------------- | ------------- |
| ResNet50  |[LINK](https://www.tensorflow.org/api_docs/python/tf/keras/applications/resnet50/ResNet50) |
| B2, AFEW, VGAF  |[LINK](https://github.com/av-savchenko/face-emotion-recognition) |
| EMONET  |[LINK](https://github.com/face-analysis/emonet) |
| DAN  |[LINK](https://github.com/yaoing/DAN) |
