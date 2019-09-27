# Celeb-DFF: A New Dataset for Celebrity DeepFake Forensics

## Overview
**Celebrity DeepFake Forensics (Celeb-DFF)** dataset contains  real and DeepFake synthesized videos having similar visual quality on par with those circulated online.
The Celeb-DFF dataset includes **158** real videos from youtube, and **795** DeepFake videos of human faces of different age, ethic group and gender, synthesized with these real videos. 

The demo video can be viewed here:

[![youtubev_video](https://img.youtube.com/.jpg)](https://www.youtube.com/)


## DFF Dataset
#### Real Videos
The real videos are collected from YouTube, which are split into two sets. 
The first set (*Real<sub>1</sub>*) contains 158 videos of 13 celebrities including 
different gender and skin color. The second set (*Real<sub>2</sub>*) includes 250 videos, 
where each video contains a different subject. 

#### Synthesized Videos
For each real video of a particular subject from the *Real<sub>1</sub>* set, we select multiple donors of the other subjects 
to create synthesized videos using the synthesis model trained between this target subject and each of the donor subjects. 

#### Dataset Structure
```commandline
Celeb-DFF
|--- Real_1 
|--- Real_2
|--- deepfake # Synthesized videos from Real_1
|--- test.txt # Videos used for testing
|--- summary_release.csv # Summary of each video including [label, video name, target name, donor name]
```

## Evaluation
Based on the Celeb-DFF dataset, we evaluate the performance of several recent 
DeepFake detection methods that have code publicly available.

<img src="src/eval.png" alt="eval" width="400"/>

* Two-stream: Zhou, Peng and Han, Xintong and Morariu, Vlad I and Davis, Larry S. "Two-stream neural networks for tampered face detection", 
IEEE Conference on Computer Vision and Pattern Recognition Workshops (CVPRW), 2017

* MesoNet: Afchar, Darius and Nozick, Vincent and Yamagishi, Junichi and Echizen, Isao.
"MesoNet: a Compact Facial Video Forgery Detection Network", IEEE International Workshop on Information Forensics and Security (WIFS), 2018

* HeadPose: Yang, Xin and Li, Yuezun and Lyu, Siwei. 
"Exposing Deep Fakes Using Inconsistent Head Poses",
IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP), 2019  

* Face Warping Artifacts (FWA): Li, Yuezun and Lyu, Siwei.
"Exposing DeepFake Videos By Detecting Face Warping Artifacts",
IEEE Conference on Computer Vision and Pattern Recognition Workshops (CVPRW), 2019  

* Visual Artifacts (VA): Matern, Falko and Riess, Christian and Stamminger, Marc.
"Exploiting Visual Artifacts to Expose Deepfakes and Face Manipulations",
IEEE Winter Applications of Computer Vision Workshops (WACVW), 2019

* Multi-task: Nguyen, Huy H and Fang, Fuming and Yamagishi, Junichi and Echizen, Isao.
"Multi-task Learning For Detecting and Segmenting Manipulated Facial Images and Videos",
arXiv preprint arXiv:1906.06876, 2019

* Xception: Andreas Rössler and Davide Cozzolino and Luisa Verdoliva and Christian Riess and Justus Thies and Matthias Nießner.
"FaceForensics++: Learning to Detect Manipulated Facial Images",
IEEE International Conference on Computer Vision (ICCV), 2019

## Download
If you would like to access the DFF dataset, 
please fill out [this form](https://docs.google.com/forms/d/e/1FAIpQLSdRRR3L5zAv6tQ_CKxmK4W96tAab_pfBu2EKAgQbeDVhmXagg/viewform).
The download link will be sent you once the form is accepted.

## Citation
Please cite our paper in your publications if the DFF dataset is used in your research:
```
@inproceedings{Li2019celebdff,
	author = {},
	title = {Celeb-DFF: A New Dataset for Celebrity DeepFake Forensics},
	booktitle= {ArXiv},
	year = {2019}
}

```

## Note
what else we need to tell?