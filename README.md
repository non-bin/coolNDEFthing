# Cool NDEF Thing

A (hopfully) highly feature-packed NDEF applet, [available through Fidesmo](https://apps.fidesmo.com/8210647A)
A constant work in progress, but I use it personally.

## Building

Install [Apache Ant](https://ant.apache.org/) from the wesite or through your package manager, change any properties at the top of build.xml, then run:
````
ant clean
ant build
````

The resulting cap file will be at `build/main.cap`.

The main ant targets are:

 - `clean`: Delete build files and extensions
 - `build`: Build the applet (download ant-javacard if nesssary)
 - `deploy`: Deploy the applet to Fidesmo, requires the FIDESMO_AUTH env variable (download fdsm if nesssary)

## Credits

 - Based on [OpenJavaCard NDEF](https://github.com/OpenJavaCard/openjavacard-ndef), which contains some code from the fine [IsoApplet by philipWendland](https://github.com/philipWendland/IsoApplet)
 - Uses code from [htop_via_ndef by Petris](https://github.com/petrs/hotp_via_ndef)

## Legal

    coolNDEFthing - a javacard applet that provides services through NDEF
    Copyright (C) 2022  non-bin

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
