Motion Detection
================
Motion detection on Hikey-960 allows user to detect motion at any remote location. It also sends images back to the user if a motion is detected with the help of mqtt

Hardware required:
------------------

  * Hikey 960
  * USB Video Camera
  * PC

Pre-requisites for Hikey960:
----------------------------

sudo apt-get update

sudo apt install python3-dev python3-pip

pip3 install imutils paho-mqtt

OpenCV on python3


Pre-requisites for PC/Laptop:
-----------------------------

sudo apt-get update

sudo apt install python3-dev python3-pip

pip3 install paho-mqtt

Steps for the Motion Detection Demo:
------------------------------------

Step 1 on PC/Laptop:

Run the mqtt_client_demo.py present in the pc folder

python3 mqtt_client_demo.py

Step 2 on Hikey-960:

Run the motion_detector.py

python3 motion_detector.py

As soon as you run the code the first frame is taken as frame of reference. As any motion is detected from the first frame of reference it captures an image and sends it back to the user through mqtt.
