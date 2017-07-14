# mbed-HDK Contribution Guidlines Libraries

## About

This following guide sets out the needed guidelines for how Eagle parts should be created to be succesfully added to the mbed-HDK

## Before you start
* Before creating a new Eagle part for the mbed-HDK it must not:
	* Be a common discrete part, such as 0402,0603,0805 R, L, C
	* Already exist in the provided libraries

## Step 1 - Create new part in correct library:
* mbed-HDK-Connector
	* USB, Ethernet, Molex picoblade, JST, Pin header …
* mbed-HDK-IC
	* EEPROM, Sensors, Battery management, PHY …
* mbed-HDK-MF-XXXX
   * Manufacture specific SoC
* mbed-HDK-Board
	* Physical board dimensions layouts
* mbed-HDK-Enclosure
	* Physical enclosure dimensions layouts
* mbed-HDK-Silkscreen
    * Silkscreen symbols: CE, Pb free, WEEE.
* mbed-HDK-Symbol
    * Schematic symbols: GND, +3.3V
* mbed-HDK-Template
    * mbed schematic page border
* mbed-HDK-Optical
    * LED
* mbed-HDK-Power
    * LDO, Buck/Boost Converter…
* mbed-HDK-RF
    * Chip Antenna, PCB trace antenna…
* mbed-HDK-RLC
     * Resistors, Inductors, Capacitors, Crystal/Oscillator
* mbed-HDK-Oscillator
     * Crystal/Oscillator
* mbed-HDK-Switch
     * SPST, DPDT, Toggle …
* mbed-HDK-Transistor
     * BJT, MOSFET …
     
## Step 2 - EAGLE PACKAGE guidelines
* Name package according to industrial convention of device, i.e. QFN48
* Include “>NAME” and “>VALUE” on silkscreen. Layers “25 tNames” & “27 tValues” respectively. Size 0.04, Ratio 12%, Vector.
* Include landing dimension silkscreen for device. Layers “21 tPlace”. Width 0.005

## Step 3 - EAGLE SYMBOL guidelines
* Name symbol, either by MFN if unique, or by function if common (i.e. 2-SPST).
* Only be created if suitable symbol not found for part. I.e. SPST switch symbol exists use this instead of creating a new symbol, no duplication.
* Include “&gt;NAME” and “&gt;VALUE”. Layers “95 Names” & “96 Values” respectively. Size 0.07, proportional.

## Step 4 - EAGLE DEVICE guidelines
* Name device by MFN
* Include bolded description. If device unique should describe its characteristics, if device commonly used (i.e. SPST switch) use similar device text as guides.
* Prefix should be included and must be:
    * Switch=SW
    * Jumper=J
    * Connector=CON
    * Integrated Circuit=U
    * Microprocessor=U
    * Diode=D
    * Led=LED
    * Resistor=R
    * Inductor=L
    * Capacitor=C
    * Transistor=T
    * Oscillator=OSC
    * Crystal=Q

* Value = Off
* Include Attributes of: MF, MFN, OC-DIGIKEY, OC-MOUSER, OC-NEWARK.
    * MF=Manufacturer of part, MFN=Manufacturers number of part, OC-=Order code from supplier, all the above must be included (if found from other supplier add OC-XXXXX to attributes, where XXXXX is the supplier)
