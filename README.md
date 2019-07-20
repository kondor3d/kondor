![img](./doc-img/kondor-logo.png)

---
# kondor
---
### 1. What't Kondor?
Kondor is an open source LCD (mask)3D printer firmware started by 2 team members of Peopoly. Our goal is to create a flexible firmware that can run on different types of boards and is ideal for experimentation and customization.   
Here are the key features:
-    Drive 2 LCDs via SPI + HDMI for improves performance over UART
-    Easy to get and low-cost BOM 
-    Runs on inexpensive easy to acquire boards like Pi 3B
-    Able to do 4K
-    Core is C++
-    Ability to drive DLP (not at initial launch)

Launch Step:
-    Shared BOM and img for Pi3 for public testing while we clean up the codes for release and take care bugs as needed to it is stable. 
-    Then when the firmware is more stable and cleaned up, we will release codes 

I also want to take this chance to share with you why we started this project: 
We want to give back to the open source community because we learned from projects like Marlin, Cura, and others.
We believe there should be more open source projects launched by Asian developers and we want to do our fair share.

While the project is launched by2 guys from Asia, it belongs to the world. Join us to have some fun printing, testing and push the project forward.

### 2.How to use it?

**Pre-flight  5/12/2019**

The first stage is making sure testers have the Pi 3B and can connect the slicer to the firmware.
please use this Google doc for instructions for now:
https://docs.google.com/document/d/19AATh-Tu5reST9AKc0AZlHu6AHty7qCWfsSJ5gP3phQ/edit?usp=sharing
We will move the descrition to github once we have the firmware more tested out. 

**Todo List 5/14/2019**

Here's some idear we need to do.

- Slicer
    - [ ] translate some chinese to english
    - [ ] record the device ip by default
    - [ ] hide/remove the autosupport temporarily

- Pi Server Controler
    - [x] add auto connect serial port 
    - [x] test the gcode sender in the pi, test z motor and titlt motor
    - [x] report the pi's IP when the software start
    - [ ] fix the virtual keyboard bug



### Kondor Code Refactoring

Kondor最初的版本是基于DLP的控制开发的，我们在使用的过程中，发现有很多地方在LCD打印机上不太使用，尤其是界面放在一个3.5寸的屏幕上时。
根据我们目前的用户的反馈，Kondor目前分为如下几个模块:

- Kondor Slicer, 用于切片，添加支撑，最简单的传输文件
- Kondor Device Manager, 用于管理Kondor设备, 基本功能包括: 传输打印文件，发现局域网的LCD打印机
- Kondor Pi Image , 适用于Raspberry 3b的一个镜像文件，实现脱机打印等打印功能
- Kondor Marlin, 适用于基于2560 Ramp1.4主板的一个Marlin固件，用于控制电机和LCD的灯泡等

上述四个为当前重构的内容。 如下是基本的UI界面:

#### 1. Device Manager
![图片](./doc-img/2019-7-20/kondor-2.jpg)

![图片](./doc-img/2019-7-20/kondor-1.jpg)


#### 2. Kondor Pi Image

![图片](./doc-img/2019-7-20/kondor-3.jpg)

![图片](./doc-img/2019-7-20/kondor-4.jpg)

![图片](./doc-img/2019-7-20/kondor-5.jpg)

![图片](./doc-img/2019-7-20/kondor-6.jpg)







