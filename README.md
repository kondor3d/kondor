# kondor


### 1. What't Kondor?
Kondor is an open source LCD (mask)3D printer firmware started by 2 team members of Peopoly. Our goal is to create a flexible firmware that can run on different types of boards and is ideal for experimentation and customization.   
Here are the key features:
-    Drive 2 LCDs via SPI + HDMI that improves performance
-    Easy to get and low-cost BOM 
-    Runs on PI3
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
-
Pre-flight 5/9/2019

The first stage is making sure testers have the Pi 3B and can connect the slicer to the firmware.
1.    Find a Pi 3B and an ethernet cable. Option (A 4” LCD connection via SPI) 
2.    Download  Firmware here and Slicer here
3.    Flash Pi 3B firmware using Win32image
4.    Install Slicer by extracting it from the zip file
5.    Power on Pi 3B and connect to the network via ethernet cable
6.    Making sure there is disk activity and if you have 
7.    Find out the IP address of the Pi3B via router(or the IP will show in the touchscreen when it first start)
8.    Enter Ip address to the slicer and hit connect


