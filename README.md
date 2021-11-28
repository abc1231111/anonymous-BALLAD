# anonymous-BALLAD
This is the anonymous code version of *A Simple Long-Tailed Recognition Baseline via Vision-Language Model* for CVPR2022 review.

![image](https://github.com/abc1231111/anonymous-BALLAD/blob/main/figure.PNG)

## Requirements
* Python3
* Pytorch(1.7.1 recommended)
* yaml

## Datasets
* ImageNet_LT
* Places_LT

Download the [ImageNet_2014](http://image-net.org/index) and [Places_365](http://places2.csail.mit.edu/download.html).

Modify the data_root in [main.py](main.py) to refer to your own dataset path.

## Training

#### Phase A
```
python main.py --cfg ./config/ImageNet_LT/clip_A_rn50.yaml
```

#### Phase B
```
python main.py --cfg ./config/ImageNet_LT/clip_B_rn50.yaml
```

## Testing
```
python main.py --cfg ./config/ImageNet_LT/test.yaml --test
```
