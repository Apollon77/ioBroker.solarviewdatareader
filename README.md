![Logo](admin/solarviewdatareader.png)
# ioBroker.solarviewdatareader

![Number of Installations](http://iobroker.live/badges/solarviewdatareader-installed.svg) 
![Number of Installations](http://iobroker.live/badges/solarviewdatareader-stable.svg)
[![NPM version](http://img.shields.io/npm/v/iobroker.solarviewdatareader.svg)](https://www.npmjs.com/package/iobroker.solarviewdatareader)
[![Downloads](https://img.shields.io/npm/dm/iobroker.solarviewdatareader.svg)](https://www.npmjs.com/package/iobroker.solarviewdatareader)
[![Dependency Status](https://img.shields.io/david/afuerhoff/iobroker.solarviewdatareader.svg)](https://david-dm.org/afuerhoff/iobroker.solarviewdatareader)
[![Known Vulnerabilities](https://snyk.io/test/github/afuerhoff/ioBroker.solarviewdatareader/badge.svg)](https://snyk.io/test/github/afuerhoff/ioBroker.solarviewdatareader)

[![NPM](https://nodei.co/npm/iobroker.solarviewdatareader.png?downloads=true)](https://nodei.co/npm/iobroker.solarviewdatareader/)

**Tests:**: [![Travis-CI](http://img.shields.io/travis/afuerhoff/ioBroker.solarviewdatareader/master.svg)](https://travis-ci.org/afuerhoff/ioBroker.solarviewdatareader)

## solarviewdatareader adapter for ioBroker

The adapter reads the data from the Solarview data logger.
Here you can find additional infos about Solarview: https://www.solarview.info/solarlogger.aspx


## Configuration

### IP address, Port
To get the data from the datalogger you must enter the ip-address and the port. The standard port is 15000. Please refer to the Solarview documentation.

### D0 converter
If you have a D0 converter connected to the Solarview data logger you can enable this option.

### Self consumption meter sum and 1 to 4
If you have a S0 meter, you can enable this option. 
You can have up to 4 self consumption meters and the sum from all meters.

### Inverter 1 to 4
Every inverter you can enable separately. 

### Interval, interval start, interval end
Here you can configure the time range and the interval.

### Set system variable CCU, System variable
This ist a special feature for the homematic CCU. You can define a system variable in the CCU.
In this system variable the actual PAC value is saved.

## Changelog
<!--
	Placeholder for the next version (at the beginning of the line):
	### __WORK IN PROGRESS__
-->
### __WORK IN PROGRESS__
* (afuerhoff) dependencies updated

### 0.2.1
* (afuerhoff) self consumption meter optimized
### 0.2.0
* (afuerhoff) Error handling optimized, self consumption meter implemented
### 0.1.0
* (afuerhoff) optimizations for adding to latest repository
### 0.0.5
* (afuerhoff) Code optimized, unload optimized, documentation added 
### 0.0.4
* (afuerhoff) Objects, Telnet client and checksum calculation changed
### 0.0.3
* (afuerhoff) inverter selection added
### 0.0.2
* (afuerhoff) test version
### 0.0.1
* (afuerhoff) initial release

## License
MIT License

Copyright (c) 2019-2021 Achim Fürhoff <achim.fuerhoff@outlook.de>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.