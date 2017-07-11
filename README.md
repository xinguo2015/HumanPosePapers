### Direct Prediction of 3D Body Poses from Motion Compensated Sequences
```
@InProceedings{ Tekin_2016_CVPR,
	author = {Tekin, Bugra and Rozantsev, Artem and Lepetit, Vincent and Fua, Pascal},
	title = {Direct Prediction of 3D Body Poses From Motion Compensated Sequences},
	booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
	month = {June},
	year = {2016}
}
```
- 取当前帧的前后多帧
- 提取身体bounding box
  - Deformable Part Model (DPM) detector
- 形成一个volume
- 计算 3D HoG feature descriptor
- regression, 三种不同的方法：
	- deep neural network
	- kernal rig regression 
	- kernel dependency estimation (kde)



### Structured Prediction of 3D Human Pose with Deep Neural Networks

```
@ARTICLE{2016arXiv160505180T,
	author = {{Tekin}, B. and {Katircioglu}, I. and {Salzmann}, M. and {Lepetit}, V. and {Fua}, P.},
	title = "{Structured Prediction of 3D Human Pose with Deep Neural Networks}",
	journal = {ArXiv e-prints},
	archivePrefix = "arXiv",
	eprint = {1605.05180},
	primaryClass = "cs.CV",
	keywords = {Computer Science - Computer Vision and Pattern Recognition},
	year = 2016,
	month = may,
}

```
训练一个autoencoder，将3D pose编码为高维latent向量
训练一个CNN，将图像表示为latent向量
运行时，图像-> latent向量-> 3D pose

### Reconstructing 3D Human Pose from 2D Image Landmarks. 
Varun Ramakrishna, Takeo Kanade, Yaser Sheikh
European Conference on Computer Vision, 2012.

https://github.com/varunnr/camera_and_pose

 - 将3D的POSE进行稀疏表达


### Comments
Pose from monocular image/video
 - fenforcing physical constraints at test time
 - data-driven priors over the pose space
 - max margin formalism based deep learning framework

### Pose Data Sets
1. Leeds Sports Pose Dataset
   http://www.comp.leeds.ac.uk/mat4saj/lsp.html
   This dataset contains 2000 pose annotated images of mostly sports people gathered from Flickr using the tags shown above. The images have been scaled such that the most prominent person is roughly 150 pixels in length. Each image has been annotated with 14 joint locations. Left and right joints are consistently labelled from a person-centric viewpoint. Attributions and Flickr URLs for the original images can be found in the JPEG comment field of each image file.

2. VGG Human Pose Estimation Datasets (Upper Body only)
   https://www.robots.ox.ac.uk/~vgg/data/pose/

   The VGG Human Pose Estimation datasets is a set of large video datasets annotated with human upper-body pose. This data is made available to the computer vision community for research purposes. 

3. Human3.6M
   http://vision.imar.ro/human3.6m/description.php

   - 3.6 million 3D human poses and corresponding images 
   - 11 professional actors (6 male, 5 female) 
   - 17 scenarios (discussion, smoking, taking photo, talking on the phone...)




