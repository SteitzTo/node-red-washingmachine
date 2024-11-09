Node-Red-Washingmaschine
=============

Hi,


At home I always had the problem, when the Waschingmaschine or the Dryer is finish, there is no notification that the Job is done.

So you have to go downstairs in the cellar to look if its done.  Very annoying!

It would be nice if Alexa reminds you.

--------------------------------------------
Dependencies:


[node-red-contrib-power-monitor](https://flows.nodered.org/node/node-red-contrib-power-monitor)

[node-red-contrib-virtual-smart-home](https://flows.nodered.org/node/node-red-contrib-virtual-smart-home)

[node-red-contrib-alexa-remote2-applestrudel](https://flows.nodered.org/node/node-red-contrib-alexa-remote2-applestrudel)

----------------------------------------------------

Additonal Information:


The [Plugs](https://www.amazon.de/gp/product/B08BFPGWZ1/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1) are some Tasmota Plugs from Amazon



----------------------------------------------------

![Waschmaschine](https://github.com/user-attachments/assets/7326f17a-fdff-4ef7-9d1d-388ce79ff5f3)


The Plugs measure the Power and if its raised over 100W the Node Red Powermonitor swich to "Starting" 

If the energy consumption fall under the value of 2W the Powermonitor switch to "Finish" and Alexa reacts with:

Hello the Waschingmaschine / Dryer is finish.

She repated this notification 2 times.

You have to adjust your thresholds Powermonitor to your fits, bacause every Washingmaschine / Dryer and every Programm on this Maschines are diffrent.

I send the readout of the Plugs to a Influx-DB and visualised it with Grafana to find out my values 







If you want to use it too: have fun with it.

Torsten
