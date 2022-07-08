# Counting-Problem2

In this exercise, we aim to adopt the source code from [1] to implement the vehicle tracking algorithm using YOLO (You Only Look Once) [2] and Deep Sort (Simple online and Realtime Tracking) [3] in order to solve the vehicle counting problem via learning methodology. Unfortunately, we fail to establish the development environment for python running CUDA and sort of machine learning tools due to unexpected hardware limitations (we will fix it up soon). Nevertheless, we can figure out the big picture of multi-object tracking which is a main philosophy of vehicle counting problem by referring to [4]. For object detection, YOLO is one of the most popular object detection algorithms which is able to output a list of bounding boxes representing the objects in the frame with less computational complexity and better efficiency compare to the traditional algorithms. On the other hand, for object tracking, the Deep Sort algorithm achieves competitive performance at high frame rates. With the aid of the hungarian algorithm and the well-known Kalman filter, the Deep Sort algorithm can endure the occlusion in case of some practical scene. Notably, the hungarian algorithm is to evaluate the association between the objects in one frame to another frame; the Kalman filter is to predict the motion of the object by using constant velocity model. Therefore, with YOLO and Deep Sort, we can present a high efficient and effective algorithm for vehicle tracking problem and even for vehicle counting problem as well. With the help of [Notebook](https://colab.research.google.com/drive/15pgDMnvXa-ZgGMeZkbbpg-gqa5Nttfi3?usp=sharing "link") (google colab) from [1], we can see the glamorous benefit providing by YOLO and Deep Sort.











# Reference
[1] kaylode, Vehicle Tracking using YOLOv5 + DeepSORT : https://github.com/kaylode/vehicle-counting .  
[2] Joseph and Ali Farhadi, YOLO9000: Better, Faster, Stronger.  
[3] Nicolai Wojke, Alex Bewley, and Dietrich Paulus, Simple Online and Realtime Tracking with a Deep Association Metric.  
[4] Jeremy Cohen, Computer Vision for Multi-Object Tracking — Live Example : https://www.thinkautonomous.ai/blog/?p=computer-vision-for-tracking .
