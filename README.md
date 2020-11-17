# Arduino-esp-detection-cam

# ESP-WHO
ESP-WHO is a face detection and recognition platform that is currently based on Espressif Systems' ESP32 chip.

# Overview
ESP-WHO supports development of face detection and recognition applications based around Espressif Systems' ESP32 chip in the most convenient way. With ESP-WHO, you can easily build up face detection- and recognition-featured applications, for instance:

* A coffee machine that brews coffee according to your taste preference;
* Home applicance that will shut off the electricity automatically when unsupervised children are operating them;
* And other more applications that suit your needs.
In general, the ESP-WHO features will be supported as shown below:

![overview](https://user-images.githubusercontent.com/70785525/99392425-07695280-291f-11eb-94d2-dcb2f559090f.jpg)


In ESP-WHO, Detection, Recognition and Image Utility are at the core of the platform.

* Image Utility offers fundamental image processing APIs.

* Detection takes images as input and give the position of face if there is a face. It is implemented with MTMN model, which refers to MTCNN and MobileNets.

* Recognition is to identify the particular person, and it needs the results of detection. It is implemented with MobileFace model.

* Optimization is mainly to increase the precision of the inference, and to accelerate the whole process. But also it might change the structure of the network, update the coefficients, refactor the code, etc.

Both input and output are flexible.

* Image sources could be input via camera. However, we don't provide many drivers right now, those for other camera modules will be released in the future.

* Results could be output and displayed through Command line, LCD or even website via Wi-Fi http service.

<h1> Quick Start with ESP-WHO
  
<h3> Hardware Preparation
  
  
To run ESP-WHO, you need to have a development board which integrates a ESP32 module that has sufficient GPIO pins and more than 4 MB external SPI RAM. Either ESP-WROVER-KIT or ESP-EYE can be a good choice as the test board.
