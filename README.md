# StealthMax-Controller
A tophat for the Raspberry Pi Pico W for the Nevermore StealthMax.  

####   THIS IS JUST A PRELIMINARY RELEASE: UNDER CONSTRUCTION, CHECK BACK on 7/30 for updated Readme   ####

Conroller Software can be found here: 
Nevermore StealthMax Project:

Mounts to the Raspberry Pi Pico W, and provides:
  - Mounting of Intake Air Sensors (SGP40 / BME280)
  - Seperate Intake Air Stack to minimize Temp and stale air caused by close proximity (sandwich mounting)
  - Utilizes GH1.25 connectors and wires - highly recommended to utilize precrimped GH1.25's
  - 5V voltage regulators onboard - 12V input
  - Recommended: MicroFit 3.0 connector for 24V supply, will include link to STL for StealthMax
  - Utilize whatever 12v powersource you want. I used a microfit 3.0 connector on the bottom of the StealthMax to input 24v to a step-down regulator to 12v. 

BOM:
ID	Name	Designator	Footprint	Quantity	Manufacturer Part	Manufacturer	Supplier	Supplier Part	Price
1	CAP-SMD_L3.2-W1.6-RD	C2,C1	CAP-SMD_L3.2-W1.6-RD	2	CA45-A-35V-0.1UF-K	CEC(振华新云)	LCSC	C2976900	0.063
2	HDR-TH_4P-P2.54-V-F	INTAKE_1,INTAKE_2	HDR-TH_4P-P2.54-V-F	2	2.54-1*4P母	BOOMELE(博穆精密)	LCSC	C2718488	0.043
3	CONN-TH_PH-3A	PWR	CONN-TH_PH-3A	1	PH-3A	CAX(创都)	LCSC	C722771	0.005
4	CONN-SMD_4P-P1.25_HCTL_HC-GH-4PLTKK	FAN,EXHAUST1	CONN-SMD_4P-P1.25_HCTL_HC-GH-4PLTKK	2	HC-GH-4PLT	HCTL(华灿天禄)	LCSC	C3011955	0.09
5	VOC_OUT	NONE,NONE,VOC_OUT,VOC_OUT1		4					
6	SOT-23-5_L3.0-W1.7-P0.95-LS2.8-TL	U1	SOT-23-5_L3.0-W1.7-P0.95-LS2.8-TL	1	MIC5219-5.0YM5-TR	MICROCHIP(美国微芯)	LCSC	C144182	2.262
7	1X8_PIN_HEADER_2.54MM	P21,P22,P23,P24	1X8_PIN_HEADER_2.54MM	4	Z-211-0811-0021-001	Nextron	LCSC	C190820	0.052

  - Board Components:
  -   5V VR: 
  -   12V VR:
  -   330nf Capacitor x2
  -   100nf Capacitor x2
  -   GH1.25 Board Connectors: (x3)

Gerber File for TopHat Fabrication : Hint: import in to EasyEDA, and you can have 5 board fabricated for $2 or less, just have to pay shipping. 

Board Information:
Input 12Vdc
5V VR: 300mA

Verify Capacitor Polarity (line on SMD reflects positive anode)
Square Pads: GND
Positive pads are marked with (+)
All connector markings reflect endpoint (SCL, SDA, GND, V, TACH/RPM, CTRL)

Easiest method to get the board:
  - Create an EasyEDA account @ https://easyeda.com/
  - Use the Standard Online Editor
  - File - Open - EasyEDA, and select the stealthMax Top hat file
  - You will have to save it as a project, and then, click File "Generate PCB Generation File (Gerber)
  - It will open a window to order the boards through JLCPCB. All parts should be in stock, and should cost about $40 for 5 boards. Coupons will be available at checkout to make it even cheaper.

  - Good Luck, and find me on Discord if you have any questions. 
  - New Project - Import
