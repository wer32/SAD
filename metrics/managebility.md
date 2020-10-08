# Manageability

Manageability defines how easy it is for system administrators to manage the application,
usually through sufficient and useful instrumentation exposed for use in monitoring systems
and for debugging and performance tuning.

# Metrics
- System logs are collected: yes/no
- Level of logging may be changed in a runtime: yes/no
- Troubleshooting tools exists, actual, well-documented and well-known to administrators: yes/no
- The system is monitored by a 3rd party tools: yes/no
- Exact list of information to be collected/traced/monitored for diagnostics and for administration/troubleshooting: list
- Business reporting system: yes/no
- The system is monitoring 3-rd party tools: SPLUNK, CloudWatch, Dynatrace, Zabbix, Spring Admin, ELK
- Ability to visualize business steps for particular event: yes/no (Camunda, custom)
- Exact list of information to be collected/traced/monitored for diagnostic and for administration/troubleshooting:
  - business events
  - exceptions
  - up/down service event
- Single configuration point for business processes: yes