
# High Level Design - Agente de Monitoramento Web

## Componentes

- **Agente Python**: coleta ping e HTTP, envia para InfluxDB
- **InfluxDB**: banco de dados time-series
- **Grafana**: visualiza os dados
- **Docker Compose**: orquestra os serviços

## Fluxo

1. Agente faz `ping` e `HTTP GET` nos sites
2. Resultado enviado para InfluxDB via API
3. Grafana consulta o InfluxDB para mostrar em dashboards

## Diagrama
```
[Agent Container] ---> [InfluxDB] ---> [Grafana]
        ^                             |
        |                             |
    [Sites monitorados]          [Dashboard Web]
```
