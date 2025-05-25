# Indigenous-Robot-for-National-Engineering-Robotic-Context-NERC-
Line-Following Robot with Object Manipulation
## Overview
This Arduino code controls an autonomous robot capable of:

-- Precise line following
-- Junction detection and counting
-- Object (rock/tree) pickup and placement
-- Complex path navigation
-- Reverse movement with line following

## Hardware Components
Microcontroller: Arduino (unspecified model)

## Sensors:
-- 5x line following sensors (leftmost, left, middle, right, rightmost)
-- 2x side sensors
-- 2x rock/tree detection sensors
-- 2x reverse line following sensors
-- 9x grid sensors (3x3 matrix)

## Actuators:
-- 2x DC motors with H-bridge control
-- 1x SG90 servo motor for object manipulation

## Key Features
-- Junction-based navigation system with counter
-- PID-like line following algorithm
-- Precise object pickup/drop mechanism
-- Reverse line following capability
-- Configurable speed and servo positions

## Installation
-- Upload the sketch to your Arduino board
-- Connect all sensors and motors as specified in the pin definitions
-- Calibrate motor speeds and servo positions as needed 

## Usage
The robot autonomously:
-- Follows a line path
-- Counts junctions
-- Performs specific actions at predetermined junctions:
-- Picks up objects (rocks/trees)
-- Transports them to designated locations
-- Drops them precisely
-- Navigates complex paths with turns and reverse movements

## Customization
Modify these variables for your specific setup:
-- lpwm, rpwm: Motor speed values
-- serdown, serup: Servo positions for object handling
-- Junction count values in the main loop for different paths

## Important Notes
Sensor readings:
-- Line sensors return HIGH/LOW for line detection
-- Rock/tree sensors return HIGH on black
-- Reverse sensors return LOW on black

The code includes debug Serial.print statements for monitoring

## File Structure
Leftarena_rightdiagonal.ino: Main Arduino sketch containing all logic

