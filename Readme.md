# Description of the project
![Schematic]("D:\It's_work\Scope\Scope_evtA\Ver5.PDF")
## Goals:
Learn more about electronics via DIYproject. Technologies which need to be used and learned are: low noise readout electronics, USB as a main data line, space compound. Shielding of pcbs,  wireless connection - additional.

## DIY project:
A portable USB, 1 channel oscilloscope version 1. 

## Activities:
Define Project Requirements;
Conceptualization (diagrams);
Feasibility Study (costs, time);
Define the components for design;
Find and order devboards of the components;
Develop preliminary design of the system;
Prepare and check the schematic;
Order components;
Testing and debugging software;
Prepare and check the pcb layout;
Manufacture the pcb;
Execute test procedure;
Testing and debugging software;
Move to next version of design which includes wireless communication modules;

## Requirements: 
Number of Channels - The oscilloscope should be a single channel.
Bandwidth - The input network bandwidth should support frequencies up to 10 MHz.
Input Impedance - The oscilloscope's input impedance should be 1 MOhm || 15 pF.
Input Signal Range - The acceptable input signal range is -5 V to +5 V.
Time Division -  min. time division of 0.1 us,  max. time 1 seconds.
Vertical Offset - Vertical offset should range from -40 to +40 divisions, with vertical resolution sensitivity set at 40 divisions.
Connector - The oscilloscope should be equipped with a BNC connector for the probes.
ADC Specifications - The ADC resolution > 12 bits, sampling frequency > 10 MHz.
Power Source - The oscilloscope should be powered through a USB Type-A connection.
Display - The device does not have a display. Data shown on a laptop
*Memory Capacity - The oscilloscope's memory capacity should be > 1 MB, TBD, optional*.
Operating Modes - The oscilloscope should support different operating modes, including normal, peak detect, average, and high-resolution modes.


## Design solution
Scope should have a status RGB LED.
Oscilloscope shouldn’t have any user’s buttons or switches
Device should include protection mechanisms against ESD and overloading.
The main processor should be a high performance MCU with maths acceleration functions (ex. STM32G484).
The main ADC should be compatible with pin-to-pin replacements, such as AD9235, ads4122-ads4129, ADC10080 - ADC10040, LTC2245. The ADCs have to have same interface 
Wireless Connectivity - The oscilloscope should include a Wi-Fi chip with support for 802.11n or superior standards.
Components should have minimal footprint.
Pcb needs to be as small as possible, preferable 30 x 20


## Success metrics:
Oscilloscope match the required parameters, technologies are working as estimated


## Reference project
https://www.martinloren.com/hs101-pro-diy-oscilloscope/ 


## Components
Mcu test  
https://eu.mouser.com/ProductDetail/STMicroelectronics/NUCLEO-G474RE?qs=T3oQrply3y%2FWWTZ0gC%252Br%2FA%3D%3D 


## Open questions
https://eu.mouser.com/ProductDetail/STMicroelectronics/STM32G491KCU6?qs=CiayqK2gdcJMDdaGLIKprw%3D%3D controller
https://eu.mouser.com/ProductDetail/Analog-Devices/LTC2225CUHPBF?qs=hVkxg5c3xu%252B3BqQYArDo0w%3D%3D ADC
https://eu.mouser.com/ProductDetail/GigaDevice/GD25D10CEIGR?qs=sGAEpiMZZMs6Aik9Fp479rsGbb%252BA9SG1KaJ9U96nvQw%3D memory
https://eu.mouser.com/ProductDetail/Toshiba/TCR15AG33LF?qs=W0yvOO0ixfEdwQi51FhISQ%3D%3D power
https://eu.mouser.com/ProductDetail/Amphenol-RF/112640?qs=g6wJ%252BjiQWOckvE%2FP9L4wAw%3D%3D connector
https://eu.mouser.com/ProductDetail/Masach/MS110-10S?qs=pUKx8fyJudBF3ymdfEXpvw%3D%3D shielding
https://eu.mouser.com/datasheet/2/609/AD8337-3119375.pdf preamplifier
https://eu.mouser.com/ProductDetail/Inolux/IN-S63TBS5R5G5B?qs=stqOd1AaK7%2Fi2QYkhDu%252BwA%3D%3D rgb led
https://eu.mouser.com/ProductDetail/Hirose-Connector/CX60-24S-UNIT?qs=W0yvOO0ixfHwfoCnP4i0Tw%3D%3D usb type C
https://eu.mouser.com/ProductDetail/Analog-Devices/ADA4830-1WBCPZ-R7?qs=pqQDoYZ2quZZWZQMT6uc6g%3D%3D difference amplifier

## Reference designs
https://www.instructables.com/DPScope-Build-Your-Own-USBPC-Based-Oscilloscope/
https://www.bitscope.com/product/BS05/ 
https://github.com/martinloren/HScope/blob/master/HS402/V3.0%2BWifi/Schematic%26PCB/SCH_HS402-WIFI_V3.1_220108.pdf 
https://hackaday.com/2023/10/18/stm32-offers-performance-gains-for-diy-oscilloscope/ 
https://www.youtube.com/watch?v=cVnVtucYcDg&ab_channel=STMicroelectronics 