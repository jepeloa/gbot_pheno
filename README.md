# Gbot-pheno

Complete documentation of the robotic platform for phenotyping soybean crops GBOT-PHENO

# Overview

The main goal of this project is provide a tool for phenotipyng soybeans crops at low cost using a robotic platform. We created this tool to estimate yield using IA algorithms.

We obtain yield measuring (at R8 stage) pods numbers, seeds number and weigth. The IA algorithms are performed using YOLOv5 (https://github.com/ultralytics/yolov5) for the counting and PixeLib (https://github.com/ayoolaolafenwa/PixelLib) for the segmentation (used to estimate weigth with the size of the pod)

The platform are fully ROS (Robot Operating System) compatible, we used e-bike wheels and controllers to perform the traction system, and for the steering four indepedient actuators. The goal is to use parts that are easy to find in the market at low cost, here in Argentina we used www.mercadolibre.com.ar to buy.

# Desing challenges

The soybean (Glycine max (L.) Merr.) is an erect leguminous plant, up to 1 m high. A fast growing herbaceous annual, it is native to Asia but currently grown worldwide. Its tap-root can extend to 2 m deep in good soil conditions, with secondary roots exploring the upper 15-20 cm of the soil. Roots bear nodules resulting from Bradyrhizobium japonicum infection (in most cases). Leaves are trifoliate and leaflets are oval to lanceolate, mostly broad in commercial cultivars (Ecoport, 2010). The papilionaceous flowers are white, pink, purple or bluish, with a 5 to 7 mm long corolla (Giller et al., 2007). Fruits are two or three-seeded pods containing yellow, rounded seeds with a hilum colour ranging from yellow to black (Koivisto, 2006).





![alt text](https://github.com/jepeloa/gbot_pheno/blob/main/soybean.jpg)






The rows in the soybeans fields are planted about 52 cm between plants, the heigth of the crop is about 1.3 m. The plant at R8 stage are dry with brow color, and without leafs. We use two rows to create a robot with 2 meter of width

![alt text](https://github.com/jepeloa/gbot_pheno/blob/main/stages_soybean.jpg)

the specification are:

-2 meter of width (variable in function of the size of the arc)

-Modular, we can dissamsemble in easy way to transport


