# 📊 Netdata Monitoring - DevOps Internship Task 7

This project demonstrates how to **monitor real-time system performance** using [Netdata](https://www.netdata.cloud/), a powerful and lightweight open-source monitoring tool. It is part of my DevOps internship (Day 7) to gain hands-on experience with live metrics visualization and system health monitoring.

---

## 🎯 Objective

- Install and run Netdata via Docker
- Access live system metrics using a web-based dashboard
- Monitor key performance indicators (KPIs) like CPU, Memory, Disk I/O, and Network
- Take a screenshot of the Netdata dashboard

---

## ⚙️ Technologies Used

| Tool       | Purpose                           |
|------------|-----------------------------------|
| Docker     | To containerize and run Netdata   |
| Netdata    | Real-time system metrics dashboard|
| Linux/Ubuntu | Host system environment          |

---

## 🚀 Getting Started

### Step 1: Pull and Run Netdata via Docker

```bash
docker run -d --name=netdata -p 19999:19999 \
  --cap-add SYS_PTRACE --security-opt apparmor=unconfined \
  netdata/netdata

### Step 2: Open this in your browser: http://localhost:19999

