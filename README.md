# bcsmart
Bucks County Smart Home

This repository contains groovy files for use on Hubitat to control IOT devices.  

File gogoGateGarage.groovy is a Hubitat driver to control the gogoGate2 Garage/Gate opener.  This file should be added via the drivers code option.  Once added, you can create a virtual device and make it User Type gogoGate2 Garage Controller.  After saving, complete the required fields, then click initialize.  You should be ready to go!

This driver polls the gogoGate2 at a 2 second interval, so the door's status gets updated fairly quickly upon completion of a door activity (i.e. open or close).  This status will update regardless of whether the door is opened via the HE.  This allows you to develop rules that will run on Door Open or Close events even if the door is activated via it's hardwired button, Homelink, or some other method.

To use with rules, choose the Door category and select your Garage Door from the list.  
