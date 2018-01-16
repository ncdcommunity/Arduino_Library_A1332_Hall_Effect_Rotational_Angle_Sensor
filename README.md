
[![A1332](A1332_I2C.png)](https://store.ncd.io/product/a1332-precision-hall-effect-rotational-angle-0-to-360-sensor-i2c-mini-module/)

#  A1332
A1332 is a Precision Hall Effect Rotational Angle 0° to 360° Sensor.
This Device is available from www.ncd.io

[SKU:  A1332_I2CS]

(https://store.ncd.io/product/a1332-precision-hall-effect-rotational-angle-0-to-360-sensor-i2c-mini-module/)
This Sample code can be used with Arduino.

Hardware needed to interface A1332 Hall effect sensor with Arduino
1. <a href="https://store.ncd.io/product/i2c-shield-for-arduino-nano/">Arduino Nano</a>
2. <a href="https://store.ncd.io/product/i2c-shield-for-arduino-micro-with-i2c-expansion-port/">Arduino Micro</a>
3. <a href="https://store.ncd.io/product/i2c-shield-for-arduino-uno/">Arduino uno</a>
4. <a href="https://store.ncd.io/product/dual-i2c-shield-for-arduino-due-with-modular-communications-interface/">Arduino Due</a>
5. <a href="https://store.ncd.io/product/a1332-precision-hall-effect-rotational-angle-0-to-360-sensor-i2c-mini-module/">A1332 Hall Effect Sensor</a>
6. <a href="https://store.ncd.io/product/i%C2%B2c-cable/">I2C Cable</a>

A1332:

The A1332 is a 360° contactless high resolution programmable magnetic angle position sensor IC. It is designed for digital systems using and I²C interface.The A1332 is ideal for automotive applications requiring high speed 360° angle measurements. 

Applications:

• Electronic power steering (EPS)

• Transmission

• Torsion bar

• Other systems that require accurate measurement of angles

## Arduino

Download and install Arduino Software (IDE) on your machine. Steps to install Arduino are provided at:

https://www.arduino.cc/en/Main/Software

Download (or git pull) the code and double click the file to run the program.
Compile and upload the code on Arduino IDE and see the output on Serial Monitor.

How to Use the A1332 Arduino Library
The A1332 is very easy to interface with arduino.There are only 3 steps as following:

1. Begin transmission:You have just start the transmission at the address of A1332 hall effect sensor by the following command:
            
       Wire.beginTransmission(address);  //start the transmission at the A1332 address

2. End transmission:After the begining of transmission you have to end the transmission by the following command:

       error = Wire.endTransmission();  // end the transmission and store the result in "error" variable

3. Read value:The value of angle can be measured by using following command and the output should be in degree.

       magAngle = a1332.Measure_HallSensor();  // read the angle value if the "error" variable is 0
