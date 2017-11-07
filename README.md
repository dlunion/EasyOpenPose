# EasyOpenPose
OpenPose的简单实现<br/>

# Usage:
这是一个linux caffe的实现版本<br/>
1.修改caffe的Makefile，CXXFLAGS += -std=c++11，使得支持c++11<br/>
2.把easyOpenPose.cpp复制到caffe的examples目录下<br/>
3.编译caffe即可<br/>

# 效果
![test.jpg](https://github.com/dlunion/EasyOpenPose/blob/master/test.jpg)
![test_openpose.jpg](https://github.com/dlunion/EasyOpenPose/blob/master/test_openpose.jpg)

# 使用方法
bin imagefile gpuid[-1] base_width[656] base_height[368] [deploy] [caffemodel]<br/>
<br/>
base_width和base_height是输入网络时候的宽高度，直接影响效果和消耗的时间<br/>

# 模型下载地址
[pose_iter_440000.caffemodel下载地址1-强烈建议](http://posefs1.perception.cs.cmu.edu/OpenPose/models/pose/coco/pose_iter_440000.caffemodel)<br/>
[pose_iter_440000.caffemodel下载地址2-强烈不建议，因为很费流量，很费钱](http://www.zifuture.com/fs/12.github/OpenPose/pose_iter_440000.caffemodel)<br/>

# Windows的实现
参照这里：[https://github.com/dlunion/OpenPose](https://github.com/dlunion/OpenPose)