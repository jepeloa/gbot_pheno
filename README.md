# Gbot-pheno

Complete documentation of the robotic platform for phenotyping soybean crops GBOT-PHENO

# Overview

The main goal of this project is provide a tool for phenotipyng soybeans crops at low cost using a robotic platform. We created this tool to estimate yield using IA algorithms.

We obtain yield measuring (at R8 stage) pods numbers, seeds number and weigth. The IA algorithms are performed using YOLOv5 (https://github.com/ultralytics/yolov5) for the counting and PixeLib (https://github.com/ayoolaolafenwa/PixelLib) for the segmentation (used to estimate weigth with the size of the pod)


![alt text](https://github.com/jepeloa/gbot_pheno/blob/main/brainpower_controller.png)
