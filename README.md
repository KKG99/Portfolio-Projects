# Kiran Kumar's Project Portfolio

Welcome to my project portfolio! Here you'll find a curated collection of projects showcasing my skills, experiences, and passion for technology.

## About Me
I am a Master's student at the University of Bremen specializing in Space Engineering, with a solid foundation in Mechanical Engineering. Through a variety of user-centric projects, I've honed my skills and continue to explore diverse areas within the engineering realm. I'm committed to continuous learning and staying abreast of the latest advancements in technology. 

## Table of Contents
- [Project 1: Garage Door Controller Project](#project-1-project-title)
- [Project 2: Project Title](#project-2-project-title)
- [Project 3: Project Title](#project-3-project-title)
- [Project 4: Project Title](#project-4-project-title)

## Project 1: Garage Door Controller Project

## Overview
This project focuses on modelling a Garage Door Controller (GDC) system using SysMLv2. The GDC controls the up and down movements of a garage door via an electric motor. It handles commands such as DOWN, UP, STOP, and REVERSE based on inputs from a remote control, door sensors, and a light sensor for safety.

## Requirements
### Safety Requirements
- BeamCrossed signal from the light sensor must trigger a REVERSE command to ensure safety.

### Structural Requirements
- The system must include a physical barrier around the motor to prevent physical contact.

### Functional Requirements
- The remote control can start and stop the door's movement.
- The system can pause and resume the door movement at any point.
- A manual override option is available for emergency use.

## Operational Environment
The GDC operates within an environment including:
- Remote Control Device (ButtonPressed signal)
- Garage Door Mechanics (DoorDown and DoorUp signals)
- Light Sensor (BeamCrossed signal)
- Electric Motor (commands: DOWN, UP, STOP, REVERSE)

## System Components
### Parts
- Remote Control
- Light Sensor
- Garage Door Mechanism

### Target System
- Garage Door Controller (GDC)

### Interfaces
- Ports and signals to communicate with the motor and sensors.
- Use of pre-defined signals (ButtonPressed, MotorControlCmd) and additional signals as needed.

## Behavior Model
The GDC's behavior is defined using a state machine that manages the door's states and transitions based on the received signals and commands.

## Safety Satisfaction Relations
Requirements are traced to model elements to ensure fulfillment:
- Structural requirements: Physical barrier around the motor.
- Functional requirements: Handling of ButtonPressed, DoorDown, DoorUp, and BeamCrossed signals.

## Usage
To work with this project, follow the steps below:

### Prerequisites:
-Eclipse IDE: Download and install the Eclipse IDE from Eclipse Downloads.

-SysMLv2 Plugin: Install the SysMLv2 plugin in Eclipse:
Open Eclipse.
Go to Help > Eclipse Marketplace.
Search for SysMLv2 and install the plugin.
Steps to Use the Project:
Extract the Project Files:
Unzip the project files and ensure the folder GarageDoorController is accessible.

-Open Eclipse:

-Start your Eclipse IDE.
Import the Project:

-Navigate to File > Import > Existing Projects into Workspace.
Select the GarageDoorController folder where the project is extracted.
Ensure all the files (e.g., Parts.sysml, Requirements.sysml) are visible in the Project Explorer.
Open SysML Diagrams:

-Right-click on any .sysml file (e.g., Parts.sysml).
Choose Open with SysML Editor.
You can start exploring the model elements such as parts, requirements, and satisfaction relations using the SysML diagram editor.
