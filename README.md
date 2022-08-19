---
page_type: sample
description: "This filter is a transaction-aware file scanner that examines data in files."
languages:
- cpp
products:
- windows
- windows-wdk
---

# AvScan File System Minifilter Driver

The AvScan minifilter is a transaction-aware file scanner. This is an example for developers who intend to write filters that examine data in files. Typically, anti-virus products fall into this category.

## Universal Windows Driver Compliant

This sample builds a Universal Windows Driver. It uses only APIs and DDIs that are included in OneCoreUAP.

## How to run this scanner?

1. Build this project in visual studio
2. Download and run OSRLoader as administrator
3. [Optional] For debugging download and configure WinDBG
4. In OSRLoader, select the scanner.dll file, set the Type to Mini-filter and Altitude to 371001
5. Click Register Service and Start Service

## How to run User mode/neehackavuser?

1. Make sure neehackav is running
2. Build this project and open it as administrator
3. create a .txt file anywhere in your PC named "virus.txt" and open it.
4. Neehackav should prevent your open event and pop and error since it is considered suspicious.

![neehackav](https://user-images.githubusercontent.com/104021378/185527821-77bf4255-d959-4381-8259-5dcab8625af7.jpg)
