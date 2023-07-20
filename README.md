# StealthMax-Controller
A tophat for the Raspberry Pi Pico W for the Nevermore StealthMax.  

####   THIS IS JUST A PRELIMINARY RELEASE: UNDER CONSTRUCTION, CHECK BACK on 7/30 for completed Readme   ####

Conroller Software can be found here: 
Nevermore StealthMax Project:

Mounts to the Raspberry Pi Pico W, and provides:
  - Mounting of Intake Air Sensors (SGP40 / BME280)
  - Seperate Intake Air Stack to minimize Temp and stale air caused by close proximity (sandwich mounting)
  - Utilizes GH1.25 connectors and wires - highly recommended to utilize precrimped GH1.25's
  - 12V and 5V voltage regulators onboard - 24V input
  - Recommended: MicroFit 3.0 connector for 24V supply, will include link to STL for StealthMax

BOM:
  - Four (4): 1x8 male and female headers (Mounting to Raspberry Pi as a Tophat)
  - Two (2): 1x4 female headers (Intake Air Sensors)
  - Two (2): 1x4 90 degree male pin headers
  - Sensors: SGP40 (x2) BME280 (x2)
  - Fan: 65mm 12V GPU fan (3w)

  - Board Components:
  -   5V VR:
  -   12V VR:
  -   330nf Capacitor x2
  -   100nf Capacitor x2
  -   GH1.25 Board Connectors: (x3)

Gerber File for TopHat Fabrication : Hint: import in to EasyEDA, and you can have 5 board fabricated for $2 or less, just have to pay shipping. 

Board Information:
Input 24Vdc
Max Current: 1A max
5V VR: 300mA
12v VR: 1A

Verify Capacitor Polarity (line on SMD reflects positive anode)
Square Pads: GND
Positive pads are marked with (+)
All connector markings reflect endpoint (SCL, SDA, GND, V, TACH/RPM, CTRL)
