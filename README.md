# Gbot-pheno

Complete documentation of the robotic platform for phenotyping soybean crops GBOT-PHENO

# Overview

The main goal of this project is provide a tool for phenotipyng soybeans crops at low cost using a robotic platform. We created this tool to estimate yield using IA algorithms.

We obtain yield measuring (at R8 stage) pods numbers, seeds number and weigth. The IA algorithms are performed using YOLOv5 (https://github.com/ultralytics/yolov5) for the counting and PixeLib (https://github.com/ayoolaolafenwa/PixelLib) for the segmentation (used to estimate weigth with the size of the pod)

The platform are fully ROS (Robot Operating System) compatible, we used e-bike wheels and controllers to perform the traction system, and for the steering four indepedient actuators. The goal is to use parts that are easy to find in the market at low cost, here in Argentina we used www.mercadolibre.com.ar to buy.

# Desing challenges

The soybean (Glycine max (L.) Merr.) is an erect leguminous plant, up to 1 m high. A fast growing herbaceous annual, it is native to Asia but currently grown worldwide. Its tap-root can extend to 2 m deep in good soil conditions, with secondary roots exploring the upper 15-20 cm of the soil. Roots bear nodules resulting from Bradyrhizobium japonicum infection (in most cases). Leaves are trifoliate and leaflets are oval to lanceolate, mostly broad in commercial cultivars (Ecoport, 2010). The papilionaceous flowers are white, pink, purple or bluish, with a 5 to 7 mm long corolla (Giller et al., 2007). Fruits are two or three-seeded pods containing yellow, rounded seeds with a hilum colour ranging from yellow to black (Koivisto, 2006).





![alt_text](https://github.com/jepeloa/gbot_pheno/blob/main/soybean.jpg)






The rows in the soybeans fields are planted about 52 cm between plants, the heigth of the crop is about 1.3 m. The plant at R8 stage are dry with brow color, and without leafs. We use two rows to create a robot with 2 meter of width

![alt text](https://github.com/jepeloa/gbot_pheno/blob/main/stages_soybean.jpg)

The cameras of the robot must be capable to record videos into the rows, in a side view of the plants. With this position we can measure the entire plant.

![alt text](https://github.com/jepeloa/gbot_pheno/blob/main/soybean_pods.jpg)

# Platform Specification

- Adaptable width (variable in function of the size of the arc and the rows)

- Adaptable heigth dimensions (variable in function of the size of the arc)

- Modular, we can dissamsemble in easy way to transport

- Weigth of the individuals modules <50kg

- Robust and water proof (for rain, not for working under rain)

- 4x4 with traction control

- 4x individual steering

- Power On with one button (previous version have multiple swichs to start the system in specific sequence)


# image specification

- The camera must be take the entire plant from a distance bellow of 30 cm (the max distance from the lens of the camera to the plant).

- It's mandatory that the camera can be customizable, to change the exposition value to avoid the bhlur on the image.

- When the exposition are reduced to avoid the blhur, is necessary increase the ligth using led reflector light.

- The quality of the images must be enougth to detect grains and pods using IA models.

# CAD desing


![CAD](https://github.com/jepeloa/gbot_pheno/blob/main/gbot.stl)


# Block diagram

![alt text](https://github.com/jepeloa/gbot_pheno/blob/main/Schematic_gbot_v3.drawio.png)


# Wiring


![alt text](https://github.com/jepeloa/gbot_pheno/blob/main/wires_AC1.png)

![alt text](https://github.com/jepeloa/gbot_pheno/blob/main/wires_AC2.png)



