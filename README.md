# Real Time Deep Sort with PyTorch

## Introduction
This code is modified based on the code from ZQPei's code. ZXQPei's code is not suitable for the real-time re-id task. The network usually can only deal with 7 frames per second. Most cameras have a higher FPS. In this case, it will fill up the buffer area, which will cause the real-time video not consistent. I use multi-processing to solve the issue. Process A is dealing with the network and shows real-time videos. Process B is keeping cleaning the buffer area to keep the real-time video consistent.
## Run Demo
```
python multi_processing_run.py [YOUR_CAMERA_ADDRESS]
```


## References
- paper: [Simple Online and Realtime Tracking with a Deep Association Metric](https://arxiv.org/abs/1703.07402)

- code: [nwojke/deep_sort](https://github.com/nwojke/deep_sort)

- paper: [YOLOv3](https://pjreddie.com/media/files/papers/YOLOv3.pdf)

- code: [Joseph Redmon/yolov3](https://pjreddie.com/darknet/yolo/)

- code:  [ZQPei/deep_sort_pytorch](https://github.com/ZQPei/deep_sort_pytorch)



