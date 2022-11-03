# WRO 2022 Future Engineers I-ROBONATOR

This repository contains engineering materials of a self-driven vehicle's model participating in the WRO Future Engineers competition in the season 2022.

## Content

- `t-photos` contains 2 photos of the team (an official one and one funny photo with all team members)
- `v-photos` contains 6 photos of the vehicle (from every side, from top and bottom)
- `video` contains the video.md file with the link to a video where driving demonstration exists
- `schemes` contains one or several schematic diagrams in form of JPEG, PNG or PDF of the electromechanical components illustrating all the elements (electronic components and motors) used in the vehicle and how they connect to each other.
- `src` contains code of control software for all components which were programmed to participate in the competition

## Our Team

-Vun Xiu Xuan

-Alvin Kong Wei Ee 

-Lai Chaun Choy 

## Introduction

This project is a self-driven vehicle's model participating in the WRO Future Engineers competition in the season 2022. The vehicle is designed to be able to drive on a 2D surface and to be able to detect and avoid obstacles. The vehicle is constructed with Lego Mindstorms EV3 Education set and is controlled by Lego Mindstorms EV3 Brick.

## Build of Robot

The build of vehicle is mainly based on Lego Mindstorms EV3 Education set. The vehicle is constructed with 2 motors, 1 color sensor, 1 gyro sensor, 1 ultrasonic sensor and [Pixy2](https://pixycam.com/pixy2/) Camera. The vehicle is controlled by Lego Mindstorms EV3 Brick.

### Chassis

The chassis is constructed with Lego Technic Parts from Lego Mindstorms EV3 Education set.

### Motors

There are 2 motors in the vehicle. One motor is used to drive the vehicle and the other one is used to control the steering of the vehicle.

#### Motor 1: Steering Motor

Lego Medium Servo Motor is used as the steering motor.

#### Motor 2: Driving Motor

Lego Large Servo Motor is used as the driving motor. The driving motor is connected to a differential gear which allows one wheel to travel at a different speed than the other during turning, while both remain powered.

### Sensors
There are 4 sensors used in this vehicle.

#### Color sensor
The color sensor help to scan and measure the color number and ouput in color. 
When the color sensor detected the orange or blue color on the map, it will adjust the steering to turn in certain direction.

#### Gyro sensor
The gyro sensor will help to detect rotational motion. Reset mode of the gyro sensor can minimize the "drifting" that cause the angle become inaccurate.

#### Ultrasonic sensor
The ultrasonic sensor can help to measure the distance to an object in front of it. Therefore, the sensor that install at the side of the vehicle can allow the vehicle to move in a suitable distance that would not cause it to knock the wall. This is because the ultrasonic sensor will make sure the vehicle to run in the middle of the lane.

#### Pixy2
The Pixy2 can learn to detect objects that thaught to it. For example, it can detect the red and green pillar based on the signature set. When the Pixy2 detected the green pillar, it will tell the robot to turn left.

### Software

The software is written with Lego Mindstorms EV3-Graphics programming language.

The software is divided into 2 parts: `CONFIG` and `MAIN`.

#### CONFIG

The `CONFIG` part is the configuration part of the software. It contains the configuration of the vehicle.

#### MAIN

The `MAIN` part is the main part of the software. It contains the main program of the vehicle.

## Round 1
Round 1 is known as qualifying round. Our teams will programmed the robot vehicle to run in a proper way that will not knock on the wall. The ultrasonic sensor will be set up to make sure the vehicle is in certain distance away from the wall. Next, when the color sensor detected the orange line, the vehicle will react by turning left. When the color sensor detected blue line, the vehicle will react by turning right.

## Round 2
For round 2, the main core of programming used is also same with the round 1. However, sensors such as Pixy2 are being used to avoid hitting the obstacles. When there is no pillar in front of the vehicle, the robot will start to run in certain distance away from the wall by using ultrasonic sensor to make sure the vehicle run in the middle of the lane. When the Pixy2 sensed the green pillar, the robot will turn the steering to the left and when the Pixy2 sensed the red pillar, the robot's steering will turn to right.

## Driving Demonstration
This is our driving demonstration on both task which is without pillars and with pillars.
https://youtu.be/Tq-YRfk3yTg 

## How to Setup and Run
Before the robot vehicle is being quarantined, the program will be downloaded to the brick through the USB cable. The robot will be placed in the starting zone that has been determined by the judges.  When the judge gives the signal to start the vehicle, the starting button is then pressed to run the program.


## Credits
We would like to express our gratitude to LEGO Education for their support and effort in providing us a good quality of LEGO EV3 sets. Besides that, the LEGO Mindstorms EV3 websites also contribute lots of reference that guide us to create the programming for the competition.
