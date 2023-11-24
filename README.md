#Smart Home Automation System
By
Syed Muhammad Tahir

Title: Smart Home Automation System with Arduino, Bluetooth,Relay and Android App

Abstract:
Smart Home Automation Systems are becoming increasingly popular due to their ability to enhance convenience and efficiency. This report details the development of a Smart Home Automation System utilizing Arduino, a Bluetooth module, a relay, a 5-volt battery and a Bluetooth Android app. The primary functionality of the system is to remotely control the ON/OFF state of lights within a home using a mobile device.

1. Introduction:
The aim of this project is to create a simple yet effective Smart Home Automation System that allows users to control the lighting in their homes wirelessly. The system is built around the Arduino platform, incorporating a Bluetooth module for communication, a relay for switching the lights, a 5-volt battery for power, and a breadboard for prototyping.

2. Components Used:
 
Hardwares:

a. Arduino UNO

b. HC-05 Bluetooth Module

c. 5 V Relay X 4

d. 5V Power Source

e. Connecting wires

f. Bluetooth Android App

g. Smartphone or tablet (Bluetooth enabled)


Softwares:

Arduino 1.8.19 compiler (application software)

a)Arduino UNO
![image](https://github.com/TahirHussaini0025/SmartHome-Lights-Control/assets/141020681/325d4998-6c4c-42e1-b4ba-eaa5ed940332)
The brain of the system, responsible for processing commands and controlling the relay.


b)HC-05 Bluetooth Module
![image](https://github.com/TahirHussaini0025/SmartHome-Lights-Control/assets/141020681/d4215647-7e31-4117-a326-e0d925055cf0)
Enables wireless communication between the Arduino and the Android app.


c)5 V Relay X 4
![image](https://github.com/TahirHussaini0025/SmartHome-Lights-Control/assets/141020681/5c90f606-13e3-43af-b674-17d31471834f)
Acts as a switch to control the ON/OFF state of the lights.


d)5V Power Source
![image](https://github.com/TahirHussaini0025/SmartHome-Lights-Control/assets/141020681/4c3c87a2-005f-4287-bc02-71847d094e8a)
Power Bank 5V 2A charger circuit module Power Supply Electronic


e)Connecting wires
![image](https://github.com/TahirHussaini0025/SmartHome-Lights-Control/assets/141020681/7857adc5-131f-47f4-baa0-c80c413c533f)
Connecting wires with Arduino UNO, Relay and Bluetooth Modules


f)Bluetooth Android App
![image](https://github.com/TahirHussaini0025/SmartHome-Lights-Control/assets/141020681/65b7f8be-c5fe-4f57-a0d8-d1c9a96a493a)
An application developed for controlling the lights remotely.


g)Smartphone or tablet (Bluetooth enabled)
![image](https://github.com/TahirHussaini0025/SmartHome-Lights-Control/assets/141020681/4f278072-b0cb-4701-9dc2-cc52c687d03a)


h)Arduino 1.8.19 compiler (application software)
![image](https://github.com/TahirHussaini0025/SmartHome-Lights-Control/assets/141020681/d35c1741-f088-418e-86e3-c6a1fd96ba4a)
In this compiler we enter a code and run it to train a mudule in Arduino UNO



3. System Architecture:
The Bluetooth module is connected to the Arduino, and the relay is connected to the output pins of the Arduino. The lights are connected to the relay. The Arduino is powered by the 5-volt battery. The Android app communicates with the Bluetooth module to send ON/OFF commands.

The flow diagram that explains the flow of the project.
![image](https://github.com/TahirHussaini0025/SmartHome-Lights-Control/assets/141020681/28ada6b7-de6e-48ee-846d-0168ff0309e9)



4. Working Principle:
The Android app sends ON/OFF commands to the Arduino via Bluetooth.
The Arduino processes the received commands and controls the relay accordingly.
The relay switches the lights ON or OFF based on the Arduino's command.
5. Implementation Steps:
a. Connect the Bluetooth module to the Arduino following the datasheet. b. Connect the relay to the Arduino output pins. c. Connect the lights to the relay. d. Power the Arduino using the 5-volt battery. e. Develop a simple Android app with Bluetooth capabilities. f. Pair the Android app with the Bluetooth module. g. Implement code on the Arduino to process Bluetooth commands and control the relay.



Arduino Coding:-
char val;
void setup() {
pinMode(13,OUTPUT);
Serial.begin(9600);
 digitalWrite(13,HIGH);
  
}
void loop() {
  if(Serial.available()){
 val = Serial.read();
 Serial.println(val);
}
if(val=='1'){
  digitalWrite(13,LOW);
}
else if(val=='2'){
  digitalWrite(13,HIGH);
}
delay(100);
}





Implementation
Circuit Diagram

6. Results:
Upon successful implementation, the lights can be remotely controlled using the Android app. The system provides a user-friendly interface for convenient home automation.


7. Conclusion:
The Smart Home Automation System presented in this report demonstrates the effective use of Arduino, Bluetooth technology, and a relay to control lights wirelessly. This project serves as a foundation for expanding home automation capabilities and can be extended to control other devices within a smart home environment.
8. Future Enhancements:
Integration with other smart home devices.
Implementation of voice control.
Enhancements to the Android app for additional features.
In conclusion, this project showcases the potential of integrating Arduino-based systems with mobile technology to create practical and user-friendly smart home solutions.




Thank You..........








Help-line:~
Contact No : 03554250025
