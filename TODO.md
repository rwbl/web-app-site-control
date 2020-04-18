# ToDo domoticz-webapp-sitecontrol
Status 20200128

### NEW: Tab Favorites, Groups
Fast access to common used functions, i.e turn dedicated light On/Off, thermostat setpoint.

Priority: Low
_Status_
Not started.

### NEW: Tab Info, Goup Various
Show the Last message in a ui-text node.

Priority: Low
_Status_
Not started.

### NEW: Tab Info, Group Key Dates
Check if the input file exists to avoid error:
```
Error: ENOENT: no such file or directory, open '\home\pi\wasc\wasc-keydates.json'
```

Priority: Low
_Status_
Not started.

### NEW: Remote Access WASC
WASC is running in a local intranet which is not accessible from outside.
Seek for a way to control or get information from WASC.
An option could be to use an email listenr with specific sender, subject and body.

Priority: Low
_Status_
Not started.

### NEW: Raspberry Pi Hardware Monitor
Get in regular intervals hardware data and display in the Tab Info, Group Hardware Monitor.
Solution idea:
Bash script "hwmondata.sh" executed via exec node. The script returns a JSON object. Example output:
```
{"cpuusage":2,"cputemp":37.394,"discspaceused":16,"ramused":234,"ramfree":274,"ramusedpct":46.063} 
```

Priority: Low
_Status_
Not started.

### NEW: Coffee Machine Monitor
See Domoticz Workbook
See also https://discourse.nodered.org/t/coffee-pot-timer/4743

Priority: Low
_Status_
Not started.


