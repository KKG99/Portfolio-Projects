# Kiran Kumar's Skill Showcase

Welcome to my portfolio! Here, you'll find a curated collection of works demonstrating my expertise and experience with various software tools.

## About Me
I am a Master's student at the University of Bremen specializing in Space Engineering, with a solid foundation in Mechanical Engineering. Through diverse, user-centric projects, I've honed my skills and continue to explore various areas within the engineering realm. I'm committed to continuous learning and staying abreast of the latest advancements in technology.

## Table of Contents
- [SysMLv2: Garage Door Controller Model](#sysmlv2-garage-door-controller-model)
- [SysMLv2: Structural Model for the Turn Indication Controller](#sysmlv2-structural-model-for-the-turn-indication-controller)
- [SysMLv2: Behavioural Model for the Turn Indication Controller](#sysmlv2-behavioural-model-for-the-turn-indication-controller)

## SysMLv2: Garage Door Controller Model

### Overview
This work demonstrates my proficiency with SysMLv2 through the modeling of a Garage Door Controller (GDC) system. The GDC controls the up and down movements of a garage door via an electric motor and handles commands such as DOWN, UP, STOP, and REVERSE based on inputs from a remote control, door sensors, and a light sensor for safety.

### Requirements
#### Safety Requirements
- The BeamCrossed signal from the light sensor must trigger a REVERSE command to ensure safety.

#### Structural Requirements
- The system must include a physical barrier around the motor to prevent physical contact.

#### Functional Requirements
- The remote control can start and stop the door's movement.
- The system can pause and resume the door movement at any point.
- A manual override option is available for emergency use.

### Operational Environment
The GDC operates within an environment including:
- Remote Control Device (ButtonPressed signal)
- Garage Door Mechanics (DoorDown and DoorUp signals)
- Light Sensor (BeamCrossed signal)
- Electric Motor (commands: DOWN, UP, STOP, REVERSE)

### System Components
#### Parts
- Remote Control
- Light Sensor
- Garage Door Mechanism

#### Target System
- Garage Door Controller (GDC)

#### Interfaces
- Ports and signals to communicate with the motor and sensors.
- Use of pre-defined signals (ButtonPressed, MotorControlCmd) and additional signals as needed.

### Behavior Model
The GDC's behavior is defined using a state machine that manages the door's states and transitions based on the received signals and commands.

### Safety Satisfaction Relations
Requirements are traced to model elements to ensure fulfillment:
- Structural requirements: Physical barrier around the motor.
- Functional requirements: Handling of ButtonPressed, DoorDown, DoorUp, and BeamCrossed signals.

## SysMLv2: Structural Model for the Turn Indication Controller

### Overview
This work showcases my ability to model structural aspects using SysMLv2 and trace structural model elements to requirements.

### Preliminaries
1. Study the informal description of the Turn Indication Controller.
2. Review the identification of structural requirements from previous exercises.
3. Introduce a new package `Structure` in the `TurnIndicationController` project.

### Structural Model
Create a structural model of the Turn Indication Controller using:
- Part definitions
- Part usages
- Port definitions
- Port usages
- Interfaces connecting ports

### Requirements Tracing
Create a package `SatisfactionRelations` to trace structural requirements to associated structural model elements. Trace requirements to concrete model element usages to ensure the existence of concrete instances in the model.


## SysMLv2: Behavioural Model for the Turn Indication Controller

### Overview
This work demonstrates my capability in modeling and implementing the behavioral aspects of a system using SysMLv2.

### Preliminaries
1. Study the informal description of the Turn Indication Controller.
2. Review the provided reference solutions and behavioral models for `CanController`, `DashboardController`, and `LampCtrlSlave`.
3. Study the behavioral requirements concerning the control of flashing indication lights based on battery state, turn indication lever, emergency flashing button, and ignition.

### Flashing Control Behaviour Model
Complete the perform action of `AutomotiveDomainLibrary/ApplicationLogic/ControlLogic` used in the rear controller to decide commands to send over the CAN bus. This decision depends on:
- BatteryVoltagePort
- TurnIndicationLeverPort
- EmergencyFlashButtonPort
- IgnitionPort

Use state machines to model and manage the transitions and control logic.

### CAN Controller
Model the perform action of the `CanController` to ensure that switching between different active flashing modes sends an OFF command first, followed by a 50ms delay before sending the new active flashing mode command.

### Tracing Behavioural Requirements
Extend the package `SatisfactionRelations` to trace the behavioral requirements on the `ControlLogic` behavior to the newly introduced behavioral model. Ensure behavioral requirements are linked to structural components performing the suitable behavior.

## Usage of the models uploded
To work with these models:
#### Prerequisites:
- Eclipse IDE: Download and install the Eclipse IDE.
- SysMLv2 Plugin: Install the SysMLv2 plugin in Eclipse:
  - Open Eclipse.
  - Go to Help > Eclipse Marketplace.
  - Search for SysMLv2 and install the plugin.

#### Steps to Use the Model:
1. Extract the Project Files:
   - Unzip the project files and ensure the folders are accessible.
2. Open Eclipse:
   - Start your Eclipse IDE.
3. Import the Project:
   - Navigate to File > Import > Existing Projects into Workspace.
   - Select the folder where the project is extracted.
   - Ensure all files are visible in the Project Explorer.
4. Open SysML Diagrams:
   - Right-click on any `.sysml` file (e.g., `Parts.sysml`).
   - Choose `Open with SysML Editor`.
   - Start exploring the model elements using the SysML diagram editor.
