# Hospital Indoor Object Detection (HIOD) dataset

A new dataset to facilitate the task of
object detection in the hospital. The proposed
hospital indoor object detection (HIOD) dataset has **4,417** annotated images covering **56** object
categories with **51,869** annotated object instances. The dataset is characterized by dense annotation, with an average of **11.7** objects and **6.8** object categories per image. Furthermore, a benchmark containing eight
state-of-the-art object detectors is created on the dataset. The benchmark indicates that the network
trained on the HIOD dataset can accurately detect and classify objects in hospitals. It is believed that
the dataset and benchmark provide valuable resources for researchers and practitioners to develop
computer-vision-based applications in hospitals.

# Data Preparation

![alt text](https://github.com/Wangmmstar/Hospital_Scene_Data/blob/main/readme/dataset_preparation.png?raw=true)

The preparation of the HIOD dataset consists of four steps: object
category selection, image collection, image selection, and image annotation.

# Example Data

![alt text](https://github.com/Wangmmstar/Hospital_Scene_Data/blob/main/readme/example_indoor_scenes.png?raw=true)

Image data were related to hospital
indoor environments, such as “intensive care unit,” “operating room,” “hospital consulting room,”
“hospital tour,” “hospital waiting room,” and more.

# Usage

Anyone who want to access the data folder could redirect to https://docs.google.com/forms/d/e/1FAIpQLSfI3UKkkIjvH1RGrN4BbCXCHLyRrtKt-jkJkMduw4K7ZXDNuA/viewform?usp=sf_link

The image folders contain the original jpeg files. The labels folers contains xml file of the object labels. Download both and combine them in one of the labeling softwares and then ready to be used. 

# The HIOD Dataset Details 

| Label        | Number of objects       | Number of images         |
| :---         |     :-----:               |     :-----:                | 
| sofa         | 1306              | 687    |
| chair        | 4777              | 1812     |
| foot board   | 606               | 490     |
| overbed table| 554              | 457     |
| hospital bed | 1581       | 1218     |
| staff        | 1852       | 965      |
| door handle  | 1659      | 1024     |
| table        | 1273      | 796     |
| bedside monitor| 2539       | 1353     |
| iv pole      | 1912      | 1166     |
| surgical light| 1138      | 641     |
| breathing tube| 448       | 406      |
| wheel chair  | 60       | 56     |
| patient      | 570      | 527     |
| drawer       | 303       | 258     |
| mouse        | 543      | 462     |
| computer     | 2160     | 1165    |
| bedrail      | 1787     | 813    |
| curtain      | 1309     | 778    |
| keyboard     | 730     | 616    |
| infusion pump| 377     | 281    |
| ventilator   | 327     | 294    |
| utility cart | 877     | 598    |
| panda baby warmer | 94 | 91    |
| visitor      | 196     | 152    |
| dispenser    | 2819     | 1474    |
| medical drawer| 814      | 599     |
| handle       | 5951     | 1382    |
| countertop   | 1463      | 1040    |
| cabinet      | 910     | 716    |
| waste_bin    | 1233     | 884    |
| faucet       | 717     | 567    |
| TV           | 747      | 597    |
| telephone    | 526     | 471    |
| syringe pump | 680     | 164    |
| light switch | 300      | 265    |
| elevator panel | 73      | 59    |
| counter      | 933      | 737    |
| medical waste container | 218  | 186    |
| push latch   | 330      | 237    |
|  operating bed | 549     | 523    |
| electrosurgical unit | 182 | 158    |
| sink         | 630     | 564    |
| restroom assist bar | 561 | 211    |
| incubator    | 101     | 95    |
| exam table   | 221     | 204    |
| bedside table | 290     | 249    |
| hallway assist bar| 1614 | 550    |
| sequential compression | 71 | 70    |
| toilet       | 191     | 180    |
| toilet handle| 114     | 110    |
| person       | 398     | 216    |
| press to open | 53     | 48    |
| surgical instrument | 87 | 58    |
| xray machine | 58      | 57    |
| xray bed     | 57     | 51    |


# Comparision with Other Datasets

The image shows the statistics and comparison with COCO, VOC, and OpenImages. The HIOD is found to be denser and more diverse than COCO,
VOC, and OpenImages with regard to the number of objects and categories on an image. Quantitatively, our HIOD dataset has an average and median of 11.7 and 10 objects on an image, respectively. In comparison, the average number of objects per image for COCO, VOC, and OpenImages are 7.3, 8.2, and 2.7, respectively. The median number of objects per image for
COCO, VOC, and OpenImages are 4, 2, and 4, respectively. On the other hand, our HIOD dataset
contains an average and median of 6.8 and 6 object categories per image, respectively, which are
both significantly greater than other benchmarks. The dense instances and diverse categories in the
HIOD dataset lay a solid foundation to build a robust object detector in hospitals.

![alt text](https://github.com/Wangmmstar/Hospital_Scene_Data/blob/main/readme/dataset_comparasion.svg?raw=true)


# Benchmark Performance

Eight state-of-the-art object detectors are trained on this dataset, which is randomly partitioned into a training set (70%), a validation set (10%), and a testing set (20%). The performance of these algorithms achieved on the testing set is summarized in Table below.

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


# Example Detection Results

The confusion matrices for YOLOv6-L and VFNet are shown in below figure. The diagonal value
represents the recall for the corresponding object category. 

![alt text](https://github.com/Wangmmstar/Hospital_Scene_Data/blob/main/readme/confusion_matrix.jpg?raw=true)

Some examples of detection results by YOLOv6-L network.

![alt text](https://github.com/Wangmmstar/Hospital_Scene_Data/blob/main/readme/yoloV6L_results.jpg?raw=true)
