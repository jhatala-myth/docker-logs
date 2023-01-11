# docker-logs
Centralized docker logs collection with Fluentd + ELK

![flow](/fluentd+elk.drawio.png)

## docker container logging example for docker-compose
```yaml
logging:
  driver: "fluentd"
  options:
    fluentd-address: 192.168.1.1:24224
    fluentd-async: true
    fluentd-retry-wait: 5
    tag: myaap_tag
```
