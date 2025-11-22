A python script that monitors the ac input source of a victron inverter and automatically switches the AC water heater 
switch on if the source is Grid or Shore, and switches it off otherwise. meant to operate on a cerbo gx but might work 
on other venus os devices as well. AC Water Heater must be controlled by one of the gx relays.

######## INSTALLATION #########

The water heater must be controlled by one of the GX devices relays, or a virtual switch connected to venus os, and that 
relay must have the custom name changed to "AC Water Heater" or "AC WH" in order for the service to discover it.
On older versions of venus os the custom name cannot be changed from the gui. In this case you can open SSH terminal and
use dbus-spy to change the custom name.

open terminal and enter the following

```
wget -O /tmp/download.sh https://raw.githubusercontent.com/drtinaz/auto_switch/master/download.sh
bash /tmp/download.sh
```
