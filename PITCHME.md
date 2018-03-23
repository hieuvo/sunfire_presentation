# Sunfire

Log-based monitoring tool. Also provides other standard monitoring functions, like OS, Web, JVM, GC and middleware.

---

### Other systems

- Xflush: log-based monitoring tool, deprecated and fully migrated into Sunfire, will be shutdown soon
- Alimonitoring: Ali’s earlier monitoring system currently completes business monitoring through keyword filtering, page traffic. Deprecated but won't be shutdown in near future

---

### Sunfire's advantages

- All-round real-time monitoring:
	Provides monitoring capabilities from a variety of perspectives. Minute to second level monitoring, high reliability, high timeliness, and low latency.

- Flexible alarm rules:
	According to business characteristics, time period, and degree of importance, so as to achieve no false positives or omissions.

- Simple management:
	Millions of equipment monitoring and deployment capabilities of minutes, automatic recovery of failures, cluster scalability

- Custom and convenient configuration:
	Rich custom product configuration features, convenient and efficient completion of product configuration, alarm configuration.

- Visualization:
	Rich visual Dashboard helps you customize personalized surveillance market.

- Low resource consumption:
	Guarantees a very low occupancy rate of resources such as the CPU and memory of the host.

- Storage:
	Time series data are all stored in a separate Hbase cluster and maintained by the big data team. All data is saved for at least one year without data loss.

- Self-monitoring, self-run maintenance:
	Quickly detect and recover the problems of the monitoring system itself from the beginning of design. A dedicated role (OPS-Agent, Ops-web) assumes the health of the entire monitoring platform. Testing, one-click installation, fault recovery, capacity monitoring and other duties.

- Unitization:
	Capability of rapid unitized deployment, the minimum unit requires only 6 docker containers, we can select Hbase or Mongodb depending on the monitoring scale.
	
---

### Sunfire's modules

- Overview: general information of monitored applications, healthcheck, history of alarms, etc

- Application: basic system information including (CPU, load, disk, memory, etc), errors, system calls, database calls, sql consumption time, etc

- Custom: customized monitoring configuration (can create your custom dashboard for specific metrics)

- Alarm: allow creating alarm rules, setting up subcription and subscriber groups of alarm rules

- Plugin: monitoring of distributed systems (schedule service, event service, etc)

- Resource: monitoring of computing resources, database, storage resource

---

### Kinds of monitoring configuration

- Monitor at minute to second level
- Single and multiple dimensions of metrics

![Flux Explained](images/a.png)

---

### Demo

- How to create a monitor config
- How to setup alarm rules
