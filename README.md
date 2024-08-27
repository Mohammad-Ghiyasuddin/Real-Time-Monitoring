# Real-Time-Monitoring

#### Prerequisites

- Prometheus - is an open-source tool that helps monitor and alert you by collecting, storing, and analyzing data over time from applicaion and infrastructure.
- Black_box_exporter- in Prometheus is a tool that checks if your websites and services are working by testing them from the outside.
- Node Exporter- in Prometheus collects and exposes hardware and OS metrics (like CPU and memory usage) from servers for monitoring.
- Alertmanager-  in Prometheus manages and routes alerts, handling notifications and deduplication for monitoring systems
- Ensure you have `wget` and `tar` installed on both VMs.
- Ensure you have appropriate permissions to download, extract, and run these binaries.
- Replace `<version>` with the appropriate version number you wish to download.


#### In this project we have to use two instance one for web app and node exporter and another one is for Monitoring tools (Prometheus, Alert Manager and Black box exporter)

#### VM-1 

1. **Download Node Exporter**
   ```bash
   wget https://github.com/prometheus/node_exporter/releases/download/v1.8.1/node_exporter-1.8.1.linux-amd64.tar.gz
   ```

2. **Extract Node Exporter**
   ```bash
   tar xvfz node_exporter-1.8.1.linux-amd64.tar.gz
   ```

3. **Start Node Exporter**
   ```bash
   cd node_exporter-1.8.1.linux-amd64
   ./node_exporter &
   ```

**Clone your web app into instance**

```bash
  git clone "github repo url"
  ```

  

