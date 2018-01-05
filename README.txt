This file serves as the README file for running the scripts for webpage classification
with the webkb University data.

The whole process can be broken down into the following processes

A. Using fetch_data.ipynb
=========================

1. This file helps to get the data structured into a CSV file from the various HTML
files.

2. The file by default requires the input directory to be "webkb". If you are using a
different path, please update the input argument for the line

                        crawl = fetch_data(directory = "webkb")
                        # initialize object to extract data

3. The preprocessing of the data is done as explained in the document.

4. Finally, the data is stored to a CSV named "data.csv".

B. Using analysis.ipynb
=======================

1. This file takes input from "data.csv" [by default].

2. Then, all the process explained in the document such as feature extraction,
model selection, model building, bias variance trade off, and evaluation are done.
