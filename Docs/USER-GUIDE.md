# mbed-HDK User Guide

## About

The User Guide is simply used to enable user who just wishes to use the tools provided, without fuss, cloning repositories or needing to contribute.

## mbed-HDK Setup

The mbed-HDK utilises Eagle PCB CAD tool for development. The following details the steps to Install Eagle PCB and how to add the mbed-HDK tools to Eagle to allow rapid development of mbed projects.

Install the necessary tools listed below. Skip any step where a compatible tool already exists.

**Step 1.** Eagle PCB

1. Install [Eagle PCB](https://www.autodesk.com/products/eagle/overview) 

**Step 2.** Download mbed-HDK

1. Download latest zip [here](https://github.com/ARMmbed/mbed-HDK/archive/master.zip)
2. Unzip to $HOME

**Step 3.** Add mbed-HDK tools to Eagle Directories

1. Open Eagle, select Control Panel window
2. Click Options, Directories
3. Change Libraries to:
	* `$EAGLEDIR\lbr;$HOME\mbed-HDK-master/Eagle Tools/lbr` (Windows)
	* `$EAGLEDIR/lbr:$HOME/mbed-HDK-master/Eagle Tools/lbr` (OS X)
4. Change Design Rules to:
	* `$EAGLEDIR\lbr;$HOME\mbed-HDK-master/Eagle Tools/dru` (Windows)
	* `$EAGLEDIR/lbr:$HOME/mbed-HDK-master/Eagle Tools/dru` (OS X)
5. Change User Language Programs to:
	* `$EAGLEDIR\lbr;$HOME\mbed-HDK-master/Eagle Tools/ulp` (Windows)
	* `$EAGLEDIR/lbr:$HOME/mbed-HDK-master/Eagle Tools/ulp` (OS X)
6. Change CAM Jobs to:
	* `$EAGLEDIR\lbr;$HOME\mbed-HDK-master/Eagle Tools/cam` (Windows)
	* `$EAGLEDIR/lbr:$HOME/mbed-HDK-master/Eagle Tools/cam` (OS X)
	


