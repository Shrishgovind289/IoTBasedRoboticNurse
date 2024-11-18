# IoTBasedRoboticNurse

Abstract

In this project I will be building a robot which can go patient with contagious diseases like COVID-19. And give them all basic necessities such as food, medicine.

Introduction

In this project we have used 2 DC motors which is controlled by NodeMCU (ESP8266), the motors are driven using L298D motordriver. The main objective of this project is to reduce the interaction of patients with doctors or nurse who are suffering from contagious diseases like COVID-19, which will help in reducing the wild spread of the disease. The robot will be controlled using a IoT based application Blynk.

Implementation

The system was made using NodeMCU (ESP8266), L298D which is used to control the 2 DC motors. The system is controlled by the user using Blynk IoT application. The robot will have a battery pack which will enable it to run independently. The battery is used to power the motordriver the NodeMCU as well. The system layout is such that the application has number of patients and its location in the room. So when the nurse gets a patients respective food or medicine they can load the item on the robot for it to deliver to the said patient. Robot once received signal from the Blynk application will follow pre-set instructions which to engaging forward or reverse to move the robot forward, reverse or turn left and right. For example, if the robot needs to be sent to Patient 1. Then both wheels will be rotating in forward motion for 10 seconds, take a right turn by 90 ̊ by rotating right motor in forward and left motor in reverse for 300 milliseconds, move forward for another 2 seconds to reach the patient’s bedside. It will stop for 10 seconds for patient to take all the items placed there by the nurse. Once the patient has received and collected all their items the robot will move backwards for 2 seconds and turn right by 90 ̊ for 300 milliseconds to face the main door and move forward for 10 seconds, once it reach the main door it will rotate 180 ̊ and stop for next set of instructions. Commands for moving the robot forward, backward, and turning it right and left is already done in form of preset functions. And for each patients only the delay use these commands vary. The main variation comes in the reaching the base of patient’s bed where the robot needs to turn either right or left.

Applications and Future scope

1) It is used to reduce interaction between patients and doctors/nurse
which will reduce the risk of spreading of diseases.
2) We can further improve its efficiency but taking commands for 2
patients at once.
3) We can add some basic sensors such IR Temperature sensor to
monitor patient’s temperature, have servos with arm-like extension
to extend Oximeter.
4) Add arms to serve the food/medicine to the respective patient.


Results
https://youtube.com/shorts/iEHpPss8-1A?si=lRjrq_-ORD3xqvn7
