# 空中交通管制员动作检测

# ![image](https://github.com/miyan393/ATC-pose/blob/master/data/image/pose.gif)

## 描述

使用迁移学习方法检测空中交通管制员工作时的状态。

* 输入：一张640,480的RGB彩色图片
* 输出：十种状态的概率

状态列表：

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

### 1. 数据集读取代码

 在keras-vgg16-visual-finetune.ipynb里

### 2. 基准模型代码

 keras-vgg16-visual-finetune.ipynb

### 3. 单模型代码

keras-resnet50-visual-finetune.ipynb

keras-inceptionV3-visual-finetune.ipynb

keras-xception-visual-finetune.ipynb

### 4. 模型融合代码

生成混合模型的输入；write_bottleneck_with_fine_tune.py

最终模型执行代码：main-finetune.ipynb



