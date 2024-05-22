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

# 代码测试数据集

这里 Yolo V6及其变体被用来测试 HIOD 数据集的质量。


## YOLOv6

官方论文:
- [YOLOv6 v3.0: A Full-Scale Reloading](https://arxiv.org/abs/2301.05586) 🔥
- [YOLOv6: A Single-Stage Object Detection Framework for Industrial Applications](https://arxiv.org/abs/2209.02976)

<p align="center">
  <img src="assets/speed_comparision_v3.png" align="middle" width = "1000" />
</p>


## 更新日志
- [2023.04.28] 发布 移动端轻量级模型 [YOLOv6Lite](configs/yolov6_lite/README.md). ⭐️ [移动端模型指标](#移动端模型指标)
- [2023.03.10] 发布 [YOLOv6-Face](https://github.com/meituan/YOLOv6/tree/yolov6-face). 🔥 [人脸检测模型指标](https://github.com/meituan/YOLOv6/blob/yolov6-face/README_cn.md#widerface-%E6%A8%A1%E5%9E%8B%E6%8C%87%E6%A0%87)
- [2023.03.02] 更新 [基础版模型](configs/base/README_cn.md) 到 3.0 版本
- [2023.01.06] 发布大分辨率 P6 模型以及对 P5 模型做了全面的升级 ⭐️ [模型指标](#模型指标)
- [2022.11.04] 发布 [基础版模型](configs/base/README_cn.md) 简化训练部署流程
- [2022.09.06] 定制化的模型量化加速方法 🚀 [量化教程](./tools/qat/README.md)
- [2022.09.05] 发布 M/L 模型，并且进一步提高了 N/T/S 模型的性能
- [2022.06.23] 发布 N/T/S v1.0 版本模型

## 模型指标
| 模型                                                       | 输入尺寸 | mAP<sup>val<br/>0.5:0.95              | 速度<sup>T4<br/>trt fp16 b1 <br/>(fps) | 速度<sup>T4<br/>trt fp16 b32 <br/>(fps) | Params<br/><sup> (M) | FLOPs<br/><sup> (G) |
| :----------------------------------------------------------- | ---- | :------------------------------------ | --------------------------------------- | ---------------------------------------- | -------------------- | ------------------- |
| [**YOLOv6-N**](https://github.com/meituan/YOLOv6/releases/download/0.3.0/yolov6n.pt) | 640  | 37.5                     | 779                                     | 1187                                     | 4.7                  | 11.4                |
| [**YOLOv6-S**](https://github.com/meituan/YOLOv6/releases/download/0.3.0/yolov6s.pt) | 640  | 45.0                     | 339                                     | 484                                      | 18.5                 | 45.3                |
| [**YOLOv6-M**](https://github.com/meituan/YOLOv6/releases/download/0.3.0/yolov6m.pt) | 640  | 50.0                     | 175                                     | 226                                      | 34.9                 | 85.8                |
| [**YOLOv6-L**](https://github.com/meituan/YOLOv6/releases/download/0.3.0/yolov6l.pt) | 640  | 52.8                     | 98                                      | 116                                      | 59.6                 | 150.7               |
|                              |                               |                                |                    |                        |
| [**YOLOv6-N6**](https://github.com/meituan/YOLOv6/releases/download/0.3.0/yolov6n6.pt) | 1280 | 44.9                     | 228                                     | 281                                      | 10.4                 | 49.8                |
| [**YOLOv6-S6**](https://github.com/meituan/YOLOv6/releases/download/0.3.0/yolov6s6.pt) | 1280 | 50.3                     | 98                                      | 108                                      | 41.4                 | 198.0               |
| [**YOLOv6-M6**](https://github.com/meituan/YOLOv6/releases/download/0.3.0/yolov6m6.pt) | 1280 | 55.2                     | 47                                      | 55                                       | 79.6                 | 379.5               |
| [**YOLOv6-L6**](https://github.com/meituan/YOLOv6/releases/download/0.3.0/yolov6l6.pt) | 1280 | 57.2                     | 26                                      | 29                                       | 140.4                | 673.4               |

<details>
<summary>表格笔记</summary>

- 除了 YOLOv6-N6/S6 模型是训练了300轮的结果，其余模型均为自蒸馏训练之后的结果；
- mAP 和速度指标是在 [COCO val2017](https://cocodataset.org/#download)  数据集上评估的，P5模型输入分辨率为 640×640，P6模型输入分辨率为 1280×1280；
- 速度是在 T4 上测试的，TensorRT 版本为 7.2；
- 复现 YOLOv6 的速度指标，请查看 [速度测试](./docs/Test_speed.md) 教程；
- YOLOv6 的参数和计算量是在推理模式下计算的；
</details>

<details>
<summary>旧版模型</summary>

| 模型                                                       | 输入尺寸 | mAP<sup>val<br/>0.5:0.95              | 速度<sup>T4<br/>trt fp16 b1 <br/>(fps) | 速度<sup>T4<br/>trt fp16 b32 <br/>(fps) | Params<br/><sup> (M) | FLOPs<br/><sup> (G) |
| :----------------------------------------------------------- | ---- | :------------------------------------ | --------------------------------------- | ---------------------------------------- | -------------------- | ------------------- |
| [**YOLOv6-N**](https://github.com/meituan/YOLOv6/releases/download/0.2.0/yolov6n.pt) | 640  | 35.9<sup>300e</sup><br/>36.3<sup>400e | 802                                     | 1234                                     | 4.3                  | 11.1                |
| [**YOLOv6-T**](https://github.com/meituan/YOLOv6/releases/download/0.2.0/yolov6t.pt) | 640  | 40.3<sup>300e</sup><br/>41.1<sup>400e | 449                                     | 659                                      | 15.0                 | 36.7                |
| [**YOLOv6-S**](https://github.com/meituan/YOLOv6/releases/download/0.2.0/yolov6s.pt) | 640  | 43.5<sup>300e</sup><br/>43.8<sup>400e | 358                                     | 495                                      | 17.2                 | 44.2                |
| [**YOLOv6-M**](https://github.com/meituan/YOLOv6/releases/download/0.2.0/yolov6m.pt) | 640  | 49.5                                  | 179                                     | 233                                      | 34.3                 | 82.2                |
| [**YOLOv6-L-ReLU**](https://github.com/meituan/YOLOv6/releases/download/0.2.0/yolov6l_relu.pt) | 640  | 51.7                                  | 113                                     | 149                                      | 58.5                 | 144.0               |
| [**YOLOv6-L**](https://github.com/meituan/YOLOv6/releases/download/0.2.0/yolov6l.pt) | 640  | 52.5                                  | 98                                      | 121                                      | 58.5                 | 144.0               |
- 速度是在 T4 上测试的，TensorRT 版本为 7.2；

### 量化模型

| 模型                 | 输入尺寸 | 精度 | mAP<sup>val<br/>0.5:0.95 | 速度<sup>T4<br/>trt b1 <br/>(fps) | 速度<sup>T4<br/>trt b32 <br/>(fps) |
| :-------------------- | ---- | --------- | :----------------------- | ---------------------------------- | ----------------------------------- |
| **YOLOv6-N RepOpt** | 640  | INT8      | 34.8                     | 1114                               | 1828                                |
| **YOLOv6-N**        | 640  | FP16      | 35.9                     | 802                                | 1234                                |
| **YOLOv6-T RepOpt** | 640  | INT8      | 39.8                     | 741                                | 1167                                |
| **YOLOv6-T**        | 640  | FP16      | 40.3                     | 449                                | 659                                 |
| **YOLOv6-S RepOpt** | 640  | INT8      | 43.3                     | 619                                | 924                                 |
| **YOLOv6-S**        | 640  | FP16      | 43.5                     | 377                                | 541                                 |

- 速度是在 T4 上测试的，TensorRT 版本为 8.4；
- 精度是在训练 300 epoch 的模型上测试的；

</details>

## 移动端模型指标

| 模型 | 输入尺寸 | mAP<sup>val<br/>0.5:0.95 | sm8350<br/><sup>(ms) | mt6853<br/><sup>(ms) | sdm660<br/><sup>(ms) |Params<br/><sup> (M) |   FLOPs<br/><sup> (G) |
| :----------------------------------------------------------- | ---- | -------------------- | -------------------- | -------------------- | -------------------- | -------------------- | -------------------- |
| [**YOLOv6Lite-S**](https://github.com/meituan/YOLOv6/releases/download/0.4.0/yolov6lite_s.pt) | 320*320 | 22.4                     | 7.99                     | 11.99                     | 41.86                     | 0.55                     | 0.56                     |
| [**YOLOv6Lite-M**](https://github.com/meituan/YOLOv6/releases/download/0.4.0/yolov6lite_m.pt) | 320*320 | 25.1                     | 9.08                     | 13.27                     | 47.95                     | 0.79                     | 0.67                     |
| [**YOLOv6Lite-L**](https://github.com/meituan/YOLOv6/releases/download/0.4.0/yolov6lite_l.pt) | 320*320 | 28.0                     | 11.37                     | 16.20                     | 61.40                     | 1.09                     | 0.87                     |
| [**YOLOv6Lite-L**](https://github.com/meituan/YOLOv6/releases/download/0.4.0/yolov6lite_l.pt) | 320*192 | 25.0                     | 7.02                     | 9.66                     | 36.13                     | 1.09                     | 0.52                     |
| [**YOLOv6Lite-L**](https://github.com/meituan/YOLOv6/releases/download/0.4.0/yolov6lite_l.pt) | 224*128 | 18.9                     | 3.63                     | 4.99                     | 17.76                     | 1.09                     | 0.24                     |

<details>
<summary>表格笔记</summary>

- 从模型尺寸和输入图片比例两种角度，在构建了移动端系列模型，方便不同场景下的灵活应用。
- 所有权重都经过 400 个 epoch 的训练，并且没有使用蒸馏技术。
-  mAP 和速度指标是在 COCO val2017 数据集上评估的，输入分辨率为表格中对应展示的。
- 使用 MNN 2.3.0 AArch64 进行速度测试。测速时，采用2个线程，并开启arm82加速，推理预热10次，循环100次。
- 高通888(sm8350)、天玑720(mt6853)和高通660(sdm660)分别对应高中低端不同性能的芯片，可以作为不同芯片下机型能力的参考。
- [NCNN 速度测试](./docs/Test_NCNN_speed.md)教程可以帮助展示及复现 YOLOv6Lite 的 NCNN 速度结果。

</details>

## 快速开始

<details>
<summary> 安装</summary>


```shell
git clone https://github.com/meituan/YOLOv6
cd YOLOv6
pip install -r requirements.txt
```
</details>

<details>
<summary> 在 COCO 数据集上复现我们的结果</summary>

请参考教程 [训练 COCO 数据集](./docs/Train_coco_data.md).

</details>

<details open>
<summary> 在自定义数据集上微调模型 </summary>

单卡

```shell
# P5 models
python tools/train.py --batch 32 --conf configs/yolov6s_finetune.py --data data/dataset.yaml --fuse_ab --device 0
# P6 models
python tools/train.py --batch 32 --conf configs/yolov6s6_finetune.py --data data/dataset.yaml --img 1280 --device 0
```

多卡 （我们推荐使用 DDP 模式）

```shell
# P5 models
python -m torch.distributed.launch --nproc_per_node 8 tools/train.py --batch 256 --conf configs/yolov6s_finetune.py --data data/dataset.yaml --fuse_ab --device 0,1,2,3,4,5,6,7
# P6 models
python -m torch.distributed.launch --nproc_per_node 8 tools/train.py --batch 128 --conf configs/yolov6s6_finetune.py --data data/dataset.yaml --img 1280 --device 0,1,2,3,4,5,6,7
```
- fuse_ab: 增加anchor-based预测分支并使用联合锚点训练模式 (P6模型暂不支持此功能)
- conf: 配置文件路径，里面包含网络结构、优化器配置、超参数信息。如果您是在自己的数据集训练，我们推荐您使用yolov6n/s/m/l_finetune.py配置文件；
- data: 数据集配置文件，以 COCO 数据集为例，您可以在 [COCO](http://cocodataset.org) 下载数据, 在这里下载 [YOLO 格式标签](https://github.com/meituan/YOLOv6/releases/download/0.1.0/coco2017labels.zip)；
- 确保您的数据集按照下面这种格式来组织；
```
├── coco
│   ├── annotations
│   │   ├── instances_train2017.json
│   │   └── instances_val2017.json
│   ├── images
│   │   ├── train2017
│   │   └── val2017
│   ├── labels
│   │   ├── train2017
│   │   ├── val2017
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
在 COCO val2017 数据集上复现我们的结果（输入分辨率 640x640 或 1280x1280）

```shell
# P5 models
python tools/eval.py --data data/coco.yaml --batch 32 --weights yolov6s.pt --task val --reproduce_640_eval
# P6 models
python tools/eval.py --data data/coco.yaml --batch 32 --weights yolov6s6.pt --task val --reproduce_640_eval --img 1280
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
</details>

<details>
<summary> 部署 </summary>

*  [ONNX](./deploy/ONNX)
*  [OpenCV Python/C++](./deploy/ONNX/OpenCV)
*  [OpenVINO](./deploy/OpenVINO)
*  [TensorRT](./deploy/TensorRT)
*  [NCNN](./deploy/NCNN)
*  [Android](./deploy/NCNN/Android)
</details>

<details open>
<summary> 教程 </summary>

*  [用户手册（中文版）](https://yolov6-docs.readthedocs.io/zh_CN/latest/)
*  [训练 COCO 数据集](./docs/Train_coco_data.md)
*  [训练自定义数据集](./docs/Train_custom_data.md)
*  [测速](./docs/Test_speed.md)
*  [ YOLOv6 量化教程](./docs/Tutorial%20of%20Quantization.md)
</details>


<details>
<summary> 第三方资源 </summary>

 * YOLOv6 NCNN Android app demo: [ncnn-android-yolov6](https://github.com/FeiGeChuanShu/ncnn-android-yolov6) from [FeiGeChuanShu](https://github.com/FeiGeChuanShu)
 * YOLOv6 ONNXRuntime/MNN/TNN C++: [YOLOv6-ORT](https://github.com/DefTruth/lite.ai.toolkit/blob/main/lite/ort/cv/yolov6.cpp), [YOLOv6-MNN](https://github.com/DefTruth/lite.ai.toolkit/blob/main/lite/mnn/cv/mnn_yolov6.cpp) and [YOLOv6-TNN](https://github.com/DefTruth/lite.ai.toolkit/blob/main/lite/tnn/cv/tnn_yolov6.cpp) from [DefTruth](https://github.com/DefTruth)
 * YOLOv6 TensorRT Python: [yolov6-tensorrt-python](https://github.com/Linaom1214/TensorRT-For-YOLO-Series) from [Linaom1214](https://github.com/Linaom1214)
 * YOLOv6 TensorRT Windows C++: [yolort](https://github.com/zhiqwang/yolov5-rt-stack/tree/main/deployment/tensorrt-yolov6) from [Wei Zeng](https://github.com/Wulingtian)
 * [YOLOv6 web demo](https://huggingface.co/spaces/nateraw/yolov6) on [Huggingface Spaces](https://huggingface.co/spaces) with [Gradio](https://github.com/gradio-app/gradio). [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/nateraw/yolov6)
 * 教程: [如何用 YOLOv6 训练自己的数据集](https://blog.roboflow.com/how-to-train-yolov6-on-a-custom-dataset/) <a href="https://colab.research.google.com/drive/1YnbqOinBZV-c9I7fk_UL6acgnnmkXDMM"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
 * YOLOv6 在 Google Colab 上的推理 Demo [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mahdilamb/YOLOv6/blob/main/inference.ipynb)
</details>


