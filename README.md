<img src="https://www.mbed.com/static/img/ARMmbedLogo.svg" width="300" height="" />

# mbed-HDK

The mbed Hardware Development Kit (mbed-HDK) is a collection of hardware design resources built on top of **Eagle PCB** that have been gathered to assist in the development of custom hardware benefiting from the mbed ecosystem, such as mbed OS, mbed SDK and associated technologies such as DAPLink. Working with development boards that were based on the mbed HDK is the most efficient way to get started with the mbed platform.

## Benefits of mbed-HDK

The mbed-HDK provides:

* Extensive collection of Eagle CAD parts libraries.
* Production Design Projects
	* Proven and manufactured mbed platforms for your reference complete with:
		* Eagle Schematic and Board files
		* PDF Schematic and Board copies
		* CAM Job GERBERS for manufacture (including pick/place and drill)
		* BOM (Bill of Materials)
* Bare Design Projects
	* Modular reference blocks of mbed TARGET and INTERFACE chip allowing rapid prototyping complete with:
		* Eagle Schematic and Board files
		* PDF Schematic copies

Please keep in mind that the resources are provided "as is". Though best efforts have been made to ensure the highest possible quality, no support or guarantees can be offered. The latest versions of Production Designs contained in the mbed HDK have been successfully manufactured by a third-party manufacturer and proven to work.

## Getting Started - Setup

The [User Guide](Docs/USER-GUIDE.md) will walk you through the setup to get the most out of the mbed-HDK.

## Getting Started - Your first PCB design
With the mbed-HDK the goal is to allow rapid PCB CAD prototyping for mbed designs, therefore we provide designs to get you started as quickly as possible. There are multiple ways to create your first design.
	
* Starting with a [Production Design Project](https://github.com/ARMmbed/mbed-HDK/tree/master/Production%20Design%20Projects/)
	* Choose this option if you wish to take an existing design that has been manufactured and tested as a starting point, or to make minor changes and then release yourself.

* Starting with a [Bare Design Project](Docs/DESIGN-GUIDE.md)
	* Choose this option if you wish to rapid prototype a design using modular blocks that have already been developed, these modular blocks include DAPLink INTERFACES and mbed TARGETS. For a simple guide to see how this works and how much time it will save.

* Starting with a blank Schematic and Board
	* Choose this option if you wish to utilise only the mbed-HDK tools in your design, this will still allow quick prototyping of mbed designs through using due to the provided mbed-hdk lbr, dru, ulp and CAM

## Moving On - Contributing your parts and designs

If you wish to contribute to the mbed HDK you can do so.

The [Contributors Guide](Docs/CONTRIBUTORS-GUIDE.md) details on how to contribute back to the mbed-HDK. There are 3 possible ways to contribute back to the mbed-HDK.

1. Contributing to mbed-HDK Eagle Libraries
2. Contributing to mbed-HDK Production Design Projects
3. Contributing to mbed-HDK Bare Design Projects
