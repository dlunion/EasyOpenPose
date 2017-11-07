# EasyOpenPose
OpenPose的简单实现

# Usage:
这是一个linux caffe的实现版本
* 1.修改caffe的Makefile，CXXFLAGS += -std=c++11，使得支持c++11
* 2.新建目录caffe/examples/EasyOpenPose，并把easyOpenPose.cpp复制进去
* 3.编译caffe即可

# 效果
![test.jpg](https://github.com/dlunion/EasyOpenPose/blob/master/test.jpg)
![test_openpose.jpg](https://github.com/dlunion/EasyOpenPose/blob/master/test_openpose.jpg)

# 使用方法
base_width和base_height是输入网络时候的宽高度，直接影响效果和消耗的时间
>bin imagefile gpuid[-1] base_width[656] base_height[368] [deploy] [caffemodel]

输出结果
```Bash
../../.build_release/examples/openpose/main.bin test.jpg 3 500 500

image: test.jpg
deploy: pose_deploy_linevec.prototxt
caffemodel: pose_iter_440000.caffemodel
compute device GPU(3).
base size = width 500 x height 500
forward fee: 634.756 ms
finish. save result to 'test_openpose.jpg', people: 3
```

# 模型下载地址
[pose_iter_440000.caffemodel下载地址1-强烈建议](http://posefs1.perception.cs.cmu.edu/OpenPose/models/pose/coco/pose_iter_440000.caffemodel)<br/>
[pose_iter_440000.caffemodel下载地址2-强烈不建议，因为很费流量，很费钱](http://www.zifuture.com/fs/12.github/OpenPose/pose_iter_440000.caffemodel)

# Windows的实现
[https://github.com/dlunion/OpenPose](https://github.com/dlunion/OpenPose)

# 引用
https://github.com/CMU-Perceptual-Computing-Lab/openpose
