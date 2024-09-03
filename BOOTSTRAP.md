# Bootstrap Elasticsearch

## Setup

```bash
docker compose \
-f ./docker-compose.yml \
-f ./extensions/fleet/fleet-compose.yml \
-f ./extensions/fleet/agent-apmserver-compose.yml \
-f ./extensions/metricbeat/metricbeat-compose.yml \
up setup
```

```pwsh
docker compose `
-f .\docker-compose.yml `
-f .\extensions\fleet\fleet-compose.yml `
-f .\extensions\fleet\agent-apmserver-compose.yml `
-f .\extensions\metricbeat\metricbeat-compose.yml `
up setup
```

## Up

```bash
docker compose \
-f ./docker-compose.yml \
-f ./extensions/fleet/fleet-compose.yml \
-f ./extensions/fleet/agent-apmserver-compose.yml \
-f ./extensions/metricbeat/metricbeat-compose.yml \
up -d --scale logstash=0
```

```pwsh
docker compose `
-f .\docker-compose.yml `
-f .\extensions\fleet\fleet-compose.yml `
-f .\extensions\fleet\agent-apmserver-compose.yml `
-f .\extensions\metricbeat\metricbeat-compose.yml `
up -d --scale logstash=0
```

## Scale `setup=0`

```bash
docker compose \
-f ./docker-compose.yml \
-f ./extensions/fleet/fleet-compose.yml \
-f ./extensions/fleet/agent-apmserver-compose.yml \
-f ./extensions/metricbeat/metricbeat-compose.yml \
scale setup=0
```

```pwsh
docker compose `
-f .\docker-compose.yml `
-f .\extensions\fleet\fleet-compose.yml `
-f .\extensions\fleet\agent-apmserver-compose.yml `
-f .\extensions\metricbeat\metricbeat-compose.yml `
scale setup=0
```
