# Speed estimation with Yolov5 + StrongSORT





<div align="center">
<p>
<img src="trackers/strong_sort/results/speed.PNG" width = 700 height = 500/> 
</p>
<br>
</div>

## Before you run

1. Clone the repository recursively:

`git clone --recurse-submodules https://github.com/cakiryusuff/Car-Speed-Estimation.git`

If you already cloned and forgot to use `--recurse-submodules` you can run `git submodule update --init`

2. Make sure that you fulfill all the requirements: Python 3.8 or later with all [requirements.txt](https://github.com/mikel-brostrom/Yolov5_DeepSort_Pytorch/blob/master/requirements.txt) dependencies installed, including torch>=1.7. To install, run:

`pip install -r requirements.txt`

## Filter tracked classes

By default the tracker tracks all MS COCO classes.

If you only want to track cars

```bash
python Speed-Estimation.py --classes 2 #only cars
```

[Here](https://tech.amikelive.com/node-718/what-object-categories-labels-are-in-coco-dataset/) is a list of all the possible objects that a Yolov5 model trained on MS COCO can detect. Notice that the indexing for the classes in this repo starts at zero.


## Execute the Speed-Estimation.py

```bash
python Speed-Estimation.py --source traffic_Trim.mp4
```
