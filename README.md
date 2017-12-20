# JRStat: A flexible open source platform for statistical analysis using IDE

## What is JRStat

**JRStat** is: 

- a platform which performs statistical analysis with R.

- a flexible IDE built with Java. You can add new modules with xml files.

- an open source project.

- a multiplatform IDE.

## Requirements

1) Java Runtime Environment (At least Java SE 1.8 Update 151).

2) GNU R, at least R-3.4.2, see http://www.r-project.org.

3) Once that R has been installed it is necessary to install a couple of R packages:

    - R Package [rJava](https://cran.r-project.org/web/packages/rJava/index.html), see more information [here](https://rforge.net/rJava/). Use `install.packages("rJava")` in R to install the package.

   - R package [JavaGD](https://cran.r-project.org/web/packages/JavaGD/index.html), see more information [here](https://rforge.net/JavaGD/). Use `install.packages("JavaGD")` in R to install the package. 

The installation can be done manually using the function `install.packages()` in R or it can be done automatically when the program run for first time.

## Software distribution

The software is distributed in a folder whose structure is shown below:

~~~
JRStat distributable
|-- Installer.R
|-- JRStat.jar
|-- Readme.md (This file)
|-- Runner_Linux
|-- Runner_Linux.c
|-- Runner_Linux.sh
|-- Runner_OsX
|-- Runner_OsX.c
|-- Runner_win_djk9.c
|-- Runner_win_jdk8.c
|-- Runner_win_jdk8.exe
|-- build_win.bat
|-- examples
|-- lib
    |-- JRI.jar
    |-- javaGD.jar
    |-- jcommon-1.0.23.jar
    |-- jfreechart-1.0.19.jar
~~~

The application is packed in the file **JRStat.jar**. Before the application runs, several environmental variables must be set (see https://rforge.net/JRI/).

In order to automate the process I am providing three small programs:

**Runner_win_jdk8.exe**: It loads the application in a windows machine with JDK/JRE 8.

**Runner_win_jdk9.exe**: It loads the application in a windows machine with JDK/JRE 9.

**Runner_Linux**: It loads the application in Linux.

**Runner_OsX**: It loads the application in macOS.

I am also providing the source code of the applications (C code), which are based on the JGR launcher developed by [Simon Urbanek](https://www.rforge.net/JGR/).

## About

JRStat 0.1 (Java + R + Statistics), available [here](http://est.colpos.mx/JRStat/).

Author: Paulino Pérez-Rodríguez, perpdgo@colpos.mx

Colegio de Postgraduados, campus montecillo, [Estadística](http://www.colpos.mx/wb/index.php/campus-montecillo/posgrados/socioeconomica-estadistica-e-informatica/estadistica), 2016-2017.

This program is Free Software.
You can distribute it under the terms
of the GNU-GPL License version 3.
