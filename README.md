# Basic_traffic_Light_Controller

Overview
This project implements a Traffic Light Controller using Verilog, simulating the operation of traffic signals at an intersection. The RTL design efficiently manages traffic flow at intersections, ensuring safety and reducing congestion by sequencing lights based on traffic conditions.

Features:
Automated light sequencing: Red, yellow, and green lights cycle in a timed manner.
Configurable signal timings: Timings for red, yellow, and green lights can be adjusted.
Testbench included: The provided testbench verifies the functionality of the Traffic Light Controller.
Files
TrafficLightController.v

Contains the Verilog code for the Traffic Light Controller.
Implements the state machine logic to control the light sequence.
TrafficLightControllerTestBench.v

Testbench code for simulating the Traffic Light Controller.
Verifies the correctness of the state transitions and output signals.
How It Works
The Traffic Light Controller uses a finite state machine (FSM) to control the sequence of traffic lights. The main states in the controller are:

Green: Traffic is allowed to flow.
Yellow: A warning before the transition to red.
Red: Traffic is stopped to allow cross traffic.
The lights follow a timed sequence:

Green: For a set time period, traffic is allowed.
Yellow: The yellow light is displayed briefly as a warning.
Red: Traffic stops completely.
The FSM transitions between these states based on time intervals, which can be modified in the Verilog code.

Simulation and Testing
To verify the functionality of the Traffic Light Controller, the testbench simulates the controller’s operation over a series of cycles. It checks that:

The green light is followed by yellow, then red.
Each state lasts for the correct duration.
The controller correctly transitions between states without skipping.
Running the Simulation
Install any Verilog simulation tool, such as ModelSim, Vivado, or Icarus Verilog.
Load the TrafficLightController.v file into the tool.
Load the TrafficLightControllerTestBench.v file to run the test.
Simulate the design to verify that the state transitions are working as expected.
Requirements
Verilog simulator (e.g., ModelSim, Vivado, Icarus Verilog)
Basic understanding of digital logic and state machines
Future Enhancements
Implement adaptive timing based on traffic density, using sensors to adjust light timings dynamically.
Add pedestrian crossing signals with a synchronized light sequence.
Integrate with IoT systems for real-time traffic monitoring and control.
Conclusion
This Verilog-based Traffic Light Controller serves as a basic model for managing traffic flow at an intersection. Its modular design allows for future extensions, making it suitable for a variety of real-world applications where traffic control is needed.
