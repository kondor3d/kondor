# Kondor


### 1. What is Kondor?
Kondor is an open source LCD (mask) resin 3D printer firmware started by 2 team members of Peopoly. Our goal is to create a flexible firmware that can run on different types of boards and is ideal for experimentation and customization.   

Here are the key features:
-    Drive 2 LCDs via SPI + HDMI (for improved performance over slower serial LCDs)
-    Easy to get and low-cost BOM 
-    Runs on inexpensive easy to acquire boards like Raspberry Pi 3B
-    Able to drive 4K displays
-    Core is C++
-    Ability to drive DLP (not at initial launch)

Launch Step:
-    Shared BOM and img for Pi3 for public testing while we clean up the code for release and take care of bugs until it is stable.
-    Then when the firmware is more stable and cleaned up, we will release the source code.

I also want to take this chance to share with you why we started this project: 
We want to give back to the open source community because we learned from projects like Marlin, Cura, and others.
We believe there should be more open source projects launched by Asian developers and we want to do our fair share.

While the project is launched by 2 guys from Asia, it belongs to the world. Join us to have some fun printing, testing and push the project forward.

### 2. How to use it?

**Pre-flight  5/12/2019**

The first stage is making sure testers have the Raspberry Pi 3B and can connect the slicer to the firmware.
Please use this Google doc for instructions for now:
https://docs.google.com/document/d/19AATh-Tu5reST9AKc0AZlHu6AHty7qCWfsSJ5gP3phQ/edit?usp=sharing
We will move the description to github once we have everything (code, links, suppliers) better tested.

**Todo List 5/14/2019**

Here are some ideas we need to do.

- Slicer
    - translate some Chinese to English
    - record/save the device IP address by default
    - hide/remove the autosupport option temporarily

- Pi Server Controler
    - add auto connect serial port 
    - test the gcode sender in the Pi
    - test z motor and tilt motor
    - report the Pi's IP address when the software starts
    - fix the virtual keyboard bug



