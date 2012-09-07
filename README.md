# AVR_ATXMega128A1_Atmel_Studio

FreeRTOS for Atmel Xmega Xplain A1 with Atmel Studio project.

## VersionsXMEGA_A1_XPLAINED_DEMO1

* FreeRTOS 7.2.0
* Atmel Studio 6
* ASF 3.3

## Atmel Studio setup

* Download Atmel Studio 6
* Go to `Tools/Extension Manager`
* Do in this order
 * Update Extension Manager (requires Atmel Studio restart)
 * Update ASF to 3.3
 * (optional?) Update AVRGCC
 * Update Atmel Studio Patch

#Instructions

* Download FreeRTOS 7.2.0
* Place this repository in the Demo directory e.g. Demo/AVR_ATXMega128A1_Atmel_Studio
* run `CreateProjectDirectoryStructure.bat` (copies FreeRTOS files into the AVR_ATXMega128A1_Atmel_Studio directory)

## About

This is a port of FreeRTOS to the XMega Xplain A1. The project includes Atmel Studio project files (msbuild).

This port is based on the Xmega WinAVR port for 6.0.4 available from FreeRTOS Interactive.

## Changes required to produce git version 1:

* Create Atmel Studio file based on XMEGA_A1_XPLAINED_DEMO1
* Use CORTEX_M4_ATSAM4S_Atmel_Studio Demo as a reference for the FreeRTOS Atmel Studio project.
* add sections to Xmega WinAVR 6.0.4 `portmacro.h` file from 7.2.0 port file
* use CORTEX_M4_ATSAM4S_Atmel_Studio Demo ParTest.c with modifications for Xmega

## Motivation

Run FreeRTOS on custom Xmega A3 hardware (Correll Lab honeycomb, etc.).

## Author

&copy; 2012 Charles Dietrich
