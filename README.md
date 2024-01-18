![Logo](admin/solarviewdatareader.png)
# ioBroker.solarviewdatareader

[![NPM version](https://img.shields.io/npm/v/iobroker.solarviewdatareader.svg)](https://www.npmjs.com/package/iobroker.solarviewdatareader)
[![Downloads](https://img.shields.io/npm/dm/iobroker.solarviewdatareader.svg)](https://www.npmjs.com/package/iobroker.solarviewdatareader)
![Number of Installations (latest)](https://iobroker.live/badges/solarviewdatareader-installed.svg)
![Number of Installations (stable)](https://iobroker.live/badges/solarviewdatareader-stable.svg)
[![Known Vulnerabilities](https://snyk.io/test/github/afuerhoff/ioBroker.solarviewdatareader/badge.svg)](https://snyk.io/test/github/afuerhoff/ioBroker.solarviewdatareader)

[![NPM](https://nodei.co/npm/iobroker.solarviewdatareader.png?downloads=true)](https://nodei.co/npm/iobroker.solarviewdatareader/)

**Tests:** ![Test and Release](https://github.com/afuerhoff/ioBroker.solarviewdatareader/workflows/Test%20and%20Release/badge.svg)

## solarviewdatareader adapter for ioBroker

The adapter reads the data from the Solarview data logger.
Here you can find additional infos about Solarview: https://www.solarview.info/solarlogger.aspx


## Configuration

### IP address, Port
To get the data from the datalogger you must enter the ip-address and the port from your solarview TCP server. 
The standard port is 15000. Please refer to the Solarview documentation https://www.solarview.info/solarlogger.aspx.

### D0 converter
If you have a D0 converter connected to the Solarview data logger you can enable this option.
For questions please refer to the Solarview documentation.

### Self consumption meter sum and 1 to 4
If you have a S0 meter, you can enable this option. 
You can have up to 4 self consumption meters and the sum from all meters.
For questions please refer to the Solarview documentation.

### Inverter 1 to 4
Every inverter you can enable separately.
For questions please refer to the Solarview documentation.

### Interval, interval start, interval end
Here you can configure the time range and the interval. The time range for 24h is 00:00 to 23:59.
Not 00:00 to 00:00.

### Set system variable CCU, System variable
This is a special feature for the homematic CCU. You can define a system variable in the CCU.
In this system variable the actual PAC value is saved.
You have to fill in the ioBroker state for that system variable -> **e.g. "hm-rega.0.12345"**

### Created states
#### pvig, pvi1..4, d0supply, d0consumption
daily = daily yield (kWh)
montly = monthly yield (kWh)
yearly = yearly yield (kWh)
total = total yield (kWh)
current = generator power in W
UDC, UDCB, UDCC, UDCD = generator voltages in volt per MPP-Tracker
IDC, IDCB, IDCC, IDCD = generator current in ampere per MPP-Tracker
UL1, IL1 = mains voltage, mains power phase 1
UL2, IL2 = mains voltage, mains power phase 2
UL3, IL3 = mains voltage, mains power phase 3
TKK= Temperature inverter

## Changelog
<!--
	Placeholder for the next version (at the beginning of the line):
	### __WORK IN PROGRESS__
-->
### 1.0.8 (2024-01-18)
* (afuerhoff) dependencies updated
* (afuerhoff) translations updated

### 1.0.7 (2022-12-21)
* (afuerhoff) dependencies updated

### 1.0.6 (2022-07-04)
* (afuerhoff) dependencies updated
* (afuerhoff) Interval settings changed from minutes to seconds
* (afuerhoff) States only writen after changes

### 1.0.5 (2022-02-17)
* (afuerhoff) dependencies updated
* (afuerhoff) test and release updated
* (afuerhoff) smaller changes

### 1.0.4 (2022-02-09)
* (afuerhoff) dependencies updated
* (afuerhoff) issue #20 fixed

## License
MIT License

Copyright (c) 2019-2024 Achim Fürhoff <achim.fuerhoff@outlook.de>

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