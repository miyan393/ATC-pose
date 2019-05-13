# 空中交通管制员动作检测

# ![image](https://github.com/miyan393/ATC-pose/blob/master/data/image/pose.gif)

## 描述

使用迁移学习方法检测空中交通管制员工作时的状态。[参考了Wayne Wong关于驾驶员的项目](https://github.com/omnigeeker/mlnd_distracted_driver_detection)

* 输入：一张640,480的RGB彩色图片
* 输出：十种状态的概率

动作列表：

* c0: 趴在桌子上睡觉
* c1: 仰头睡
* c2: 点头打盹
* c3: 和别人交谈
* c4: 正常指挥飞机
* c5: 左手托腮
* c6:右手托腮
* c7: 填写飞行进程单
* c8: 调频 
* c9: 右手扶额

## 数据

后续会公开在此，可以点这里:[百度云](https://pan.baidu.com/s/1pyEAlmqYI7wKQdd8AZ01_g)  密码 cn2b

## 代码说明，依次执行以下步骤：



### 1. 基准模型代码

 vgg16.ipynb

### 2. 单模型代码（后缀nde无数据增强，de数据增强）

inception_nde.ipydb 

inception_de.ipydb

Resnet50_nde.ipynb

Xception_nde.ipynb

### 3模型可视化示例

hotmap.ipynb

### 4. 模型融合代码

write_bottleneck_with_fine_tune.py

模型融合的思路有前期融合和后期融合

![](F:\ATC-pose\data\image\Fig2.png)

![](F:\ATC-pose\data\image\Fig3.png)

