# Prometheus & Grafana Monitoring Dashboards

This directory contains Grafana dashboard screenshots showing various metrics from our EKS cluster monitoring setup.

## 📊 CPU Usage
![CPU Usage Dashboard](./cpu-usage.png)
*Dashboard showing cluster-wide CPU utilization patterns and resource consumption metrics*

## ⏱️ Application Uptime
![Application Uptime Dashboard](./Application-uptime.png)
*Displays service availability and uptime metrics across different components*

## 💾 Memory Usage
![Memory Usage Dashboard](./memory-usage.png)
*Visualization of memory consumption patterns and allocation across pods/nodes*

## 🔄 Throughput
![Throughput Dashboard](./throughput.png)
*Network throughput metrics showing request/response patterns and data transfer rates*

## Dashboard Details

These dashboards are configured using:
- Prometheus as the data source
- Grafana v9.x for visualization
- 5-minute refresh intervals