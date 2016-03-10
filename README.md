# zabbix_crashplan_stats
Zabbix Script for Crashplan healthcheck and backup lag in seconds


put his in your user_parameters.conf:
```
UserParameter=crashplan.crashplan_lag[*],/etc/zabbix/agent_scripts/crashplan_stats -d $1
UserParameter=crashplan.crashplan_is_running[*],/etc/zabbix/agent_scripts/crashplan_stats -r $1
UserParameter=crashplan.crashplan_service_is_running,/etc/zabbix/agent_scripts/crashplan_stats -p
```
