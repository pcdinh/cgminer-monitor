cgminer-monitor
===============

Simple monitor script for cgminer in python. Console display, http server, email alerts. No additional modules required.

Tested with python 2.7.6 and cgminer 3.7.2 in Windows 7 64 bit

usage: cgminer-monitor.py [command] [parameter]


## Monitor mode
cgminer-monitor.py
 - Monitors cgminer by checking a few critical values
 - Emails if something is wrong
 - Restarts cgminer if the GPU is sick or dead
 - Runs a dead simple http server that only serves a page with the results of the monitor (identical to the console output with a nice display)
 - Monitors MMFCE pools and display the current balance in their currencies
 - Could support multi-gpus very easily (see comment in the code)
 - CTRL+C to stop everything

![cgminer-monitor](http://www.shazbits.com/images/cgminer-monitor.png)

![cgminer-monitor-iphone](http://www.shazbits.com/images/cgminer-monitor-iphone_tn.png)

![cgminer-monitor-email](http://www.shazbits.com/images/cgminer-monitor-email.png)


## Command mode
cgminer-monitor.py somecommand someoptionalparameter
 - Ouputs the results returned by cgminer miner and exits
 - Examples:
 	- cgminer-monitor.py summary
 	- cgminer-monitor.py gpu 0
 	- See cgminer's API-README for all available commands


### Credits
CGMinerClient class based on  WyseNynja's gist https://gist.github.com/WyseNynja/1500780

### Official forum thread
https://bitcointalk.org/index.php?topic=232232

## ISC License

https://github.com/shazbits/cgminer-monitor/blob/master/LICENSE.txt

Romain Dura
http://www.shazbits.com

BTC 1Kcn1Hs76pbnBpBQHwdsDmr3CZYcoCAwjj

![myviewcounter](http://www.shazbits.com/viewcounter-monitor.png)

