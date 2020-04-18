# Web App Site Control
A tailor made Home Automation & Information System with a WebUI for use with smartphones.

### Purpose
To create a Home Automation & Information System, running on a Raspberry Pi 3B+, accessible via a browser-based application (WebUI) for use mainly (but not only) with smartphones.

**Requirements**

* Easy-to-use User Interface (WebUI, in German) accessible from any device capable running a browser - smartphones [target device], tablets, PC, SBC, TV.
* WebUI with Tabs & Groups organised by function Heating ("Heizung"), Lights ("Lampen"), Climate ("Klima"), Switches ("Schalter"), Information ("Info").
* Devices integrated like Thermostats (Homematic IP), Philips Hue Lights, Outdoor Weather sensors (RFXCOM), Energy consumption (Meters), Switches (Homematic IP) etc.

### Solution
* built with [Node-RED](https://nodered.org/) and additional nodes
* additional nodes are used to communicate with external devices or create the WebUI (Dashboard).
* split into functions, which are represented in the WebUI (German) by Tabs with Groups - each having its own flow.
* created for **private use only**. To adapt for own purposes, it will need a deep dive into the various flows.
* ment as an experiment & trigger for ideas or suggestion building a Home Automation & Information System.
* is _developed further_ - working title **WASC**.

#### WebUI with additional information of the functions
![wasc-ui](https://user-images.githubusercontent.com/47274144/79632673-29201280-8161-11ea-9b79-02f5cb0f99eb.png)

#### Topology with HTTP API requests between Node-RED and subsystems.
![wasc-topology](https://user-images.githubusercontent.com/47274144/79632672-29201280-8161-11ea-90fe-257009ab8efc.png)

#### Flows of the functions = just as an illustration.
![wasc-flows](https://user-images.githubusercontent.com/47274144/79632671-28877c00-8161-11ea-975f-a91ef5f6ad84.png)

### Documentation
The folder **flows** contain the Node-RED flows & subflows (formatted). Use the Node-RED import function to import as new flow.
_IN PROGRESS_ (not shared yet): PDF document **webapp-sitecontrol.pdf** describing the solution and concept.

### Software Versions
_(The versions are subject to change as keeping to the latest versions)_
* Linux: 4.19.66-v7+ #1253
* Node-RED: 1.0.5, node-red-dashboard 2.20.0, node-red-contrib-bme280 1.0.0, node-red-contrib-rfxcom 2.10.0

### Credits
To the developers of Node-RED & additional flows and to all sharing related information.
Without these, it would not be possible to build this project.

### Disclaimer
THIS SOLUTION IS PROVIDED BY THE AUTHOR “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. 
IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, 
PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, 
STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
