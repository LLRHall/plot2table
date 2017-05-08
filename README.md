Plot to Table
-------------

A toolkit to convert a plot into table of values.


Description
-----------

plot2table uses Image Processing to extract plots from documents and produces a table of the data points used for all types of plots in the graph. It works for multiple graphs in a page with multiple plots in a single graph.

The input is a set of (multiple) scanned pdf pages, each containing (one or more) figures which are two-dimensional plots of experimental results. A scanned page can have a single or multiple plots which may or may not be embedded in text. Each plot has the x and y axis with their labels and unit measurements marked in the plot (linear scale). Inside each figure are one or more plots, each with a different colour depicting a certain plotted entity (Ei) and their labels given separately within the plot as a caption.

The software reads the set of scanned pages as input and generate one table per plot, where each row of the table has the following values - the x-axis value, y-axis value and values for each Ei or a dash (-) in case there is no value for that Ei. Each Table has the first row as the name labels for the x-axis, y-axis and various Ei values. It covers x and y axis values from the minimum to maximum range with one tenth of the minimum marked unit in the plot as granularity. The Table as a whole has a caption as per the caption of the figure.

The output is a set of pdf pages which contains the name of the participant as the first page followed by a sequence of results having the first input page followed by the set of tables corresponding to the figures in that page (one table per page) followed by the next input page and the tables of that page, etc.

Installation
------------

See INSTALL.txt

Execute `install.sh` for full dependency downloads and installation.

Tests
-----

Execute

```
$ nosetests -v
```

from the root of the library to check if all the test cases compile and run.

Usage
-----

Open terminal and run execute

```
$ plot2table
```

to open the Graphical User Interface.

Provide the command with a pdf file as an argument and it will run the CLI tool.

Authors
-------

* Sumit Goswami
* Ankesh Kumar Jha
* Samuel S. Bushi
* Krishna Sai Rohith
* Sidhartha Satapathy
* Gunjan Sengupta
* Siddhant Singh
* Aniket Choudhary
* Ashrujit Ghoshal
* Dilip Kumar Veeraraghavan
* Abhishek Panigrahi
* Himanshu Mishra

