# Tesla-Drive-Unit
Open Source logic board for the Tesla Model S large rear drive unit. PCB Files in DesignSpark 8 format.
Based on the inverter designed by Johannes Heubner using slip control.

29/07/17 : V1 files released. Please note that as of this date the design is completely untested.
Use at your own risk for education purposes only. Further updates when testing starts and future versions are released.

10/08/17 : While functional the V1 board will not correctly read the Tesla current sensors as they are Sigma - Delta ADC as opposed to analog. Other issues with the design include spurious triggering of the fault detection lines due to switching noise.Solutions to these problems along with some upgrades are on the way in the V2. Stay tuned:)

19/08/17 : V2 files for the Large drive unit board released. Same discalimer as before : untested , for educational use only. If you blow up your house , cat or car with this design I accept no responsibility. Major upgrades over the V1 :

Three stage active filter to recover current sensor analog values from Sigma Delta encoding.

Variable frequency clock generator for Sigma Delta converters.

Buffer on IGBT drive lines.

All temp sensors read via a dual 4:1 multiplexer.

Crusie control input.

Jumper selectable CAN or RS232 communication.

10/09/17 : The V2 board has passed all bench tests and works well. Not tested in a car as yet.

23/09/17 : Creep and cruise control working on bench tests with inverter back in drive unit. Released beta software .bin file and paramaters for low voltage and high voltage testing. Not yet ran in a car. Same discalimer as before : untested , for educational use only. If you blow up your house , cat or car with this design I accept no responsibility.

30/09/17 : Uploaded a spreadsheet with resistance / temperature values for the inverter heatsink and motor case for the large drive unit. 

01/10/17 : Uploaded latest software build with working temperature sensors.

26/10/17 : Uploaded latest software build and document detailing CAN message formats.

03/11/17 : Link to source code for those interested : http://johanneshuebner.com/quickcms/index.html%3Fen_downloads,14.html
Note I do not write the software. It is however fully open source and available from the link above.

25/11/17 : Started the documentation. Work in progress as the project evolves.

09/12/17 : First test drive in car a success. Uploaded series of wiring diagrams. 

Have fun :)

    Copyright (C) 2017  Damien Maguire and Johannes Huebner

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.
