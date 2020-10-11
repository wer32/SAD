# Scalability

Scalability is ability of a system to either handle increases in load without impact on the performance of the system,
or the ability to be readily enlarged.

# Metrics
- System architecture allows horizontal scaling: yes/no
- Time needed to scale up/down the system: # of secs/mins
- Scaling limits(number of servers, network bandwidth, disk space etc.) sufficient for the business domain: list
- Exact solution components to be able to scale out
- Exact scale out conditions
- Ability to scale out Product (addressing growth volume of transaction, number of custom content, response time, number of libraries).
- Exact scale out conditions: CPU usage > xxx%, Memory usage > xx%

# Example metrics
- If the parallel request number is more than 14 or the CPU usage is over 70% during 5 minutes then the given service
  should be scaled up by using Azure’s auto scaling functionality.
- If the parallel request number is, less than 14 or the CPU usage is under 70% during 20 minutes and if the instance
  number is more than 1 then the given AppService should be scaled down by using Azure’s auto scaling functionality