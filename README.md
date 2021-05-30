# Launch Grafana with Network-Latency and node availability dashboards

```
1. git clone https://github.com/MichaelGit-beep/grafana-network-latency.git
2. cd grafana-network-latency
3. edit URLs in ./config/telegraf/telegraf.conf
4. docker-config up -d
```
Access grafana on localhost:3000 username - "admin" password - "CHANGEME"

# Add monitoring target
```
1. Add URL to ./config/telegraf/telegraf.conf
2. docker-compose restart
```
# Delete monitoring target
```
1. Remove URL from ./config/telegraf/telegraf.conf
2. docker-compose down
3. docker volume rm grafana-network-latency_influxdb
4. docker-compose up -d
```
