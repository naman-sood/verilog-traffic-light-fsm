# verilog-traffic-light-fsm
FSM-based traffic light controller designed in Verilog for the ZedBoard, with complete RTL and testbench simulation in Vivado.


📘 FPGA-Targeted Traffic Light Controller (Verilog FSM)

A clean and modular Verilog-based traffic light controller, designed using Finite State Machines (FSM) and verified through RTL simulation in Xilinx Vivado.
The design targets the Xilinx ZedBoard (FPGA) and demonstrates proficiency in synchronous digital design, timing control, and simulation-driven verification.

🚦 Project Overview

This project implements a traffic light controller for a highway–farm road intersection, using:

Well-structured FSM architecture

Parameterized timing using counters

Optional input for HC-SR501 PIR sensor (simulation logic included)

Complete testbench for waveform verification

The work focuses on FPGA-oriented RTL design, not physical deployment.

🧩 Features

Three-state FSM (Highway Green → Highway Yellow → Farm Green)

Sensor-triggered state override logic (PIR)

Parameterized delays for realistic timing

Modular Verilog design with separate logic + top module

Fully tested using Vivado simulation

Clean waveforms showing correct timing and transitions

🛠 Tools & Technologies

Verilog HDL

Xilinx Vivado (Simulation + RTL analysis)

Finite State Machines (FSM)

FPGA-oriented design (ZedBoard)

Testbench development & waveform debugging

🎯 Design Architecture
State Machine

HGRE_FRED — Highway Green, Farm Red

HYEL_FRED — Highway Yellow, Farm Red

HRED_FGRE — Highway Red, Farm Green

Each state uses counters driven by the clock to generate real-time delays.

Sensor Integration (Simulated)

A PIR sensor input is sampled to trigger early transition to the farm-road green state.

▶️ Simulation & Results

The behavior was verified entirely through Vivado Behavioral Simulation:

Correct sequencing through all FSM states

Highway → Yellow → Farm transitions match configured delays

Sensor-triggered override successfully tested

Clean waveforms demonstrate proper synchronous timing

