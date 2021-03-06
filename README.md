# Introduction
* deployed on NVIDIA Jetson 
* detecting people
* tracking detected people
* counting in/out of people
![Alt Text](https://github.com/erichsiao1106/tensorRT-yolov4-MOT/blob/main/TRT_demo_480.gif)


### People detection
* using YOLOv4-tiny as object detection model
* model is trained in Darknet framework and converted to TensorRT inference engine with 608 x 608 input size

### Prepare to run
* a cam or a video with people to replace `crowd.mp4` in `main.py`
* modify the `main.py`: replace 'crowd.mp4' by your video
* modify the `main.py`: **point_1_y** and **point_2_y** to define a line to represent the boundary for in/out counting 
* download the engine file: 'yolov4_tiny_608.engine'

### Run python
* simply type: `python3 main.py
<br>
<img src="https://github.com/erichsiao1106/tensorRT-yolov4-MOT/blob/main/rt3.JPG" width="480" height="240" /><br>
<img src="https://github.com/erichsiao1106/tensorRT-yolov4-MOT/blob/main/trt2.JPG" width="480" height="240" /><br>
