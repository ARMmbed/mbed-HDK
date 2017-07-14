# mbed-HDK Contribution Guidelines Production Design Projects

## About

This following guide sets out the needed guidelines for how production projects designed within Eagle can be added to our mbed-HDK.

## Step 1 - Must follow directory layout
* “mbed-HDK/Production Design Projects/YourCompanyHere/YourNewProject/vX.X.X”
	* Where “YourCompanyHere” is the desired referenced name of the company submitting
	* Where “YourNewProject” is the desired referenced name of the project
	* Where “vX.X.X” is the version of design files contained, previous versions should always be kept. When creating a new version, do not overwrite older versions.

## Step 2 - Include “readme.md”
* Located in “mbed-HDK/Production Design Projects/YourCompanyHere/YourNewProject/”
* Written in markdown and includes:
	* Short description
		* A brief outline of what the design is, with image.
	* “Whats included here?”
		* Outlining what is included within the files.
	* “Hardware”
		* Features of the hardware
	* “eBOM”
		* Online Bill of Materials (BOM) through Octopart
	* “Software and more info”
		* Relevant links to the firmware for the device
	* “How to get hardware”
		* Relevant links to purchase or manufacturer device
	* “Revisions”
		* List Revisions and their changes.

## Step 3 - Include all design files
* Located in “mbed-HDK/Production Design Projects/YourCompanyHere/YourNewProject/vX.X.X”
* Eagle schematic and board files.
	* YourNewProject-V_X_X_X.sch
	* YourNewProject-V_X_X_X.brd
* Eagle schematic and board PDF
	* YourNewProject-V_X_X_X-BRD.pdf
	* YourNewProject-V_X_X_X-SCH.pdf
* Bill of Materials (BOM)
	* Generated via “mbed-HDK/Eagle Tools/ulp/mbed-HDK-BOM”, list by “Value”, export CSV.
	* YourNewProject-V_X_X_X-BOM.xlsx

## Step 4 - Include all production files
* Located in “mbed-HDK/Production Design Projects/YourCompanyHere/YourNewProject/GERBERS”
* Generate CAM Gerbers for PCB production
	* All Gerbers generated via mbed CAM jobs “mbed-HDK/Eagle Tools/cam”
* Pick and Place mount files
	* .mnt & .mnb generated via “mbed-HDK/Eagle Tools/ulp/mountsmd.ulp”
