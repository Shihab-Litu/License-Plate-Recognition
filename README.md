# License-Plate-Recognition

step1 : License plate detection

In order to detect licence we will use Yolo ( You Only Look One ) deep learning object detection architecture based on convolution neural networks.
This architecture was introduced by Joseph Redmon , Ali Farhadi, Ross Girshick and Santosh Divvala first version in 2015 and later version 2 and 3.


This network is extremely fast, it processes images in real-time at 45 frames per second. A smaller version of the network, Fast YOLO, processes an astounding 155 frames per second.Used darknet which is pretrained YOLO algorithm.


Step2 : Licence plate segmentation

Segmentation is one of the most important processes for the automatic identification of license plates, because any other step is based on it. If the segmentation fails, recognition phase will not be correct.To ensure proper segmentation, preliminary processing will have to be performed.
1. Input image 
2. BGR to RGB
3. Binarization
4. Blur
5. Segmentation

Step3 : Licence plate recognition

In order to make the most of the data available for learning, we cut each character indivudually by resizing it in a square after applying the same image processing steps used before segmentation of the license plate. As a result, we obtained a set of of data composed of 11 classes and for each class we have 30–40 images of 28X28 pixel dimesion PNG formats; numbers from 0 to 9.


![GitHub Logo](/OpenCV_3_License_Plate_Recognition_Python-master/imgOriginalScene.png)
Format: ![Alt Text](url)

