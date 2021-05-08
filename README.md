# README #

HDMI Out Demo project running on ARTY Z7-20 hardware for Vivado 2017.3

Based on the original "Arty-Z7-20-hdmi-out" example from Digilent

Copyright (C) 2021 Magictale Electronics
http://magictale.com

Getting started:

* Build the PL code locally by executing the following commands in the:

       Vivado directory:
        
        + Create the project file from the block diagram, wrapper and constraints file:
            vivado -mode batch -source create_project_file.tcl
        
        + Synthesise, place & route and generate bitfile for use in SDK:
            vivado -mode batch -source create_sdk_files.tcl

* Execute the following command in the SDK/hdmi_out_demo directory:
    + xsdk -batch create_sdk.tcl 0

* Now the SDK can be opened with the following command:
    + xsdk -workspace .

* The boot image can be created with the following comand:
    + xsdk -batch bootgen_sdk.tcl 0
