# Safety at construction sites. Monitoring the availability of helmets for workers
## Formulation of the problem
The aim of this project is to detect the presence of helmets among workers at a construction site, with the goal of reducing accidents and ensuring safety compliance.
The primary quality metric will be mAP (mean average precision) since the task involves detecting three classes with imbalanced representation, making this metric the most comprehensive reflection of model quality.
## Dataset information and applied models
The images and annotations were taken from the website https://public.roboflow.com/object-detection/hard-hat-workers/1
In this study, we will explore solutions based on the following architectures: SSD 300 (https://github.com/sgrvinod/a-PyTorch-Tutorial-to-Object-Detection), YOLO(https://www.ultralytics.com/ru) to determine the best approach.
We have annotated data suitable for testing SSD300 (in the PASCAL VOC format), YOLOv8 (with txt annotations and yaml). Our dataset consists of 7041 images, with 5269 designated for training and 1766 for testing.
As we can see, we have 3 classes that we will be detecting, and based on the class, we will make decisions accordingly (penalties for the worker/ignoring, etc.).
