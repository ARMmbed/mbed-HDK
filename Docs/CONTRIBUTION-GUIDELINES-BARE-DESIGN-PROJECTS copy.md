# mbed-HDK Contribution Guidelines Bare Design Projects

## About

This following guide sets out the needed guidelines for how bare design projects designed within Eagle can be added to our mbed-HDK.

## Step 1 - Must follow directory layout
* “mbed-HDK/Bare Design Projects/YourCompanyHere/Type/YourNewProject/”
	* Where “YourCompanyHere” is the desired referenced name of the company submitting
	* Where "Type" is "TARGET" or "INTERFACE" 
	* Where “YourNewProject” is the desired referenced name of the project

## Step 2 - Include specific design files
* Located in “mbed-HDK/Production Design Projects/YourCompanyHere/Type/YourNewProject/vX.X.X”
* Eagle schematic and board files.
	* YourNewProject-V_X_X_X.sch
	* YourNewProject-V_X_X_X.brd
* Eagle schematic PDF
	* YourNewProject-V_X_X_X-SCH.pdf

## Step 3A - Design Requirements if 'Type' 'TARGET'
1. Include Target module/circuit with minimum bring up components for function
2. Layers
	* Layer 1 - Polygon fill generously surronding whole design, named "GND"
	* Layer 16 - Polygon fill generously surronding whole design, named "+3.3V"
	* Layer 20 - Dimension draw **not** included around design.
3. Pin Names
	* In schematic design Target **must** have the following Net Names 
	* In board design Target **must** route out the traces of the following Net Names to allow easy accesibility for end user, see examples.

		| TARGET Pin | Schematic Net Name |
		|------------|--------------------|
		| VCC        | +3.3V              |
		| GND        | GND                |
		| SWCLK      | TGT_SWCLK          |
		| SWDIO      | TGT_SWDIO          |
		| NRESET     | TGT_NRESET         |
		| UART TX    | TGT_TX             |
		| UART RX    | TGT_RX             |

	
## Step 3B - Design Requirements if 'Type' 'INTERFACE'
1. Include Interface module/circuit with minimum bring up components for function.
2. Include micro USB
3. Include 5V to 3.3V regulator
4. Include switch 'RESET' tied to NRESET
5. Include 3 GPIO LEDs for PWR(RED), DAP(BLUE), COM(GREEN) LEDs, see example.
6. Layers
	* Layer 1- **No** Polygon fill generously surronding whole design, named "GND"
	* Layer 16 - **No** Polygon fill generously surronding whole design, named "+3.3V"
	* Layer 20 - Dimension draw **not** included around design.
7. Pin Names
	* In schematic design Interface **must** have the following Net Names 
	* In board design Interface **must** route out the traces of the following Net Names to allow easy accesibility for end user, see examples.

		| INTERFACE Pin | Schematic Net Name |
		|---------------|--------------------|
		| VCC           | +3.3V              |
		| GND           | GND                |
		| SWCLK         | TGT_SWCLK          |
		| SWDIO         | TGT_SWDIO          |
		| NRESET        | TGT_NRESET         |
		| USB D+        | TGT_USB_D+         |   
		| USB D-        | TGT_USB_D-         |
		| UART TX       | TGT_RX             |
		| UART RX       | TGT_TX             |



