# TinyG-to-2-DM542T-Drives
TinyG to 2 DM542T Driver 12/24V Version

Original Idee was to connect on the TinyG v8 2 external stepperdriver of type DM542T to connect 2 Nema 23 on it. 
Thanks to Carl McGrath

Dokuments: 
Overview_TinyG_DM542T.pdf --> Typical application overview
DM542_PCB.PNG --> PCB view
DM542_PCB_top_Comp_.PNG --> Top View Components
DM542_SCH.PNG --> Schematic view
DM542T_Specification.pdf --> Driver Specification
Eagle_files
  --> DM542T.brd
  --> DM542T.SCH
  --> Eagle.epf
  
Function: 
Connect to tinyg v8 "Step, DIR,ENA" power with 12V from tinyg or 24V to where also the 2 DM542T Drivers are powered. with Jumpers switch Voltage can be be selected. 

Connection:
Connector: xTinyG to TinyG Board 
  12VDC -->  FAN 12VDC
  GND --> GND
  STEP --> STEP (Motor 1...4)
  DIR --> DIR (Motor 1...4)
  ENA --> ENABLE (Motor 1...4)

Connector: 24V1 .. 24V4
  GND --> Powersupply Ground
  24V1 --> Powersupply 24VDC

Connector for Drive 1 and 2:
  Pul+ --> Pul+
  Pul- --> Pul-
  DIR+ --> DIR+
  DIR- --> DIR-
  ENA+ --> ENA+
  ENA- --> ENA-
  
Voltage Selector
  JP12/24 selects the Power Source 12V if powered by TinyG or 24V if Powered with same Powersource like DM542T 
  JP12.1 .. JP12.6 if 12V Powerd from TinyG
  JP24.1 .. JP24.6 if Powered same then DM542T 
  BE AWARE OF: Power Source can only be either 12V or 24V. 
  
