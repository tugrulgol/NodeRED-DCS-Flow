# Node-RED Flow for Detector Control System (DCS)

This repository contains the Node-RED flow used in the master’s thesis entitled:

**"Design of a Detector Control System (DCS) for Nuclear Instrumentation in Experimental Particle Physics"**

## Description

The flow processes two primary sensor data streams (`sensor1/data`, `sensor2/data`) and one error channel (`sensor/error`). It includes the following functionalities:

- Real-time data visualization via `chart` and `gauge` nodes
- Rule-based automation using `function`, `switch`, and `mqtt` nodes
- Control commands published to dedicated topics:
  - `sensor1/control`: controls the data flow from **sensor 1 only**
  - `sensor2/control`: controls the data flow from **sensor 2 only**
  - `sensor/control`: used to control the data flow from **both sensors simultaneously**
- Error detection and notification through filtering and email alerts


## Usage

To import the flow into your Node-RED environment:

1. Open your Node-RED editor.
2. Go to the menu → *Import* → *Clipboard*.
3. Paste the contents of the `flows.json` file.
4. Click *Deploy* to activate the flow.

Editor: Tuğrul Göl
Istinye University Computer Engineering Master's Thesis
