# Web App Site Control (WASC)
A tailor made Home Automation & Information System with a WebUI for use with smartphones.

### Purpose
To create a Home Automation & Information System, running on a Raspberry Pi 3B+, accessible via a browser-based application (WebUI) for use with smartphones.

**Requirements**

* Easy-to-use User Interface (WebUI, in German) accessible from any device capable running a browser - smartphones [target device], tablets, PC, SBC, TV.
* WebUI with Tabs & Groups organised by function Heating ("Heizung"), Lights ("Lampen"), Climate ("Klima"), Switches ("Schalter"), Information ("Info").
* Devices integrated like Homematic IP Thermostats, Philips Hue, Outdoor Weather sensors (RFXCOM), Energy consumption (Meters), Switches (Homematic IP) etc.

### Solution
* The application is build with [Node-RED](https://nodered.org/) and additional nodes - recommend to visit the Node-RED homepage to explore more.
* The flow is split into functions, which are represented in the WebUI (German) by Tabs with Groups - each having its own flow.
* The Node-RED additional nodes are used to communicate with external devices or create the WebUI (Dashboard).
* The solution has been developed for **private use only**. To adapt for own purposes, it will need a deep dive into the various flows.
* Is ment as a trigger for ideas or as a suggestion building a Home Automation & Information System.

**Screenshots**, with additional information of the various functions. 

**Topology** with HTTP API requests between Node-RED and subsystems.

**Screenshot** of the various flows = just as an illustration.

### Documentation
The files starting with **wasc** contains the Node-RED flows & subflows (formatted). Use the Node-RED import function to import as new flow.
The solution is being _developed further_.
IN PROGRESS (not shared yet): PDF document **webapp-sitecontrol.pdf** describing the solution and concept.

### Software Versions
(The versions are subject to change as keeping to the latest versions)
Linux: 4.19.66-v7+ #1253
Node-RED: 1.0.5, node-red-dashboard 2.20.0, node-red-contrib-bme280 1.0.0, node-red-contrib-rfxcom 2.10.0

### Credits
To the developers of Node-RED & additional flows and to all sharing related information.
Without these, it would not be possible to build this project.

### Disclaimer
THIS DOCUMENT IS PROVIDED BY THE AUTHOR “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. 
IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, 
PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, 
STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
