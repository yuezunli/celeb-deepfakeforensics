# DeepFake Game Competition (DFGC) Dataset 2021

## Introduction
This dataset is collected from the [DeepFake Game Competition (DFGC)](https://competitions.codalab.org/competitions/29583#learn_the_details-overview)
 held at [IJCB-21](http://ijcb2021.iapr-tc4.org/). The fake subsets are created by DFGC creation track participants 
based on the [Celeb-DF v2 dataset](https://github.com/yuezunli/celeb-deepfakeforensics). They are created by a variety of 
faceswap methods, and many are post processed with adversarial noises, making them hard to be detected by deepfake detection 
models. This dataset can be used as a held-out testing dataset to evaluate the generalization ability and robustness 
of newly proposed detection models.  
For more details, please see our competition paper.

## Dataset Structure
Each subset (real or fakes) contains 1,000 frame images that are from the [test-split](https://github.com/bomb2peng/DFGC_starterkit/blob/master/test-list.txt) of Celeb-DF v2 videos.
For more information on how the fake subsets are specified, please see the "List Files" section of [DFGC starter-kit](https://github.com/bomb2peng/DFGC_starterkit).
### Description of Subsets
|  Subset   | Method  |
|  ----  | ----  |
| real_fulls.zip |   original Celeb-DF real data |  
|fake_baseline.zip	|				 original Celeb-DF fake data|  
|DFGC_SYSU_852924.zip    |		 Adversarial Attacks with some post processing|  
|jerryHUST_853638.zip  		|	 FaceShifter + Adversarial Attacks; A self-trained faceswap model with some post processing|  
|miaotao_853000.zip  		|	 FaceShifter|  
|seanseattle_853068.zip  	|	 FaceController + Adversarial Attacks    |  
|yZzzzzz_849853.zip			|	 MegaFS on 256 resolution|  
|DFischerHDA_852673.zip  	|	 FaceMorpher + dlib landmarks +|  
|joshhu_853266.zip  		|		 Adversarial Attacks   |  
|nbhh_853436.zip     		|	 FaceShifter + Adversarial Attacks|  
|smartz_849705.zip       	|	 A face-anonymization algorithm generated data|  
|yangquanwei_852303.zip  	|	 Swap facial regions based on key points of the face|  
|zhaobh_852336.zip			|	 Using an adversarial model to generate noise to add on warp-based face swap results|  
|ctmiu_853213.zip   		|		 FaceShifter + Adversarial Attacks  |  
|lowtec_853184.zip   		|	 FacceShifter with some post processing      |  
|wany_853175.zip   			|	 face shifter      |  
|yuejiang_852934.zip    	|		 crop and paste |  
|zz110_853170.zip			|	 unkown|  
### Metadata
*bbox&landmarks.json* includes the pre-computed bounding-box, 5-landmarks, and 68 landmarks information.
Bounding-box and 5-landmarks are extracted using MTCNN.
The real images metadata are extracted for the *real_fulls* subset. The fake subsets (approximately) share the same 
metadata, which is extracted based on *fake_baseline*.

## How to Use
We recommend to only use this dataset as a held-out testing dataset. 

As the number of real samples 
are much less than the total fake samples, mean metric over each pair of real-fake sets can be calculated.
This can give more weight to each real sample.
E.g. in the DFGC-2021, we use the mean AUROC to report performance on the dataset.

## Citation
To use this dataset in your work, please cite the following two papers:  
```
@inproceedings{DFGC_2021,  
   author = {Bo Peng, Hongxing Fan, Wei Wang, Jing Dong, Yuezun Li, Siwei Lyu, 
   Qi Li, Zhenan Sun, Han Chen, Baoying Chen, Yanjie Hu, Shenghai Luo, Junrui Huang, 
   Yutong Yao, Boyuan Liu, Hefei Ling, Guosheng Zhang, Zhiliang Xu, Changtao Miao, 
   Changlei Lu, Shan He, Xiaoyan Wu, Wanyi Zhuang},  
   title = {DFGC 2021: A DeepFake Game Competition},  
   booktitle= {IJCB},  
   year = {2021}  
}  
@inproceedings{Celeb_DF_cvpr20,  
   author = {Yuezun Li, Xin Yang, Pu Sun, Honggang Qi and Siwei Lyu},  
   title = {Celeb-DF: A Large-scale Challenging Dataset for DeepFake Forensics},  
   booktitle= {IEEE Conference on Computer Vision and Patten Recognition (CVPR)},  
   year = {2020}  
}  
```

## Acknowledgement
We would also like to thank the following DFGC-21 participants (among some other anonymous ones) for sharing their created DeepFake datasets to the research community:   
*Zhiliang Xu, Quanwei Yang, Fengyuan Liu, Hang Cai, Shan He, Christian Rathgeb, Daniel Fischer, Binghao Zhao, Li Dongze.*