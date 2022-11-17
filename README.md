# WRO 2022 Future Engineers I-ROBONATOR

This repository contains engineering materials of a self-driven vehicle's model participating in the WRO Future Engineers competition in the season 2022.

## Content

- `t-photos` contains 2 photos of the team (an official one and one funny photo with all team members)
- `v-photos` contains 6 photos of the vehicle (from every side, from top and bottom)
- `video` contains the video.md file with the link to a video where driving demonstration exists
- `schemes` contains one or several schematic diagrams in form of JPEG, PNG or PDF of the electromechanical components illustrating all the elements (electronic components and motors) used in the vehicle and how they connect to each other.
- `src` contains code of control software for all components which were programmed to participate in the competition

## Our Team

- Lai Chaun Choy (Programmer)
- Vun Xiu Xuan (Programmer)
- Alvin Kong Wei Ee (Robot handler)

## Introduction

This project is a self-driven vehicle's model participating in the WRO Future Engineers competition in the season 2022. The vehicle is designed to be able to drive on a 2D surface and to be able to detect and avoid obstacles. The vehicle is constructed with Lego Mindstorms EV3 Education set and is controlled by Lego Mindstorms EV3 Brick.

## Build of Robot

The build of vehicle is mainly based on Lego Mindstorms EV3 Education set. The vehicle is constructed with 2 motors, 1 HiTechnic NXT Color Sensor V2, 1 gyro sensor and 2 [Pixy2](https://pixycam.com/pixy2/) Camera. The vehicle is controlled by Lego Mindstorms EV3 Brick.

### Chassis

The chassis is constructed with Lego Technic Parts from Lego Mindstorms EV3 Education set.

### Motors

There are 2 motors in the vehicle. One motor is used to drive the vehicle and the other one is used to control the steering of the vehicle.

#### Motor 1: Steering Motor

Lego Medium Servo Motor is used as the steering motor.

#### Motor 2: Driving Motor

Lego Large Servo Motor is used as the driving motor. The driving motor is connected to a differential gear which allows one wheel to travel at a different speed than the other during turning, while both remain powered.

### Sensors
There are 3 types of sensors used in this vehicle.

#### HiTechnic NXT Color Sensor V2
It helps to scan and measure the color number and ouput in color. 
When the color sensor detected the orange or blue color on the map, it will adjust the steering to turn in certain direction.

#### Gyro sensor
The gyro sensor will help to detect rotational motion. Reset mode of the gyro sensor can minimize the "drifting" that cause the angle become inaccurate.

#### Pixy2
The Pixy2 can learn to detect objects that thaught to it. For example, it can detect the red and green pillar based on the signature set. When the Pixy2 detected the green pillar, it will tell the robot to turn left. The Pixy2 sensor also help the vehicle to allign with the wall and ensure the vehicle to walk straight.

## Software

The software is written with Lego Mindstorms EV3-Graphics programming language.
The software is divided into two parts which is `QUALIFY` & `MAIN`.

### QUALIFY
The `QUALIFY` part contains the progam for the qualify round.

#### Description of the program
Round 1 is known as qualifying round. Our teams will program the robot vehicle to run in a proper way that will not knock on the wall. The Pixy2 sensor is used to allign the vehicle with the wall so that the vehicle can run in a straight and same way and thus can avoid from knocking the wall. Next, our team also use the color sensor to detect the color of line. When the color sensor scan orange line, it will react by turning to the right side and vice versa for the blue color. After the color sensor detect the line, it will turn to the particular direction by 25 degree until the Pixy2 detect the wall again. The robot will continue to walk straight with the wall until detect the corner of the wall again. The robot will stop after this process is repeated by 3 loops.

### MAIN
The `MAIN` part contains the program for the final round.

#### Description of the program
For round 2, the main core of programming used is almost similar to the round 1. The color sensor wil be used  to help the robot to turn into the correct direction. However, there are 2 Pixy2 sensors will be used instead of one Pixy2 stated in the first round. The Pixy2 located at the highest is used to help the robot to turn in a correct direction. Besides that, it also help to allign the vehicle with the wall and prevent it from knocking into the wall. The Pixy2 located below will be used to avoid the traffic. The robot will avoid the pillars via the signature that have set in the Pixy2. 

## Driving Demonstration
This is our driving demonstration on both task which is without pillars and with pillars.
https://youtu.be/Tq-YRfk3yTg 

## How to Setup and Run
Before the robot vehicle is being quarantined, the program will be downloaded to the brick through the USB cable. The robot will be placed in the starting zone that has been determined by the judges.  When the judge gives the signal to start the vehicle, the starting button is then pressed to run the program.


## Credits
We would like to express our gratitude to LEGO Education for their support and effort in providing us a good quality of LEGO EV3 sets. Besides that, the LEGO Mindstorms EV3 websites also contribute vast of references that guide us to create the programming for the competition.
