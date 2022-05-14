# Requirements #
## Introduction ##
A windscreen wiper or windshield wiper or wiper blade is a device used to remove rain, snow, ice, washer fluid, water from a vehicle's front window.Current car wipers works on the principle of manual switching. The traditional wiper system requires driver's constant attention in adjusting the wiper speed. Traditional windshield wiper speed constantly varies according to time and vehicle’s speed which not only require driver’s attention but also causes a certain level of discomfort to the driver's vision and serves as a source of distraction which increases the risk of accidents.So,to offer comfort to the driver and essentially reduce the risk of accidents, an automatic rain sensing device has become a necessity, as they work to minimize the time of the driver.Automatic rain sensing wiper system detects rain and starts automatically and also stops when the rain stops.

# Requirements for the project #
 ### STM32CubeIDE ### 
 * STM32CubeIDE is an advanced C/C++ development platform with peripheral configuration, code generation, code compilation, and debug features for STM32 microcontrollers and microprocessors. It is based on the Eclipse/CDT framework and GCC toolchain for the development, and GDB for the debugging. It allows the integration of the hundreds of existing plugins that complete the features of the Eclipse IDE.
 ## Xpack Packages ##
 ### Windows Build Tools: ###
* The xPack Windows Build Tools is a standalone Windows binary distribution of GNU make and a few of other tools required by the Eclipse Embedded CDT (formerly GNU MCU/ARM Eclipse) project, but the binaries can also be used in generic build environments.
### OpenOCD ###
* Open On-Chip Debugger (OpenOCD) is a free, open-source project that aims to provide debugging, in-system programming, and boundary scan using a debug adapter. The adapter is a hardware module that provides the right signals for the target to understand.
### QEMU ###
* The xPack QEMU Arm is a standalone cross-platform binary distribution of QEMU, with several extensions for Arm Cortex-M devices.
# Components used in the project #
## STM32F4O7VG Microcontroller board #
The STM32F407 Kit takes advantage of the high-performance STM32F407 microcontrollers' capabilities to make it simple for users to create audio-based applications.It comes with an ST-LINK embedded debug tool, an ST-MEMS digital accelerometer, a digital microphone, an audio DAC with integrated class D speaker driver, LEDs, pushbuttons, and a USB OTG micro-AB connector.Ethernet connectivity, an LCD display, and other features have been added to the STM32F4 DISCOVERY kit. The STM32F405xx and STM32F407xx families are built around the high-performance Arm® Cortex®-M4 32-bit RISC core, which runs at up to 168 MHz.
## Features of STM32F407VG Microcontroller ##
* In a LQFP100 package, the STM32F407VGT6 microcontroller has a 32-bit ARM Cortex-M4 with FPU core, 1-Mbyte Flash memory, and 192-Kbyte RAM.

* On-board ST-LINK/V2 or ST-LINK/V2-A on STM32F4 DISCOVERY (old reference) or STM32F407G-DISC1 (new order code)

* USB ST-LINK with three separate interfaces and re-enumeration capability.

* Virtual Com port Debug port (with new order code only)

* Large-scale storage (with new order code only)

* Board power is supplied through USB or an external 5 V supply source.

* 3 V and 5 V external application power supply.
## Uses of STM32F407VG Microcontroller ##
* This Microcontroller is utilised in printing and scanning machines ,heat ventilation, air conditioning, and security systems.
* This module can be found in a variety of household products.

## Working Principle ##
Assume that the automobile is the microcontroller(STM32F407VG). If the button is pressed , the first led (red) will turn on, Clicking again the wiper will starts , and the second led (blue) will turn on for a desired rate. If the button is pressed again , the third led (green) will turn on, and the wiper's speed will be increased in comparison to the previous one. The fourth press will turn on the fourth led (orange) , and the wiper speed will be increased in accordance with the previous one. The microcontroller (vehicle) is turned off after the fifth click of the button.

# 4W's & 1H # 
## What ##
The operational speed of a vehicle wiper is controlled by a wiper speed control mechanism based on rain conditions. To generate, the control system incorporates a rain sensor (30) that detects rain conditions. The amplitude of an analogue signal depends on the detected rain conditions.
## Why ##
To clean the windscreen clean enough to give adequate view at all times from the front and rear windshields of the car.Wiper cleans the windshield by removing oil, dust, moisture, and grime that have become attached to the glass.
## Who ##
 It is extremely important for drivers of any type of vehicle that require clear road visibility in the event of dust, snow, or rain.
## When ##
When the weather is terrible, such as snow, dust, or rain and so the windshield wipers remove rain and snow from the windshield, while the headlights improve visibility at night.
## How ##
It is implemented using the STM32 microcontroller and once when the rain droplets fall on the windshield of the vehicle.

# Swot Analysis #
## Strengths ##
* Hands-Free Calling.
* Automatically detects rain and wipes the windows by moving the wiper.
* Improve safety by decreasing driver distraction.
* Low Budget.
## Weakness ##
* The rain sensor-based system functions when water falls on the sensor directly.
* Week Focus on Process Innovations.
* Structural Inertia.
## Opportunities ##
* Safety.
* Hands-free calling.
* Emerging New Markets.
## Threats ##
* Low Bargaining Power Buyers.
* Ethical Pressure.
* Once the board repaired cannot be replaced quickly.

# High Level Requirements #
ID	 |  Description	                                                |     Status
-----|--------------------------------------------------------------|-------------------------
HLR-1|	Turn on the Ignition	                                      |   Implemented
HLR-2|	Activating wiper system	                                    |   Implemented
HLR-3|	Controlling the speed of the wiper based on frequency levels|	  Implemented
HLR-4|	Deactivating wiper system	                                  |   Implemented
HLR-5|	Turn off the Ignition	                                      |   Implemented

# Low level Requirements # 

ID	 |  Description	                                                                       |  Status
-----|-------------------------------------------------------------------------------------|--------------------------------------------------------
LLR-1|	Turn on the Microcontroller	                                                       | Implemented
LLR-2|	Press push button for 2secs – RED LED ON	                                         | Implemented
LLR-3|	Press push button for first time - BLUE, GREEN,ORANGE LED’s glow with 1Hz frequency|	Implemented
LLR-4|	Press push button for second time - BLUE,GREEN,ORANGE LED’s glow with 4Hz frequency|	Implemented
LLR-5|	Press push button for third time - BLUE,GREEN,ORANGE LED,s glow with 8Hz frequency |	Implemented
LLR-6|	Press push button for fourth time – ORANGE,GREEN,BLUE LED,s stops glowing	         | Implemented
LLR-7|	Press push button for 2secs – RED LED OFF	                                         | Implemented
