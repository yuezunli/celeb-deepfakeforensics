
## ***(New!)*** Check [here](Celeb-DF-v2/README.md) for Celeb-DF (v2) dataset (5639 DeepFake videos included!). 

# Celeb-DF (v1): A New Dataset for DeepFake Forensics

[Yuezun Li<sup>1</sup>](https://www.albany.edu/~yl149995/), 
Xin Yang<sup>1</sup>, Pu Sun<sup>2</sup>, Honggang Qi<sup>2</sup> and [Siwei Lyu<sup>1</sup>](http://www.cs.albany.edu/~lsw/)</br>
<sup>1</sup> University at Albany, State University of New York, USA; 
<sup>2</sup> University of Chinese Academy of Sciences, China</br>

Celeb-DF (v1) dataset contains real and DeepFake synthesized videos having similar visual quality on par with those circulated online. The Celeb-DF dataset includes 408 original videos collected from YouTube with subjects of different ages, ethic groups and genders, and 795 DeepFake videos synthesized from these real videos.

<a href="https://youtu.be/vLTiluewGQY">
<img src="src/cover.png" width="350" height="250" title="Video Demo" alt="Video Demo">
</a>

Video Demo of our dataset

### Download
If you would like to access the Celeb-DF dataset, 
please fill out [this form](https://drive.google.com/open?id=1zQSTM1Vjc5iJyI1_0pncOzuTOCwLSWld)
and send it to [deepfakeforensics@gmail.com](). The download link will be sent to you once the form is accepted.

Please cite our [paper](https://arxiv.org/abs/1909.12962) in your publications if the Celeb-DF dataset is used in your research:
```
@article{Li2019celebdf,
	author = {Yuezun Li, Xin Yang, Pu Sun, Honggang Qi and Siwei Lyu},
	title = {Celeb-DF: A New Dataset for DeepFake Forensics},
	Journal= {arXiv preprint arXiv:1909.12962},
	year = {2019}
}
```

### Dataset Structure
```commandline
Celeb-DF
|--- Celeb-real # Celebrity videos downloaded from YouTube
|--- YouTube-real # Additional videos downloaded from YouTube
|--- Celeb-synthesis # Synthesized videos from Celeb-real
|--- List_of_testing_videos.txt 
```

### Evaluation
Based on the Celeb-DF dataset, we evaluate the performance of several recent 
DeepFake detection methods that have code publicly available. Since not all methods have the code for training,
we use the released model performed on all datsets for evaluation.

<p align="center">
  <img src="src/eval.png" alt="eval" width="400"/>
</p>

## Privacy Statement
This dataset is released under the [Terms to Use Celeb-DF](https://drive.google.com/open?id=1zQSTM1Vjc5iJyI1_0pncOzuTOCwLSWld), which
is provided "as it is" and we are not responsible for any subsequence from using this dataset.
All original videos of the Celeb-DF dataset are obtained from the Internet which
are not property of the authors or the authors’ affiliated institutions. Neither the
authors or the authors’ affiliated institution are responsible for the content nor the
meaning of these videos. If you feel uncomfortable about your identity shown in this dataset, please contact us and we will 
remove corresponding information from the dataset. 


## Reference
<sub>
[1] Afchar, Darius and Nozick, Vincent and Yamagishi, Junichi and Echizen, Isao.
"MesoNet: a Compact Facial Video Forgery Detection Network", IEEE International Workshop on Information Forensics and Security (WIFS), 2018
</br>
[2] Korshunov, Pavel and Marcel, Sebastien.
"DeepFakes: a New Threat to Face Recognition? Assessment and Detection",
arXiv preprint arXiv:1812.08685, 2018 </br>
[3] Li, Yuezun and Lyu, Siwei.
"Exposing DeepFake Videos By Detecting Face Warping Artifacts",
IEEE Conference on Computer Vision and Pattern Recognition Workshops (CVPRW), 2019 </br>
[4] Matern, Falko and Riess, Christian and Stamminger, Marc.
"Exploiting Visual Artifacts to Expose Deepfakes and Face Manipulations",
IEEE Winter Applications of Computer Vision Workshops (WACVW), 2019
</br>
[5] Nguyen, Huy H and Fang, Fuming and Yamagishi, Junichi and Echizen, Isao.
"Multi-task Learning For Detecting and Segmenting Manipulated Facial Images and Videos",
arXiv preprint arXiv:1906.06876, 2019
</br>
[6] Andreas Rössler and Davide Cozzolino and Luisa Verdoliva and Christian Riess and Justus Thies and Matthias Nießner.
"FaceForensics++: Learning to Detect Manipulated Facial Images",
IEEE International Conference on Computer Vision (ICCV), 2019
</br>
[7] Yang, Xin and Li, Yuezun and Lyu, Siwei. 
"Exposing Deep Fakes Using Inconsistent Head Poses",
IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP), 2019 
</br>
[8] Zhou, Peng and Han, Xintong and Morariu, Vlad I and Davis, Larry S. "Two-stream neural networks for tampered face detection", 
IEEE Conference on Computer Vision and Pattern Recognition Workshops (CVPRW), 2017
