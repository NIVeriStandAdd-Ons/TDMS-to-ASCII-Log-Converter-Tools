## TDMS to ASCII Log Converter Tools ##

**TDMS to ASCII Log Converter Tools** is source for a stand alone exe and NI VeriStand service whose primary goal is to convert TDMS log files to human readable text.

The executable converts a directory (sub directories optionally included) of NI VeriStand TDMS data logs in binary format (*.TDMS) to human readable text format. The exact format used in NI VeriStand 2009's text format.

The service, when added to an NI VeriStand project, will convert logged NIVS TDMS files to human readable ASCII in the format of NIVS 2009. The service runs in the background, and as **legacy** stimulus profiles complete, it converts the logged TDMS files on the host to ASCII. 

To use:

1. Add this service to your NIVS project
2. Deploy and connect. Now as you run batch/sequence legacy stimulus profiles, the tdms data logs will be in the appropriate logs directory as well as converted ASCII formats.

This service makes one assumptions:

1. You always run legacy stimulus profiles with the legacy batch/sequence editor.
2. The service expects the .nivstest files being sequenced in the sequence editor have relative paths for their log configurations. For example "MyLog.tdms" instead of "C:\MyLog.tdms"

### LabVIEW Version ###

LabVIEW 2010

### Built Availability ###

No builds are available

### Quality, Limitations ###

This IP was developed for a specific use case in 2010 and has not been tested since. It has not been updated for the new NI VeriStand stimulus profiles. Therefore, this has some usefulness for legacy project but needs upgrades to be useful for new projects.

### License ###

*This repository and any materials provided by NI therein are provided AS IS. NI DISCLAIMS ANY AND ALL LIABILITIES FOR AND MAKES NO WARRANTIES, EITHER EXPRESS OR IMPLIED, INCLUDING WITHOUT LIMITATION ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR  PARTICULAR PURPOSE, OR NON-INFRINGEMENT OF INTELLECTUAL PROPERTY. NI shall have no liability for any direct, indirect, incidental, punitive, special, or consequential damages for your use of the repository or any materials contained therein.*