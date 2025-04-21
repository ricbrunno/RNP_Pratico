
# Prova Prática - DevOps em Redes

## 🛠️ Solução

A prova foi implementada com Docker e Docker Compose, monitorando `google.com`, `youtube.com` e `rnp.br` via ping e HTTP. Os resultados são enviados para o InfluxDB e visualizados no Grafana.

## 🔧 Tecnologias Usadas
- Python 3.9
- Docker / Docker Compose
- InfluxDB 2.7
- Grafana
- InfluxDB Python Client

## ▶️ Como Executar

```bash
git clone <seu-repo>
cd devops-monitoring-prova
docker-compose up -d
```

Grafana estará em: http://localhost:3000  
Login padrão: `admin` / `admin`

## 📊 Dashboards
Veja o print abaixo ou importe o JSON da pasta `dashboards/`.

![Dashboard Print](dashboards/agent-monitor.png)

## 💡 Projetos Relevantes

- [CI Monitoring com Prometheus](https://github.com/seu-usuario/projeto-1)
- [Automação com Ansible](https://github.com/seu-usuario/projeto-2)

## 📘 HLD

Ver arquivo [HLD.md](HLD.md)
