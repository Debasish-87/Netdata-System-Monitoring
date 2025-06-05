# 📊 Netdata System Monitoring via Docker

## 🧩 Objective
This project demonstrates how to monitor system resources using **Netdata**, a real-time monitoring tool, via Docker.

---

## 🚀 Setup Instructions

### 🔧 Step 1: Run Netdata using Docker
```bash
docker run -d --name=netdata -p 19999:19999 \
  --cap-add=SYS_PTRACE --security-opt apparmor=unconfined \
  netdata/netdata
🌐 Step 2: Access Dashboard
Open your browser and visit:
👉 http://localhost:19999

📊 Metrics Collected
CPU Usage

Memory Usage

Disk Usage

Docker Containers

Systemd services & logs

Network I/O

🧠 System Details
Kernel Version: 6.11.0-26-generic

CPU Cores: 4

RAM: 7.54 GB

Disk Size: 476.94 GB

Architecture: x86_64

Virtualization: None

📂 Key Directories and Configs
Logs: /var/log/netdata

Configs: /etc/netdata, /usr/lib/netdata/conf.d

Database: /var/lib/netdata

Plugins: /usr/libexec/netdata/plugins.d

Web Files: /usr/share/netdata/web

📸 Screenshot

❓ Interview Questions & Answers
1. What does Netdata monitor?
Netdata monitors CPU, RAM, disk I/O, network traffic, Docker containers, system services, and more.

2. How do you view real-time metrics?
By accessing the live dashboard at http://localhost:19999.

3. How is Netdata different from Prometheus?
Netdata is real-time, lightweight, and provides auto-dashboards. Prometheus is pull-based, scalable, and ideal for long-term monitoring and alerting (often paired with Grafana).

4. What is a collector in Netdata?
A plugin/module that gathers specific metrics from the OS, apps, or containers (like proc, disk, apps, cgroups).

5. What performance KPIs are important?
CPU load and usage

Memory usage

Disk I/O latency

Network bandwidth

Container resource usage

6. How to deploy Netdata on a VM?
Run the one-liner script:
bash <(curl -Ss https://my-netdata.io/kickstart.sh)
or use Docker for quick deployment.

7. How does Netdata alerting work?
Netdata has preconfigured thresholds. When exceeded, it generates alerts based on health configuration files.

8. What is a dashboard in this context?
A web-based interface that displays real-time charts and alerts for monitored metrics.

📘 Outcome
✅ Gained hands-on experience in:

Lightweight monitoring

Using Docker for tool deployment

Understanding key system KPIs

Real-time performance tracking

📎 Submission Checklist
 Dashboard screenshot added (screenshot.png)

 Full README with setup, metrics, Q&A

 GitHub repo created

yaml
Copy
Edit

---

