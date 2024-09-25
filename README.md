# MANG@COAST


## Description

Mangrove coast dynamics simulation in French Guiana
This version is written using Ocelet Chartreuse (v2.1.0) 64 bits.
Ocelet can be downloaded from [http://www.ocelet.fr/](http://www.ocelet.fr/)

+ The Ocelet langage source files are located in `oclt/`

## Installation

+ Unarchive the zip file in a directory.

> Warning: 
Make sure that Java Version 8 has been installed 
on your system before use. If this is not the case, 
or if you are not sure, you can install Java free 
of charge from the official Java website at :
[https://www.java.com/fr/download/manual.jsp
](https://www.java.com/fr/download/manual.jsp)

## Usage

Two types of execution are possible from a command 
prompt placed in the MANG@COAST_2024 directory: 


Use with default parameters: 

    java -jar .\MANGACOAST_2024.jar


Use with parameters :

    java -jar .\MANGACOAST_2024.jar pown bcol sfw startyear endyear idsector

+ `pown,bcol,sfw` are model's coefficients (type: float)
+ `startyear,endyear` determine the simulation period (between 2013 and 2023) (type: integer)
+ `idsector` identifying the mangrove areas to be simulated (between 1 to 8) (type: integer)

The model outputs are deposited in the "output" folder in GIS format.

>Warning:
All parameters must be supplied in the order in which they were declared.
If the number of parameters given on the command line is different, the default values will be used.

+ Parameters are separated by a space on the command line. If you need to 
supply text that contains spaces, you must enclose it in inverted commas.

+ You must ensure that the values given on the command line correspond to 
the type of parameters declared. For example, if you declare a parameter of 
type Integer and give a value of 4.5, this parameter will not be valid and 
its default value will be used. A message is displayed in this situation 
to indicate that there has been a problem converting the type. 


## 	License	

CC BY NC SA - [https://creativecommons.org/licenses/by-nc-sa/4.0/deed.en](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.en)