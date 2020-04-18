# Web App Site Control
A tailor made Home Automation & Information System with a WebUI for use with smartphones.

### Purpose
To create a Home Automation & Information System, running on a Raspberry Pi 3B+, accessible via a browser-based application (WebUI) for use mainly (but not only) with smartphones.

**Requirements**

* Easy-to-use User Interface (WebUI, in German) accessible from any device capable running a browser - smartphones [target device], tablets, PC, SBC, TV.
* WebUI with Tabs & Groups organised by function Heating ("Heizung"), Lights ("Lampen"), Climate ("Klima"), Switches ("Schalter"), Information ("Info").
* Devices integrated like Thermostats (Homematic IP), Philips Hue Lights, Outdoor Weather sensors (RFXCOM), Energy consumption (Meters), Switches (Homematic IP) etc.

### Solution
* built with [Node-RED](https://nodered.org/) and additional nodes.
* additional nodes are used to communicate with external devices or create the WebUI (Dashboard).
* modular approach, split into functions, represented in the WebUI several Tabs with Groups - each having its own flow.
* MQTT interface to control or use the data by other systems, i.e. the WASC-BOX (a custom digital Lego creation displaying data).
* created for **private use only**. To adapt for own purposes, it will need a deep dive into the various flows.
* ment as an experiment & trigger for ideas or suggestion building a Home Automation & Information System.
* being _developed further_ [more functions] - working title **WASC**.
* running smooth since Q4'2019.

#### WebUI with additional information of the functions
![wasc-ui](https://user-images.githubusercontent.com/47274144/79632673-29201280-8161-11ea-9b79-02f5cb0f99eb.png)

#### Topology with HTTP API requests between Node-RED and subsystems
![wasc-topology](https://user-images.githubusercontent.com/47274144/79632672-29201280-8161-11ea-90fe-257009ab8efc.png)

#### Flows of the functions = just as an illustration
![wasc-flows](https://user-images.githubusercontent.com/47274144/79632671-28877c00-8161-11ea-975f-a91ef5f6ad84.png)

#### WASC-Box
Fun project, which is a custom LEGO® creation displaying WASC data and control functions (LEGO is a trademark of the LEGO Group). Hardware: Raspberry Pi Zero W, LCD2004 display, 4 Pushbuttons. Software: Node-RED.

_Note_: Solution not finalized - work in progress on push-button handling & integrating LEDs. The initial solution displays climate data (MQTT) and a clock. The green push-button sets the setpoint of a Homematic IP thermostat, the white push-button shuts the Raspberry Pi down.

![wasc-box](https://user-images.githubusercontent.com/47274144/79644032-87bbaf80-81a6-11ea-94b5-c56f0894e807.png)

### Documentation
The folder **flows** contain the Node-RED flows & subflows (formatted). Use the Node-RED import function to import as new flow.
_IN PROGRESS_ (not shared yet): PDF document **webapp-sitecontrol.pdf** describing the solution and concept more in detail.

### Software Versions
_(The versions are subject to change as keeping to the latest versions)_
* Linux: 4.19.66-v7+ #1253
* Node-RED: 1.0.5
* Additional nodes: node-red-dashboard 2.20.0, node-red-contrib-bme280 1.0.0, node-red-contrib-rfxcom 2.10.0, node-red-contrib-lcd20x4-i2c 0.1.1 (used by the WASC-Box).

### Credits
To the developers of Node-RED & additional nodes & flows and to all sharing related information.
Without these, it would not be possible to create this project.

### License
This project is licensed under the GNU GENERAL PUBLIC LICENSE Version 3 - see the LICENSE file for details.
