简体中文 | [English](README.md)

# 医院室内目标检测数据集一个新的数据集，以方便目标检测

医院室内目标检测(HIOD)数据集有 * * 4,417 * * 注释图像覆盖 * * 56 * * 对象,具有 * * 51,869 * * 注释对象实例的类别。该数据集是拥有属性密集的注释，平均每张图片有 * * 11.7 * * 对象和 * * 6.8 * * * 对象类别。此外，包含8个在数据集上创建最先进的对象检测器。基准指示网络对 HIOD 数据集进行训练，可以准确地检测和分类医院中的物体数据集和基准提供了宝贵的资源，研究人员和从业人员开发计算机视觉在医院中的应用。

如需进一步描述，请参阅本文: [Object detection in hospital facilities: A comprehensive dataset and performance evaluation](https://www.sciencedirect.com/science/article/pii/S0952197623004074)
# Data Preparation

![alt text](https://github.com/Wangmmstar/Hospital_Scene_Data/blob/main/readme/dataset_preparation.png?raw=true)

HIOD 数据集的准备包括四个步骤: 对象类别选择、图像收集、图像选择和图像注释。

# 示例数据

![alt text](https://github.com/Wangmmstar/Hospital_Scene_Data/blob/main/readme/example_indoor_scenes.png?raw=true)

图像数据与医院有关;室内环境比如“重症监护室”“手术室” “医院咨询室” “医院之旅” “医院候诊室”等等。

# 用途

任何想要访问数据文件夹的人都可以重定向到 https://docs.google.com/forms/d/e/1FAIpQLSfI3UKkkIjvH1RGrN4BbCXCHLyRrtKt-jkJkMduw4K7ZXDNuA/viewform?usp=sf_link

图像文件夹包含原始 jpeg 文件。标签页面包含对象标签的 xml 文件。下载两者并将它们组合到一个标签软件中，然后准备使用。

# HIOD 数据集详细信息

| 标签 | 对象数量 | 图像数量 |
| :---         |     :-----:               |     :-----:                | 
| 沙发         | 1306              | 687    |
| 椅子        | 4777              | 1812     |
| 脚踏板   | 606               | 490     |
| 床上桌| 554              | 457     |
| 病床 | 1581       | 1218     |
| 员工        | 1852       | 965      |
| 门把手  | 1659      | 1024     |
| 桌子        | 1273      | 796     |
| 床边监护器| 2539       | 1353     |
| 静脉输液架     | 1912      | 1166     |
| 无影手术灯| 1138      | 641     |
| 呼吸管| 448       | 406      |
| 轮椅 | 60       | 56     |
| 病人      | 570      | 527     |
| 抽屉       | 303       | 258     |
| 鼠标        | 543      | 462     |
| 电脑     | 2160     | 1165    |
| 床栏杆      | 1787     | 813    |
| 窗帘      | 1309     | 778    |
| 键盘     | 730     | 616    |
| 输液泵| 377     | 281    |
| 呼吸机   | 327     | 294    |
| 小推车| 877     | 598    |
| 熊猫宝宝取暖器 | 94 | 91    |
| 访客      | 196     | 152    |
| 分配器    | 2819     | 1474    |
| 医用抽屉| 814      | 599     |
| 把手       | 5951     | 1382    |
| 工作台面   | 1463      | 1040    |
| 橱柜      | 910     | 716    |
| 垃圾桶    | 1233     | 884    |
| 水龙头       | 717     | 567    |
| 电视           | 747      | 597    |
| 电话    | 526     | 471    |
| 注射泵 | 680     | 164    |
| 电灯开关 | 300      | 265    |
| 电梯面板 | 73      | 59    |
| 柜台      | 933      | 737    |
| 医用废物容器 | 218  | 186    |
| 推杆式锁扣   | 330      | 237    |
|  手术床| 549     | 523    |
| 高频电刀| 182 | 158    |
| 水池         | 630     | 564    |
| 洗手间辅助架 | 561 | 211    |
| 保温箱    | 101     | 95    |
| 检查台  | 221     | 204    |
| 床边桌| 290     | 249    |
| 走廊辅助架| 1614 | 550    |
| 压力 | 71 | 70    |
| 马桶       | 191     | 180    |
| 马桶冲水按钮| 114     | 110    |
| 人       | 398     | 216    |
| 残疾人门开关 | 53     | 48    |
| 手术器械 | 87 | 58    |
| x光机器 | 58      | 57    |
| x光床    | 57     | 51    |


# 与其他数据集的比较


该图像显示了统计数据，并与 COCO、 VOC 和 OpenImages 进行了比较。HIOD 被发现比 COCO 更为密集和多样化, vOC 和 OpenImages 关于图像上的对象和类别的数量。在数量上，我们的 HIOD 数据集在一张图像上的平均值和中值分别为11.7和10个对象。相比之下，COCO、 VOC 和 OpenImages 每个图像的平均对象数分别为7.3、8.2和2.7。每个图像对象的中位数。COCO、 VOC 和 OpenImages 分别是4、2和4；每幅图像的平均和中位数分别为6.8和6个目标类别，HIOD 数据集为医院建立健壮的目标检测器奠定了坚实的基础。

![alt text](https://github.com/Wangmmstar/Hospital_Scene_Data/blob/main/readme/dataset_comparasion.svg?raw=true)


# Benchmark Performance

在这个数据集上训练了八个最先进的对象检测器，它被随机分为训练集(70%) ，验证集(10%)和测试集(20%)。下表总结了这些算法在测试集上实现的性能。

| **Algorithm** | **mAP** | **$\mathbf{AP}_{50}$** | **$\mathbf{AP}_{75}$** | **$\mathbf{AP}_{small}$** | **$\mathbf{AP}_{medium}$** | **$\mathbf{AP}_{large}$** |
| ----- | ----- | ----- | ----- | ----- | ----- | ----- |
| **One-stage**|
| YOLOv5-L | 0.473 |0.696 |0.501 |0.193 |0.402 |0.520 |
| YOLOX-L | 0.484 |0.708 |0.520 |0.178 |0.407 |0.554 |
| YOLOv6-L | 0.517 |0.737 |0.553 |0.211 |0.418 |0.597 |
| YOLOv7 | 0.506 |0.738 |0.545 |0.201 |0.432 |0.546 |
| **Two-stage**|
| Faster R-CNN | 0.403 |0.646 |0.438 |0.141 |0.327 |0.466 |
| Deformable DETR | 0.490 |0.741 |0.529 |0.209 |0.406 |0.565 |
| VFNet | 0.495 |0.711 |0.538 |0.200 |0.420 |0.567 |
| DyHead | 0.430 |0.645 |0.468 |0.145 |0.345 |0.507 |


# 检测结果范例

YOLOv6-L 和 VFNet 的混淆矩阵如下图所示 表示对相应对象类别的召回。

![alt text](https://github.com/Wangmmstar/Hospital_Scene_Data/blob/main/readme/confusion_matrix.jpg?raw=true)

Some examples of detection results by YOLOv6-L network.

![alt text](https://github.com/Wangmmstar/Hospital_Scene_Data/blob/main/readme/yoloV6L_results.jpg?raw=true)


## 快速开始

<details>
<summary> 安装</summary>


```shell
git clone https://github.com/Wangmmstar/Hospital_Scene_Data.git
pip install -r requirements.txt
```

</details>

<details open>
<summary> 在自定义数据集上微调模型 </summary>

单卡

```shell
# P5 models
python tools/train.py --batch 32 --conf configs/yolov6s_finetune.py --data data/hiod.yaml --fuse_ab --device 0
# P6 models
python tools/train.py --batch 32 --conf configs/yolov6s6_finetune.py --data data/hiod.yaml --img 1280 --device 0
```

多卡 （我们推荐使用 DDP 模式）

```shell
# P5 models
python -m torch.distributed.launch --nproc_per_node 8 tools/train.py --batch 256 --conf configs/yolov6s_finetune.py --data data/hiod.yaml --fuse_ab --device 0,1,2,3,4,5,6,7
# P6 models
python -m torch.distributed.launch --nproc_per_node 8 tools/train.py --batch 128 --conf configs/yolov6s6_finetune.py --data data/hiod.yaml --img 1280 --device 0,1,2,3,4,5,6,7
```
- fuse_ab: 增加anchor-based预测分支并使用联合锚点训练模式 (P6模型暂不支持此功能)
- conf: 配置文件路径，里面包含网络结构、优化器配置、超参数信息。如果您是在自己的数据集训练，我们推荐您使用yolov6n/s/m/l_finetune.py配置文件；
- data: 数据集配置文件 hiod.yaml
- 确保您的数据集按照下面这种格式来组织；
```
├── dataset
│   ├── hiod
│      ├── images
│      │   ├── train
│      │   └── val
│      ├── labels
│      │   ├── train
│      │   ├── val
```

YOLOv6 支持不同的输入分辨率模式，详情请参见 [如何设置输入大小](./docs/About_training_size_cn.md).

</details>

<details>
<summary>恢复训练</summary>


如果您的训练进程中断了，您可以这样恢复先前的训练进程。
```
# 单卡训练
python tools/train.py --resume

# 多卡训练
python -m torch.distributed.launch --nproc_per_node 8 tools/train.py --resume
```
上面的命令将自动在 YOLOv6 目录中找到最新保存的模型，然后恢复训练。

您也可以通过 `--resume` 参数指定要恢复的模型路径
```
# 记得把 /path/to/your/checkpoint/path  替换为您要恢复训练的模型权重路径
--resume /path/to/your/checkpoint/path
```
这将从您提供的模型路径恢复训练。

</details>


<details>
<summary> 评估</summary>
在 HIOD 数据集上复现我们的结果（输入分辨率 640x640 或 1280x1280）

```shell
# P5 models
python tools/eval.py --data data/hiod.yaml --batch 32 --weights yolov6s.pt --task val --reproduce_640_eval
# P6 models
python tools/eval.py --data data/hiod.yaml --batch 32 --weights yolov6s6.pt --task val --reproduce_640_eval --img 1280
```
- verbose: 如果要打印每一类的精度信息，请设置为 True；
- do_coco_metric: 设置 True / False 来打开或关闭 pycocotools 的评估；
- do_pr_metric: 设置 True / False 来显示或不显示精度和召回的指标；
- config-file: 指定一个包含所有评估参数的配置文件，例如 [yolov6n_with_eval_params.py](configs/experiment/yolov6n_with_eval_params.py)
</details>


<details>
<summary>推理</summary>

首先，从 [release页面](https://github.com/meituan/YOLOv6/releases/tag/0.3.0)  下载一个训练好的模型权重文件，或选择您自己训练的模型；

然后，通过 `tools/infer.py`文件进行推理。

```shell
# P5 models
python tools/infer.py --weights yolov6s.pt --source img.jpg / imgdir / video.mp4
# P6 models
python tools/infer.py --weights yolov6s6.pt --img 1280 1280 --source img.jpg / imgdir / video.mp4
```
如果您想使用本地摄像头或者网络摄像头，您可以运行:
```shell
# P5 models
python tools/infer.py --weights yolov6s.pt --webcam --webcam-addr 0
# P6 models
python tools/infer.py --weights yolov6s6.pt --img 1280 1280 --webcam --webcam-addr 0
```
`webcam-addr` 可以是本地摄像头的 ID，或者是 RTSP 地址。


 * [YOLOv6 web demo](https://huggingface.co/spaces/nateraw/yolov6) on [Huggingface Spaces](https://huggingface.co/spaces) with [Gradio](https://github.com/gradio-app/gradio). [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/nateraw/yolov6)
 * 教程: [如何用 YOLOv6 训练自己的数据集](https://blog.roboflow.com/how-to-train-yolov6-on-a-custom-dataset/) <a href="https://colab.research.google.com/drive/1YnbqOinBZV-c9I7fk_UL6acgnnmkXDMM"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
 * YOLOv6 在 Google Colab 上的推理 Demo [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mahdilamb/YOLOv6/blob/main/inference.ipynb)
</details>


