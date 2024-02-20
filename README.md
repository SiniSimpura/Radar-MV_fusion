*Information about the used methods available at:*

# Radar-MV_fusion
A sensor fusion method that fuses radar detetions in geographic goordinates with video detections which locations are converted to geographic coordinates.
The video detections are done with YoloV4
There are two different ways of fusing radar data and video data, checkline-method and continuous data fusion.
For both methods, first step is to calculate velocities of detecions made with machine vision and acceleration for detection made with machine vision and radar sensor
# Checkline
If check-line method is used, data about vehicles that have crossed check-line is obtained from Checkline.ipynb
Checkline.ipynb is also used to assign radar IDs with Video IDs
To create fused data that has the trajectory from assigned radar IDs and vehicle type from assigned video IDs, Creating fused data.ipynb is used
# Continuous radar and video data fusion
If continuous data fusion is used, the first step is to create candidate matches between IDs with Creating candidate matches.ipynb
The assigned candidate matches are evaluated and final assignments are done with Assigning radarID to videoID.ipynb
To create fused data that has trajectory from assigned radar IDs and vehicle type from assigned video IDs, Creating fused data.ipynb is used

Detections for video are made with: https://github.com/theAIGuysCode/yolov4-deepsort
