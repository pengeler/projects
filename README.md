# List of Projects
The following is a list of projects that I have worked on, along with brief descriptions and involved technologies. 

Due to various restrictions, source access is only provided for selected projects. I might be able to supply access to other projects on demand.

[TOC]

# Wave simulator
**Involved Technologies**: C++, OpenGL, GLSL, SDL2, DearImGui

**Link**: [gitlab](https://gitlab.phys.ethz.ch/engelerp/framebuffer-testing)

Wave simulator controlled via a 4K multitouch display in real-time.

Plane waves are propagating over the screen, and users can either scatter the waves off their fingers, place preprogrammed obstruction patterns, or draw their own obstructions directly onto the screen. 

The finite difference simulation is performed in real time on an RTX 3080, and in operation the system performs well over 10^10 single site updates per second. 

This system is an exhibit part of the "Wellen - Tauch ein!" exhibition from FocusTerra, which has since also been shown in the Seemuseum Kreuzlingen, and is currently in the HNF Paderborn. 

More in-depth information can be found in the project's README.md, and impressions of the final device are shown below.

<img src="resources/wave_photo_side.jpeg" alt="Wellentisch" width="600"/>


# Simulation framework for system of thousands of coupled resonators
**Involved Technologies**: C++, LAPACK, python, Make

**Link**: [gitlab](https://gitlab.phys.ethz.ch/engelerp/rbcomb-simulation)

This is a simulation framework made to simulate the system I developed during my PhD, namely a system of 2000 coupled nonlinear resonators.

As several different approaches can be taken to represent the system (more theoretical assuming specific couplings, or more physical working with voltages), a lot of flexibility is provided in the definition of forces and the like.

For timestepping, an RK4 implementation is provided, but custom steppers can be plugged in instead.





# Autonomous temperature stabilization system [gitlab](https://gitlab.phys.ethz.ch/engelerp/rbcomb-temperature-control)

# FPGA lock-in amplifier [gitlab](https://gitlab.phys.ethz.ch/engelerp/stitch)

# High performance interference ray tracer
**Involved Technologies**: C++, OpenMP, python

**Link**: [gitlab](https://gitlab.phys.ethz.ch/engelerp/rbcomb-ray-tracer)

The goal of this project was writing a program that can predict interference patterns seen in a microscope, for certain configurations of deformed overlapping thin films. 
The motivation of this project was sparked by a lack of understanding of observed results in the cleanroom. 

The ray tracer is parallelized using OpenMP and was run on a cluster (Piz Daint). 
As opposed to conventional ray tracers, here rays of several different colours are traced through materials with nontrivial curvatures and refractive indices. 
The meshes used to describe various surfaces present in the scene were generated leveraging the mesher infrastructure I developed for the Structure Search project. 

The obtained results were able to reproduce observations, and guided us in the right direction for the resolution of the encountered issues.


# RBComb control system
**Involved Technologies**: VHDL, python

**Link** (partial): [gitlab](https://gitlab.phys.ethz.ch/engelerp/bridge_fpga_ram)

The control system of the RBComb experiment consists of a star network of 11 FPGAs. 
The hub receives commands from a PC via UART, and programs the other 10 FPGAs correspondingly. 
It also receives measurement data from an attocube IDS 3010, stores relevant data in LPDDR SDRAM and streams it back to the PC when requested.
The other 10 FPGAs generate analog voltages on 576 independent channels each, by controlling a total of 720 DACs.
These voltages are generated according to fully independently programmable sequences, parallelly in well synchronized manner.

The linked repo only shows the gateware flashed on the hub FPGA.

More information about the gateware can be found [in my PhD thesis](https://doi.org/10.3929/ethz-b-000678922), in the Setup chapter 4, especially 4.5 and 4.6. 
The python API to communicate with the system is described in chapter 4.4.

# PCB generation framework
**Involved Technologies**: python

**Link**: [gitlab](https://gitlab.phys.ethz.ch/code/experiment/rbcomb-breakout)

Contains classes to represent Kicad pcbs, along with scripts that use these classes to generate different versions of Breakoutboards to break out the 5000 analog nets of the RBComb sample.

# RBComb sample visualizer
**Involved Technologies**: C++, OpenGL, python

**Link**: [gitlab](https://gitlab.phys.ethz.ch/engelerp/rbcomb-sample-visualizer)

Meshes are generated in python using the earcut algorithm 

# Interactive MEMS resonator design optimizer [gitlab](https://gitlab.phys.ethz.ch/engelerp/arm-designer)

# Interactive WLI data analyzer and visualizer [gitlab](https://gitlab.phys.ethz.ch/engelerp/nt1100-analyser)

# Labbook generator [gitlab](can't, contains private information, but offer to clean up)

# Git diff [gitlab](https://gitlab.phys.ethz.ch/engelerp/gitdiff)

# FPGA defined FM transmitter [gitlab](not online yet)

# Spartan Sound
**Involved Technologies**: VHDL, python, electronics

**Link**:  [gitlab](https://gitlab.phys.ethz.ch/engelerp/spartansound)

An FPGA (Spartan 6) defined soundcard. 
It receives wave packets via serial, and drives a speaker via a pin by outputting the corresponding voltage through delta-sigma modulation. 
Continuous playback functionality is enabled by double buffering, one buffer is being played back while new data is being streamed into the other. 

The purpose of this project was mainly knowledge discovery pertaining programming the Spartan 6, using BRAM, communicating via serial, and performing delta-sigma modulation on an FPGA.

A video of the device in operation is shown below.

![SpartanSoundDemo](resources/SpartanSound.mp4)


# Fitbit watchface
**Involved Technologies**: JavaScript, stylesheets

I programmed a watch face for a Fitbit smartwatch. 
While the the face displays lists all the typical data, it also draws a height trace, which shows how the user's height over sea level changed during the past few hours.
This functionality was inspired by a Garmin smartwatch.

Unfortunately the code was lost when Fitbit Studio was shut down, but an impression of the design in operation is shown below.

<img src="resources/fitbit.jpeg" alt="Fitbit Watchface" width="400"/>

# Blackjack multiplayer game [gitlab](only on Synthetic so far)

# Home automation [gitlab](not online yet)

# DLSC Projects [gitlab](https://gitlab.phys.ethz.ch/engelerp/dlsc-tasks)

# Automatic lab monitoring

# Experimental data storage in database

# Foodweb simulations [gitlab](https://gitlab.phys.ethz.ch/engelerp/Foodwebs)

# Framework for automatic topological structure design [](not published yet)

# Dynamic friction simulation[]()

# Texas Hold'em probability analysis []()

# Gameboy emulator []()

# Switchboard [](could do, there's 2 or 3 repos involved in this (pcb, api, firmware))

# Project to automate and optimize study planning for sports research []()

# Project to automate address retrieval from web resources []()