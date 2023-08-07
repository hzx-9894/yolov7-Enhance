# yolov7-Enhance
Yolov7 Enhanced Edition , adding frame association.
Please replace **detect.py** and **general.py** in the original version of Yolov7.
The code is still being continuously expanded and has now implemented the following functions:
```
Algorithm for Frame-to-Frame Association Based on Object Tracking Principles, which employs the Hungarian algorithm to match detection boxes from the previous frame to all detection boxes in the next frame. Matched objects receive a confidence boost based on a certain coefficient, alleviating issues of object detection gaps and flickering caused by occlusion or blurriness.（coefficient could be changed by changing the hyper-parameters in **general.py Line 672**：coefficient, which is now 50%. ）
```
