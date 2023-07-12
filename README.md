# IOT-based emergency ambulance detection system
## Introduction
Based on the START triage method and inspired by the emergency response documentary of the Puyuma train derailment accident, we have conceived an emergency medical triage system based on machine learning and the Internet of Things.
During large-scale accidents, a single device can classify and assess injuries for individual patients while simultaneously measuring six vital signs in real-time, including respiration, heartbeat, blood oxygen level, body temperature, diastolic pressure, and systolic pressure. This device addresses the limitations of traditional triage tools such as START. Additionally, it is equipped with an embedded system that allows for monitoring during emergencies and provides immediate alerts through voice reminders. Moreover, using Bluetooth technology, this device can transmit the patients' vital signs and location information to the disaster response center, enabling rescue personnel to promptly understand the patients' conditions.

Here are the example images showcasing the functionalities of our intelligent steering wheel system:

<p float="left">
  <img src="https://github.com/hsh0615/picture/blob/main/%E5%9C%96%E7%89%878.png" alt="Improper Hand Placement" width="270" />
  <img src="https://github.com/hsh0615/picture/blob/main/%E5%9C%96%E7%89%877.png" alt="Driver Fatigue Detection" width="270" /> 
  <img src="https://github.com/hsh0615/picture/blob/main/%E5%9C%96%E7%89%879.png" alt="Drunk Driving Detection" width="270" />
</p>

## HW/SW Setup
### 【Hardware Requirements】
- **     ARC EM9D       **(IoT Applications Platform)
- **      Buttons		**(Selecting a Level of Detection)
- **   Finger switch    **(Locking Detection Level)
- **      MAX86150      **(PPG Sensor 			  , Physiological Signal Detection)
- **       TMP117		**(Body Temperature Sensor, Physiological Signal Detection)
- **       ST7735		**(Full Color LCD Monitor , Displays injury level and vital signs)
- ** 	  SD178BMI      **(Voice Module			  , Accidental Voice Alert)
- **      PCA9672		**(Expansion I/O		  ,Connections to ST7735 DC, Pushbutton, Thumb Switch)
- **     RBW6100-RA		**(BT 5.1				  ,Transmit vital signs and location to on-site disaster centers)
- **     GY-NEO6MV2     **(GPS Model			  ,Getting the location)
![hardware](https://github.com/hsh0615/picture/blob/main/%E5%9C%96%E7%89%875.png)
### 【Software】
- **PPG SQI Model**
![image](https://github.com/hsh0615/picture/blob/main/SQI-good-bad.png)
![image](https://github.com/hsh0615/picture/blob/main/accuracy-sqi.png)
- **Yawn detection Model**
![image](https://github.com/hsh0615/picture/blob/main/Yawn.png)
![image](https://github.com/hsh0615/picture/blob/main/accuracy-yawn.png)

## User manual
### 【Setup on Car】
![硬體](https://github.com/hsh0615/picture/blob/main/%E7%A1%AC%E9%AB%94.png) ![汽車](https://github.com/hsh0615/picture/blob/main/car-resize.png)
### 1. Hands Off the Wheel Testing
![image](https://github.com/hsh0615/picture/blob/main/hand-off.png)
### 2. Driver Yawn Testing
![image](https://github.com/hsh0615/picture/blob/main/Driver-Yawn.png)
### 3. Driver Drunkenness
![image](https://github.com/hsh0615/picture/blob/main/Drunk.png)
### 4. Cloud Testing
- When the Safety Steering Wheel detects potential signs of drunk driving, it will trigger the cloud testing process.
![Hardware](https://github.com/hsh0615/picture/blob/main/python-cloud-gps.png)

### Youtube link
- https://www.youtube.com/watch?v=9_kwLSGJuDw
