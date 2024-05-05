[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/kzkUPShx)
# a14g-final-submission

    * Team Number: 14
    * Team Name:  HumidifierZ
    * Team Members: Haomin Zhu; Hao Zhang
    * Github Repository URL: https://github.com/ese5160/a14g-final-submission-t14-humidifierz.git
    * Description of test hardware: (development boards, sensors, actuators, laptop + OS, etc): laptop, whole humdifier product

## 1. Video Presentation
Here is the link of our video
https://youtu.be/VFljNrePpyU

## 2. Project Summary
### Device Description
This is a humidifier that can spray water automatically. We use multiple sensors to detect humidity, temperature, tank level and other parameters. Users can set the target humidity according to their own needs. After the setting is completed, the humidifier will work automatically and display the environmental data on the user interface in real time. After setting, the humidifier will work automatically and display the environmental data on the user interface. Users can adjust their own settings according to the data feedback from the user interface, also can control the humidifier remotely by cell phone or computer.

### Inspiration
Water is an indispensable part of people's lives. Living in a humid environment has certain benefits for the human body, so in recent years humidifier is a more popular household appliances. However, humidifiers on the market generally do not have networking capabilities, but also can not be controlled remotely, very inconvenient. So we wanted to design a smart humidifier that can be controlled remotely and can see the room humidity, temperature and other parameters in real time to provide a better user experience.

### Device Functionality
This device has five main parts. There are two sensors, two actuators and one controller. It can detect the ambient temperature and humidity by temperature and humidity sensors (SHTC3-TR-10KS), also detect the water level of the humidifier tank in real time by distance sensor (4007). Then the information of the temperature, humidity and water level data in real time will be displayed on the OLED (SSD1306) display. The second actuator is humidifier module. It is made up from two parts: one is vibrating tablet and other is driving circuit which can supply specific frequency power signal. This module starts when the ambient humidity is below the set value and stops when it is above the set value. In general, the user can control the humidifier through the software, and power the atomizing ceramic piece through the driving circuit to form a spray. When the water level is below a certain condition, the software will alert the user and the display will present warning text to prompt the user to change the water.

### Challenges
Where did you face difficulties? This could be in firmware, hardware, software, integration, etc.
How did you overcome these challenges?
### Prototype Learnings
What lessons did you learn by building and testing this prototype?
If you had to build this device again, what would you do differently?
### Next Steps
What steps are needed to finish or improve this project?
### Takeaways from ESE5160
What did you learn in ESE5160 through the lectures, assignments, and this course-long prototyping project?
### Project Links

## 3. Hardware & Software Requirements
### Hardware Requirement
#### HRS 01 – Project shall be based on SAMW25 microcontroller
We meet the requirement.

#### HRS 02 – 4007 distance sensor shall be used for obstacle detection. The sensor should be able to measure a 16cm change in water level (the sensor shall be able to measure a minimum of 4cm and a maximum of 20cm from the water surface). Data shall transfer to microcontroller via GPIO.
We meet the requirement. The range of measurement distance have a small change, it is 4cm to 15cm.

#### HRS 03 – An 1.30 inch OLED SSD1306 display shall be used for user interface. The display shall communicate with the microcontroller via I2C bus.
We meet the requirement.

#### HRS 04 – A Temperature and humidity sensors(SHTC3-TR-10KS) shall be used to detect ambient temperature and humidity. Data shall transfer to microcontroller I2C bus.
We meet the requirement.

#### HRS 05 – A humidifier module shall be used to generate water mist to humidify the air. Humidifier module shall be controlled by GPIO.
We meet the requirement.

#### HRS 06 – A WIFI module WINC1500 shall be used to send data to cloud service and receive commands from cloud service. The WIFI module shall communicate with the microcontroller via SPI.
We meet the requirement.

#### HRS 07 – A button shall be used to control the device on and off. The button shall be connected to the microcontroller via GPIO.
We did not create a button to control. When we build 3D model, we found that there is hard to place a button and it is not useful. According to this, we detect this part.

#### HRS 08 – A LED shall be used to show device on and off. The LED shall be connected to the microcontroller via GPIO.
We meet the requirement.

### Software Requirment
#### SRS 01 – The 4007 distance sensor shall measures the water level continuously. When the water level falls below a certain value, low water mode will be activated.
We meet the requirement.

#### SRS 02 – The temperature and humidity sensors shall measures the ambient temperature and humidity continuously.
We meet the requirement.

#### SRS 03 – OLED shall display ambient temperature humidity and water level.
We meet the requirement.

#### SRS 04 – The wifi module shall be able to send temperature, humidity, operating status, and water level information to the cloud service. The wifi module shall be able to accept commands from the cloud service.
We meet the requirement.

#### SRS 05 – Humidifier module shall work below the set humidity level and stop working above the set humidity level. The set humidity level shall be set by user via wifi module.
We meet the requirement.

## 4. Project Photos & Screenshots
### Final Project
<img src="https://github.com/ese5160/a14g-final-submission-t14-humidifierz/assets/147022262/562a0aa6-c602-493d-af88-d8364d76bf94" width="45%"></img> 
<img src="https://github.com/ese5160/a14g-final-submission-t14-humidifierz/assets/147022262/f0283abd-65c9-4df4-bb36-71d3559b4b6d" width="45%"></img> 
<img src="https://github.com/ese5160/a14g-final-submission-t14-humidifierz/assets/147022262/fa4ba896-737b-4572-a2f5-6cff1e02aa52" width="45%"></img> 
<img src="https://github.com/ese5160/a14g-final-submission-t14-humidifierz/assets/147022262/b0542401-0473-4882-bcf0-95bf63d03816" width="45%"></img> 

### PCBA
TOP

<img src="https://github.com/ese5160/a14g-final-submission-t14-humidifierz/assets/147022262/5aa05539-c385-44d5-b861-1534afa6b568" width="45%"></img> 
<img src="https://github.com/ese5160/a14g-final-submission-t14-humidifierz/assets/147022262/0127d1f1-4f41-42d8-97bc-7ad0da3538e8" width="45%"></img> 
<img src="https://github.com/ese5160/a14g-final-submission-t14-humidifierz/assets/147022262/ec198045-58b6-4b64-a812-bae20a20bf6c" width="45%"></img> 

BOTTOM

<img src="https://github.com/ese5160/a14g-final-submission-t14-humidifierz/assets/147022262/217dcfcd-8c54-4812-bcc6-949ed201cd28" width="45%"></img> 

THERMAL IMAGE

<img src="https://github.com/ese5160/a14g-final-submission-t14-humidifierz/assets/147022262/fb67dfba-710d-4ca1-a75d-8abcb1d85d8f" width="45%"></img> 

### Design Circuit
2D View

<img src="https://github.com/ese5160/a14g-final-submission-t14-humidifierz/assets/147022262/f522df86-b556-4973-8275-3689bf7f74cd" width="45%"></img>

3D View

<img src="https://github.com/ese5160/a14g-final-submission-t14-humidifierz/assets/147022262/978b3941-caba-4427-b78a-b016bea3333e" width="45%"></img> 

### Node-RED Screenshot
Node-RED dashboard 

<img src="https://github.com/ese5160/a14g-final-submission-t14-humidifierz/assets/147022262/90c7706b-07d0-4d49-a665-170be114c250" width="45%"></img> 

Node-RED backend

<img src="https://github.com/ese5160/a14g-final-submission-t14-humidifierz/assets/147022262/99e08aac-41f2-49fc-ba89-75302ce1955f" width="45%"></img>  

### Block diagram
<img src="https://github.com/ese5160/a14g-final-submission-t14-humidifierz/assets/147022262/e63bf1a5-677b-4853-b061-c0d20e4c346e" width="45%"></img> 
<img src="https://github.com/ese5160/a14g-final-submission-t14-humidifierz/assets/147022262/f3ee7575-b174-4f43-b812-3c85855869b7" width="45%"></img> 


 
















 
 


