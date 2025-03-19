This project demonstrates how to set up a monitoring stack for a Kubernetes cluster using Prometheus, Grafana, and Alertmanager.

## Folder Structure

- `prometheus/`: Contains Prometheus configuration files and dashboards.
- `grafana/`: Contains Grafana dashboards.
- `alertmanager/`: Contains Alertmanager configuration files.

## How to Use

1. Deploy Prometheus:
   ```
   kubectl apply -f prometheus/
   Deploy Grafana:



kubectl apply -f grafana/
Deploy Alertmanager:



kubectl apply -f alertmanager/
Access the monitoring stack:

Prometheus: http://<prometheus-service-ip>:9090

Grafana: http://<grafana-service-ip>:3000

Alertmanager: http://<alertmanager-service-ip>:9093

Prerequisites
Kubernetes cluster.

kubectl installed and configured.

**Example Commands**


Deploy Prometheus
kubectl apply -f prometheus/


Deploy Grafana
kubectl apply -f grafana/


Deploy Alertmanager
kubectl apply -f alertmanager/


Access Prometheus
kubectl port-forward svc/prometheus 9090:9090


Access Grafana
kubectl port-forward svc/grafana 3000:3000

Access Alertmanager
kubectl port-forward svc/alertmanager 9093:9093
