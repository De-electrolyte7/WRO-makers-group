# WRO-makers-group
WRO Future Engineers Robot Documentation and Development Repository
# WRO Makers Group

Autonomous Self-Driving Robot Project for WRO Future Engineers.

## Team
WRO Makers Group

## Repository Owner
De-electrolyte7

## Project Status
🚧 In Development

## Features
- Autonomous Navigation
- Obstacle Detection
- Sensor-Based Decision Making
- Future Engineers Documentation

WRO Makers Group

Robot Images and Documentation

This repository contains images and documentation for our WRO Future Engineers robot project.

Robot Overview

The robot is an autonomous vehicle designed using LEGO robotic components. It is intended for line following, obstacle detection, autonomous navigation, and future participation in robotics competitions such as WRO Future Engineers.

Images

Front View

Image showing the front of the robot with ultrasonic sensor assembly used for obstacle detection.

Rear View

Image showing the rear structure, support wheels, and cable management.

Top View

Image showing the overall component layout including the controller, sensors, and wheel arrangement.

Bottom View

Image showing the underside structure and wheel positioning.

Left Side View

Image showing the left profile of the robot including wheel placement and sensor arrangement.

Right Side View

Image showing the right profile of the robot and structural design.

Hardware Components

- LEGO controller hub
- Ultrasonic distance sensor
- Large drive wheels
- Structural LEGO frame
- Power system integrated within hub

Purpose

This repository serves as documentation for the development and testing of the robot and will be expanded with:

- Engineering Journal
- Source Code
- Test Results
- Design Improvements
- Competition Documentation

Team

WRO Makers Group
1. Program and test run for keeping a distance of 25cm to the wall by distance checking and correction.

How it works: when the distance is exactly 25cm the robot moves straight, when the distance is less than 25cm the robot tilts slightly away from the wall by reducing it's left motor speed and when the distance is greater than 25cm the robot tilts slightly toward the wall by reducing it's right motor speed.

Reason: for distance correction with wall.

2. Program and test run for straight movement using built in gyro sensor (built into the hub).

How it works: when the gyro senses no tilt (yaw = 0) the robot moves straight, when the gyro senses a tilt to the left (yaw < 0) the robot moves slightly right by reducing it's right motor speed and when the gyro senses a tilt to the right (yaw > 0) the robot moves slightly left by reducing it's left motor speed.

Reason: (a.) to straighten the robot when somewhere in the middle of the track and not near the walls. (b.) To reduce the amount of major tilts needed to correct robot if just relying on distance sensor for keeping it in the center of the track.

3. Program and test run for stopping when in front of wall.

How it works: keeps going forward until it sees either a black or white surface. In this situation when working with a white wall a black option was also added because of the color sensor's tendency to detect white as black in a farther distance than it's detection range as shown in the video, to allow the robot stop as far as possible from the wall.

Reason: to stop before hitting a track wall

4. Problem statement: 

Leaning forward after break stop.

Distance sensor on one side not being able to accommodate both clock wise and anti clockwise movement on track.

5. Additions on upgraded robot:
Front distance sensor moved to side to accommodate both clock wise and anti clock wise movement when relying on outer wall for centralization on track.
Addition of color sensor to detect black wall in front to replace distance sensor.
Small front wheels added to prevent leaning forward after stopping.
Additional magenta frame at the back of the robot for better structural integrity.

6. Program and test run for distance, gyro and color sensor track dynamic.

How it works: when the robot is within 30cm of the right wall the robot tilts left by reducing it's left motor speed, when the robot is within 30cm of the left wall the robot tilts right by reducing it's right motor speed and when it's neither within 30cm of the right wall nor the left wall and somewhere in the center it straightens itself using the gyro. It straightens itself using the gyro sensor by moving left if it's tilted right (yaw > 0), moving right if it's tilted left (yaw < 0) and going forward if it's straight.
In the video it can be seen trying to move as close as possible to the middle of the track whether it started from the middle, left or right at the beginning of the track.

Reason: to keep the robot at the middle of the track.
