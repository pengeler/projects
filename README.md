# List of Projects
The following is a list of projects that I have worked on, along with brief descriptions and involved technologies. 

Due to nontrivial source licences, access to sourcecode will be provided on a per-request basis, where possible.

- [List of Projects](#list-of-projects)
  - [Wave simulator gitlab](#wave-simulator-gitlab)
  - [Simulation framework for system of thousands of coupled resonators gitlab](#simulation-framework-for-system-of-thousands-of-coupled-resonators-gitlab)
  - [Autonomous temperature stabilization system gitlab](#autonomous-temperature-stabilization-system-gitlab)
  - [FPGA lock-in amplifier gitlab](#fpga-lock-in-amplifier-gitlab)
  - [High performance interference ray tracer gitlab](#high-performance-interference-ray-tracer-gitlab)
  - [RBComb control system \[gitlab\](Bridge with RAM only)](#rbcomb-control-system-gitlabbridge-with-ram-only)
  - [PCB generation framework gitlab](#pcb-generation-framework-gitlab)
  - [RBComb sample visualizer gitlab](#rbcomb-sample-visualizer-gitlab)
  - [Interactive MEMS resonator design optimizer gitlab](#interactive-mems-resonator-design-optimizer-gitlab)
  - [Interactive WLI data analyzer and visualizer gitlab](#interactive-wli-data-analyzer-and-visualizer-gitlab)
  - [Labbook generator gitlab](#labbook-generator-gitlab)
  - [Git diff gitlab](#git-diff-gitlab)
  - [FPGA defined FM transmitter gitlab](#fpga-defined-fm-transmitter-gitlab)
  - [FPGA defined soundcard gitlab](#fpga-defined-soundcard-gitlab)
  - [Fitbit watchface gitlab](#fitbit-watchface-gitlab)
  - [Blackjack multiplayer game gitlab](#blackjack-multiplayer-game-gitlab)
  - [Home automation gitlab](#home-automation-gitlab)
  - [DLSC Projects gitlab](#dlsc-projects-gitlab)
  - [Automatic lab monitoring](#automatic-lab-monitoring)
  - [Experimental data storage in database](#experimental-data-storage-in-database)
  - [Foodweb simulations ](#foodweb-simulations-)
  - [Framework for automatic topological structure design ](#framework-for-automatic-topological-structure-design-)
  - [Dynamic friction simulation](#dynamic-friction-simulation)
  - [Texas Hold'em probability analysis ](#texas-holdem-probability-analysis-)
  - [Gameboy emulator ](#gameboy-emulator-)
  - [Switchboard ](#switchboard-)
  - [Project to automate and optimize study planning for sports research ](#project-to-automate-and-optimize-study-planning-for-sports-research-)
  - [Project to automate address retrieval from web resources ](#project-to-automate-address-retrieval-from-web-resources-)


## Wave simulator [gitlab](https://gitlab.phys.ethz.ch/engelerp/framebuffer-testing)

## Simulation framework for system of thousands of coupled resonators [gitlab](https://gitlab.phys.ethz.ch/engelerp/rbcomb-simulation)

## Autonomous temperature stabilization system [gitlab](https://gitlab.phys.ethz.ch/engelerp/rbcomb-temperature-control)

## FPGA lock-in amplifier [gitlab](https://gitlab.phys.ethz.ch/engelerp/stitch)

## High performance interference ray tracer [gitlab](https://gitlab.phys.ethz.ch/engelerp/rbcomb-ray-tracer)
The goal of this project was writing a program that can predict interference patterns seen in a microscope, for certain configurations of deformed overlapping thin films. The motivation of this project was sparked by a lack of understanding of observed results in the cleanroom. 

The ray tracer is parallelized using OpenMP and was run on a cluster (Piz Daint). As opposed to conventional ray tracers, here rays of several different colours are traced through materials with nontrivial curvatures and refractive indices. The results were able reproduce observations, and guided us in the right direction for the resolution of the observed issues.

**Technologies**: C++, OpenMP, python

## RBComb control system [gitlab](https://gitlab.phys.ethz.ch/engelerp/bridge_fpga_ram)

## PCB generation framework [gitlab](https://gitlab.phys.ethz.ch/code/experiment/rbcomb-breakout)
Contains classes to represent Kicad pcbs, along with scripts that use these classes to generate different versions of Breakoutboards.

## RBComb sample visualizer [gitlab](https://gitlab.phys.ethz.ch/engelerp/rbcomb-sample-visualizer)

## Interactive MEMS resonator design optimizer [gitlab](https://gitlab.phys.ethz.ch/engelerp/arm-designer)

## Interactive WLI data analyzer and visualizer [gitlab](https://gitlab.phys.ethz.ch/engelerp/nt1100-analyser)

## Labbook generator [gitlab](can't, contains private information, but offer to clean up)

## Git diff [gitlab](https://gitlab.phys.ethz.ch/engelerp/gitdiff)

## FPGA defined FM transmitter [gitlab](not online yet)

## Spartan Sound [gitlab](https://gitlab.phys.ethz.ch/engelerp/spartansound)
An FPGA (Spartan 6) defined soundcard. 
It receives wave packets via serial, and drives a speaker via a pin by outputting the corresponding voltage through delta-sigma modulation. 
Continuous playback functionality is enabled by double buffering, one buffer is being played back while new data is being streamed into the other. 

The purpose of this project was mainly knowledge discovery pertaining programming the Spartan 6, using BRAM, communicating via serial, and performing delta-sigma modulation on an FPGA.

A video of the device in operation is shown below.

![SpartanSoundDemo](resources/SpartanSound.mp4)


## Fitbit watchface [gitlab]()

## Blackjack multiplayer game [gitlab](only on Synthetic so far)

## Home automation [gitlab](not online yet)

## DLSC Projects [gitlab](https://gitlab.phys.ethz.ch/engelerp/dlsc-tasks)

## Automatic lab monitoring

## Experimental data storage in database

## Foodweb simulations [gitlab](https://gitlab.phys.ethz.ch/engelerp/Foodwebs)

## Framework for automatic topological structure design [](not published yet)

## Dynamic friction simulation[]()

## Texas Hold'em probability analysis []()

## Gameboy emulator []()

## Switchboard [](could do, there's 2 or 3 repos involved in this (pcb, api, firmware))

## Project to automate and optimize study planning for sports research []()

## Project to automate address retrieval from web resources []()