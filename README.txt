
This plugin can check if a service is running using SNMP v1 queries.

check_snmp_service is written in Bash and is distributed under the GPLv2 license. This plugin have been created by Yoann LAMY.

Usage: ./check_snmp_service -H xxx.xxx.xxx.xxx -C public -s Service -p Parameters -w 5 -c 10

-H ADDRESS
Name or IP address of host (default: 127.0.0.1)
-C STRING
Community name for the host's SNMP agent (default: public)
-s STRING
Service's name
-p STRING
Service's parameters
-w INTEGER
Warning level for the number of service (default: 0)
-c INTEGER
Critical level for the number of service (default: 0)
-h
Print this help screen
-V
Print version and license information

This plugin uses 'snmpget' and 'snmpwalk' commands included with the NET-SNMP package.
This plugin support performance data output. If the percentage of the warning and critical levels are set to 0, then the script returns a OK state.

This nagios plugins comes with ABSOLUTELY NO WARRANTY.

You may redistribute copies of the plugins under the terms of the GNU General Public License v2. 
