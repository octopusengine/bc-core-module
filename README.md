BigClown Core Module Development Setup
======================================

## Prerequisites

* Clean install of 64-bit (or 32-bit) Ubuntu 16.04 LTS

NOTE: We know it works on macOS and Windows too but description is coming later...

## Steps to install the toolchain

This section will guide you through GCC ARM Embedded toolchain installation on your host system.

#### Open Terminal and add PPA repository

`sudo add-apt-repository ppa:team-gcc-arm-embedded/ppa`

#### Update the package lists:

`sudo apt-get update`

#### Download and install ARM GCC compiler package:

`sudo apt-get install gcc-arm-embedded`

#### Verify that the ARM GCC compiler has installed correctly:

`arm-none-eabi-gcc --version`

You should get this output in Terminal:

	arm-none-eabi-gcc (GNU Tools for ARM Embedded Processors) 6.2.1 20161205 (release) [ARM/embedded-6-branch revision 243739]
	Copyright (C) 2016 Free Software Foundation, Inc.
	This is free software; see the source for copying conditions.  There is NO
	warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

## Steps to build firmware

This section will guide you through the BigClown Core Module firmware build process.

#### Clone BigClown Core Module top-level repository:

`sudo apt-get install git build-essential`

`git clone --recursive https://github.com/bigclownlabs/bc-core-module.git`

#### Build firmware:

`cd bc-core-module`

`make`

#### Check if the file firmware.elf has been created:

`ls -l out`

## Steps to start the debugger

TODO
