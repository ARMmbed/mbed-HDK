# mbed-HDK Contributors Guide

## About

The Contributors Guide is an extension of the User Guide, this details on how to contribute back to the mbed-HDK. There are 3 possible ways to contribute back to the mbed-HDK.

1. Contributing to mbed-HDK **Eagle Libraries**
2. Contributing to mbed-HDK **Production Design Projects**
3. Contributing to mbed-HDK **Bare Design Projects**

## mbed-HDK Contributors Setup

The mbed-HDK utilises Eagle PCB CAD tool for development. The following details the steps to Install Eagle PCB and how to add the mbed-HDK tools to Eagle to allow rapid development of mbed projects.

Install the necessary tools listed below. Skip any step where a compatible tool already exists.

**Step 1.** Prerequisites

1. Install [Eagle PCB](https://www.autodesk.com/products/eagle/overview) 
2. Install [Git](https://git-scm.com/downloads) Add to PATH.

**Step 2.** Fork the mbed-HDK source

* See for [guide](https://help.github.com/articles/fork-a-repo/)

**Step 3.** Clone the mbed-HDK source

```
$ cd $HOME 
$ git clone https://github.com/YOURUSERNAME/mbed-HDK.git
$ git remote add upstream https://github.com/ARMmbed/mbed-HDK.git
```
**Step 4.** Add mbed-HDK tools to Eagle Directories

1. Open Eagle, select Control Panel window
2. Click Options, Directories
3. Change Libraries to:
	* `$EAGLEDIR\lbr;$HOME\mbed-HDK/Eagle Tools/lbr` (Windows)
	* `$EAGLEDIR/lbr:$HOME/mbed-HDK/Eagle Tools/lbr` (OS X)
4. Change Design Rules to:
	* `$EAGLEDIR\lbr;$HOME\mbed-HDK/Eagle Tools/dru` (Windows)
	* `$EAGLEDIR/lbr:$HOME/mbed-HDK/Eagle Tools/dru` (OS X)
5. Change User Language Programs to:
	* `$EAGLEDIR\lbr;$HOME\mbed-HDK/Eagle Tools/ulp` (Windows)
	* `$EAGLEDIR/lbr:$HOME/mbed-HDK/Eagle Tools/ulp` (OS X)
6. Change CAM Jobs to:
	* `$EAGLEDIR\lbr;$HOME\mbed-HDK/Eagle Tools/cam` (Windows)
	* `$EAGLEDIR/lbr:$HOME/mbed-HDK/Eagle Tools/cam` (OS X)
	
## How to Contribute: Libraries
If you wish to contribute Eagle parts to one of the provided mbed-HDK-xxxx libraries in this repository you can do.

1. Refer to the [How to Contribute Guidelines: Libraries guide](CONTRIBUTION-GUIDELINES-LIBRARIES.md)
2. Pull the lastest upstream from ARMmbed/mbed-HDK

```
$ git checkout master
$ git pull upstream master && git push origin master
```
3. Create new branch 

```
$ git checkout -feature/MYCHANGES
``` 

4. Create Pull Request

```
 $ git push -u origin lbr/MYCHANGES
``` 
5. Navigate to your fork on GitHub.com, select " "Compare & pull request" button"

## How to Contribute: Production Design Projects
If you wish to contribute one of your own Production Design Projects to our HDK for others to use open source you can do.

1. Refer to the [How to Contribute Guidelines: Production Design Projects guide](CONTRIBUTION-GUIDELINES-PRODUCTION-DESIGN-PROJECTS.md)
2. Pull the lastest upstream from ARMmbed/mbed-HDK

```
$ git checkout master
$ git pull upstream master && git push origin master
```
3. Create new branch 

```
$ git checkout -feature/MYCHANGES
``` 

4. Create Pull Request

```
 $ git push -u origin pdp/MYCHANGES
``` 
5. Navigate to your fork on GitHub.com, select " "Compare & pull request" button"

## How to Contribute: Bare Design Projects
If you wish to contribute devices one of your own Bare Design Projects to our HDK for others to use open source you can do.

1. Refer to the [How to Contribute Guidelines: Bare Design Projects guide](CONTRIBUTION-GUIDELINES-BARE-DESIGN-PROJECTS.md)
2. Pull the lastest upstream from ARMmbed/mbed-HDK

```
$ git checkout master
$ git pull upstream master && git push origin master
```
3. Create new branch 

```
$ git checkout -feature/MYCHANGES
``` 

4. Create Pull Request

```
 $ git push -u origin bdp/MYCHANGES
``` 
5. Navigate to your fork on GitHub.com, select " "Compare & pull request" button"


