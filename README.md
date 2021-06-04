# CPPM_NLS
This repository describes the possibility to import ClearPass Radius and TACACS+ logs in Nagios Logserver.

In CPPM go to: Administration => External Servers => Syslog Targets and add the Nagios Logserver as your Syslog Target. (UDP 5544)
In CPPM go to: Administration => Syslog Export Filters and add a few export filters:

Filter1:
Add a name, this name will be in your log message and will be used in the Nagios Logserver input filter. In this example use radius as the name.
Choose the export Template "Insight Logs"
Add your Syslog server
Add your ClearPass servers
In "Filter and Columns" choose RADIUS Authentications
Save this filter.

Filter2:
Add a name, this name will be in your log message and will be used in the Nagios Logserver input filter. In this example use radius-failed as the name.
Choose the export Template "Insight Logs"
Add your Syslog server
Add your ClearPass servers
In "Filter and Columns" choose RADIUS Failed Authentications

