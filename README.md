# PCB-Lithium-shield

This is my personal backup for a wemos Lithium battery shield with battery protection. Feel free to use and improve on design. Some quick tips for improvement:
- Ground plane
- Shrink the design further with smd
- Use potentiometers to be flexibile on cutoff voltage.

## What is this?
This design is for an 'shield' which fits onto a wemos esp8266/esp32 device and adds the possibility to use unprotected Lithium batteries. The MAX931CPA-DIP8 includes build in reference voltage and hysterisis to drive the enable pin of the LDO Linear regulator (MCP1825). This creates (depending on resistor configuration) for an automatic cut-off of the battery when the voltage drops to low. I found that long term battery powered projects get 'forgotten' causing deep discharges to damage the batteries. The housing and physical mounting did not allow for protected 18650 cells due to a slight increase in length. 

## Why I made this
I needed a shield that would allow me to use an unprotected lithium battery with my wemos(ESP8266/ESP32) powered projects. I had a large amount of MCP1825-3302EAT devices which being LDO Linear did make for an easy option. Since the project required the devices to be in deep sleep 99% of the time, efficieny wasn't a big deal. 

## What does this repository contain
The following files can be found and used to your hearts content!:
- [PCB design](PCB_PCB_Lithium-wemos-shield.json)
- [Schematic](Schematic_Lithium-wemos-shield.json)
- [Bill of Materials (BOM)](BOM_Lithium-wemos-shield.xlsx)

Lithium battery shield with linear ldo and battery protection 3.5v  