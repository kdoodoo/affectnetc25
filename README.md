# NOTE1: We obtained written permission from the University of Denver, Office of IP & Tech Transfer.

Before Use:

1. Cite: <br>
Ali Mollahosseini, Behzad Hasani, and Mohammad H. Mahoor, “AffectNet: A New Database for Facial Expression, Valence, and Arousal Computation in the Wild”, IEEE Transactions on Affective Computing, 2017<br>
2. Refer to http://mohammadmahoor.com/affectnet/ <br>
and DOWNLOAD AffectNet, firstly.

<!--http://mohammadmahoor.com/affectnet/
and Cite the following: <br>
Ali Mollahosseini, Behzad Hasani and Mohammad H. Mahoor, "AffectNet: A Database for Facial
Expression, Valence, and Arousal Computing in the Wild," in IEEE Transactions on Affective Computing,
vol. 10, no. 1, pp. 18-31, 1 Jan.-March 2019, doi: 10.1109/TAFFC.2017.2740923.'-->

# AffectNetC25
We named the new annotation as AffectNetC25 as 'C25' means **Crowd and 25 people**. 
<br>
|index|filename |Participant1 |Participant2 |Participant3 |...|Participant25 |
|:----|:--------|:------------|:------------|:------------|:----|:-----------|
|123| abc.jpg |5 |2 |5 |...|8 |
|789| xyz.jpg |4|4 |5 |...|4 |

<br>

1. We included **index** of the images. <br>
Indeces are counted rows of the **Training.csv** file of the AffectNet. (which we _counted_ from 0) <br>  
2. We included **filenames** of the images. <br>
3. Each Image was Annotated by **25 International Participants**.<br>

  
|Set  | Images |Participants |
|:-----------------|:--------------------|:---------------|
|Experiment Set I |800 Confusing Images |25 Participants |
|Experiment Set II | 800 Random Images |25 Participants  |
|Total         | 1600 Images | 50 Participants  |

- ScreenShot of Free Annotation HTML-Javascript WebAPP.
- A Facial image of human is located at the top (Green Alien now), during the experiments.
<img src="https://raw.githubusercontent.com/kdoodoo/affectnetc25/html_js1.png" width=60% >



### 8 Expressions, Arousal and Valence
|AffectNetC25 | Expression | Arousal | Valence | 
|:-----------|:-----------|:-----------|:-----------|
| Set I |   [expression_set1_C25.csv](https://github.com/kdoodoo/affectnetc25/blob/main/AffectNetC25/expression_set1_c25.csv) |  [arousal_set1_C25.csv](https://github.com/kdoodoo/affectnetc25/blob/main/AffectNetC25/arousal_set1_c25.csv) |[valence_set1_c25.csv](https://github.com/kdoodoo/affectnetc25/blob/main/AffectNetC25/valence_set1_c25.csv) | |
| Set II | [expression_set2_C25.csv](https://github.com/kdoodoo/affectnetc25/blob/main/AffectNetC25/expression_set2_c25.csv)  | [arousal_set2_C25.csv](https://github.com/kdoodoo/affectnetc25/blob/main/AffectNetC25/arousal_set2_c25.csv) |[valence_set2_c25.csv](https://github.com/kdoodoo/affectnetc25/blob/main/AffectNetC25/valence_set2_c25.csv) | |


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


# NOTE2: The Data and Code Here is under review in IEEE journal. 
The information transmitted, including any attachments, is intended only for the person or entity to which it is addressed and may contain confidential and/or privileged material. 
Any review, retransmission, dissemination or other use of, including academiccal and personal use,  or taking of any action in reliance upon, this information by persons or entities other than the intended recipient is prohibited, 
and all liability arising therefrom is disclaimed. If you received and seen this in error, please contact the sender and delete the material from any computer.


<!--Images are from AffectNet: 
Ali Mollahosseini, Behzad Hasani and Mohammad H. Mahoor, "AffectNet: A Database for Facial Expression, Valence, and Arousal Computing in the Wild," in IEEE Transactions on Affective Computing, vol. 10, no. 1, pp. 18-31, 1 Jan.-March 2019, doi: 10.1109/TAFFC.2017.2740923.'-->

---
# Reference
|MODEL  | LINK |
| ------------- | ------------- |
| ResNet50  |[LINK](https://www.tensorflow.org/api_docs/python/tf/keras/applications/resnet50/ResNet50) |
| Crowd Layer  |[LINK](https://github.com/fmpr/CrowdLayer) |
| EfficientNet (B2, AFEW, VGAF)  |[LINK](https://github.com/av-savchenko/face-emotion-recognition) |
| EMONET  |[LINK](https://github.com/face-analysis/emonet) |
| DAN  |[LINK](https://github.com/yaoing/DAN) |

AffectNet:<br>
```@ARTICLE {8013713,
author = {A. Mollahosseini and B. Hasani and M. H. Mahoor},
journal = {IEEE Transactions on Affective Computing},
title = {AffectNet: A Database for Facial Expression, Valence, and Arousal Computing in the Wild},
year = {2019},
volume = {10},
number = {01},
issn = {1949-3045},
pages = {18-31},
keywords = {databases;computational modeling;face;face recognition;affective computing;magnetic heads},
doi = {10.1109/TAFFC.2017.2740923},
publisher = {IEEE Computer Society},
address = {Los Alamitos, CA, USA},
month = {jan}
}
```

ResNet50:<br>
```@misc{he2015deep,
      title={Deep Residual Learning for Image Recognition}, 
      author={Kaiming He and Xiangyu Zhang and Shaoqing Ren and Jian Sun},
      year={2015},
      eprint={1512.03385},
      archivePrefix={arXiv},
      primaryClass={id='cs.CV' full_name='Computer Vision and Pattern Recognition' is_active=True alt_name=None in_archive='cs' is_general=False description='Covers image processing, computer vision, pattern recognition, and scene understanding. Roughly includes material in ACM Subject Classes I.2.10, I.4, and I.5.'}
}
```
Crowd Layer:<br>
```
@inproceedings{10.5555/3504035.3504232,
author = {Rodrigues, Filipe and Pereira, Francisco C.},
title = {Deep learning from crowds},
year = {2018},
isbn = {978-1-57735-800-8},
publisher = {AAAI Press},
booktitle = {Proceedings of the Thirty-Second AAAI Conference on Artificial Intelligence and Thirtieth Innovative Applications of Artificial Intelligence Conference and Eighth AAAI Symposium on Educational Advances in Artificial Intelligence},
articleno = {197},
numpages = {8},
location = {New Orleans, Louisiana, USA},
series = {AAAI'18/IAAI'18/EAAI'18}
}
```

EfficientNet:

```@inproceedings{savchenko2023facial,
  title = 	 {Facial Expression Recognition with Adaptive Frame Rate based on Multiple Testing Correction},
  author =       {Savchenko, Andrey},
  booktitle = 	 {Proceedings of the 40th International Conference on Machine Learning (ICML)},
  pages = 	 {30119--30129},
  year = 	 {2023},
  editor = 	 {Krause, Andreas and Brunskill, Emma and Cho, Kyunghyun and Engelhardt, Barbara and Sabato, Sivan and Scarlett, Jonathan},
  volume = 	 {202},
  series = 	 {Proceedings of Machine Learning Research},
  month = 	 {23--29 Jul},
  publisher =    {PMLR},
  url={https://proceedings.mlr.press/v202/savchenko23a.html}
}
```
```@inproceedings{savchenko2021facial,
  title={Facial expression and attributes recognition based on multi-task learning of lightweight neural networks},
  author={Savchenko, Andrey V.},
  booktitle={Proceedings of the 19th International Symposium on Intelligent Systems and Informatics (SISY)},
  pages={119--124},
  year={2021},
  organization={IEEE},
  url={https://arxiv.org/abs/2103.17107}
}
```
```@inproceedings{Savchenko_2022_CVPRW,
  author    = {Savchenko, Andrey V.},
  title     = {Video-Based Frame-Level Facial Analysis of Affective Behavior on Mobile Devices Using EfficientNets},
  booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
  month     = {June},
  year      = {2022},
  pages     = {2359-2366},
  url={https://arxiv.org/abs/2103.17107}
}
```
```@inproceedings{Savchenko_2022_ECCVW,
  author    = {Savchenko, Andrey V.},
  title     = {{MT-EmotiEffNet} for Multi-task Human Affective Behavior Analysis and Learning from Synthetic Data},
  booktitle = {Proceedings of the European Conference on Computer Vision (ECCV 2022) Workshops},
  pages={45--59},
  year={2023},
  organization={Springer},
  url={https://arxiv.org/abs/2207.09508}
}
```
```@article{savchenko2022classifying,
  title={Classifying emotions and engagement in online learning based on a single facial expression recognition neural network},
  author={Savchenko, Andrey V and Savchenko, Lyudmila V and Makarov, Ilya},
  journal={IEEE Transactions on Affective Computing},
  year={2022},
  publisher={IEEE},
  url={https://ieeexplore.ieee.org/document/9815154}
}
```
EmoNet:<br>

```@article{toisoul2021estimation,
  author  = {Antoine Toisoul and Jean Kossaifi and Adrian Bulat and Georgios Tzimiropoulos and Maja Pantic},
  title   = {Estimation of continuous valence and arousal levels from faces in naturalistic conditions},
  journal = {Nature Machine Intelligence},
  year    = {2021},
  url     = {https://www.nature.com/articles/s42256-020-00280-0}
}
```

DAN:<br>

```@article{Wen_2023,
   title={Distract Your Attention: Multi-Head Cross Attention Network for Facial Expression Recognition},
   volume={8},
   ISSN={2313-7673},
   url={http://dx.doi.org/10.3390/biomimetics8020199},
   DOI={10.3390/biomimetics8020199},
   number={2},
   journal={Biomimetics},
   publisher={MDPI AG},
   author={Wen, Zhengyao and Lin, Wenzhong and Wang, Tao and Xu, Ge},
   year={2023},
   month=may, pages={199} }
```

