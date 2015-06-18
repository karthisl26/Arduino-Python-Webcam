# Arduino-Python-Webcam

Ultrasonic Functions

  ultrasonic sensor is non-contact distance measurement module, which is also compatible with electronic brick.It’s designed for easy modular project usage with industrial performance. 

Features

 Detecting range: 3cm-4m
 
 Best in 30 degree angle
 
 Electronic brick compatible interface
 
 5VDC power supply
 
 Breadboard friendly
 
 Dual transducer
 
 Arduino library ready

Installation
-------------

Detects if any intruder nears your computer with the help of Ultrasonic sensor and captures their image immediately
with the help of your Webcam.

<img src="ultrasonic_sensor_bb.png" alt="Arduino Sketch Schema" style="width: 500px; height: 400px"/>

### Setup

* Install the required python libraries from requirement.txt file

        sudo pip install -r requirements.txt

* Connect your Arduino board over USB and find the name of the port it is connected to (Usually this is **`/dev/ttyUSB0`** if there is only one device connected over USB).
* Open and Arduino IDE; Verify & Upload the sketch **`arduino/ultra_sonic_sensor.ino`** to the board.


## Running the program

        python python/capture_user.py /dev/ttyUSB0

Depending on the range you have set in the python script `capture_user.py` `RANGE` variable, the script will activate the camera, captures the image and saves it. You can find the image in your $HOME/image_captures/ directory
