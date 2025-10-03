---
title: "curl"
draft: false
---
# curl

Some useful curl commands

## Request IP address with specific names

Example: Resolve the domain example.com on port 80 to 127.0.0.1

```bash
curl --resolve example.com:80:127.0.0.1 http://example.com/
```

## View the latest version for specific software on GitHub

### URL to API

* https://api.github.com/repos/prometheus/alertmanager/releases/latest
* https://api.github.com/repos/prometheus/blackbox_exporter/releases/latest
* https://api.github.com/repos/grafana/grafana/releases/latest
* https://api.github.com/repos/prometheus/prometheus/releases/latest
* https://api.github.com/repos/influxdata/telegraf/releases/latest
* https://api.github.com/repos/thanos-io/thanos/releases/latest


```bash
curl --silent "<apiurl>" | grep '"tag_name":' | sed -nre 's/^[^0-9]*(([0-9]+\.)*[0-9]+).*/\1/p'
```
