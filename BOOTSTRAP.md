# Bootstrap Elasticsearch

## PowerShell

### Setup

```pwsh
docker compose `
-f .\docker-compose.yml `
-f .\extensions\fleet\fleet-compose.yml `
-f .\extensions\fleet\agent-apmserver-compose.yml `
-f .\extensions\metricbeat\metricbeat-compose.yml `
up setup
```

### Up

```pwsh
docker compose `
-f .\docker-compose.yml `
-f .\extensions\fleet\fleet-compose.yml `
-f .\extensions\fleet\agent-apmserver-compose.yml `
-f .\extensions\metricbeat\metricbeat-compose.yml `
up -d --scale logstash=0
```

### Scale `setup=0`

```pwsh
docker compose `
-f .\docker-compose.yml `
-f .\extensions\fleet\fleet-compose.yml `
-f .\extensions\fleet\agent-apmserver-compose.yml `
-f .\extensions\metricbeat\metricbeat-compose.yml `
scale setup=0
```
