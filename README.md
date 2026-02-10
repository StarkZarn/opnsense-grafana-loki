# OPNSense Filterlog Firewall Dashboard (Grafana)

This repository contains a **Grafana dashboard JSON export** for visualizing OPNSense firewall traffic logs (`filterlog`) with **GeoIP enrichment**. It accompanies my [blog post](https://roguesecurity.dev/blog/opnsense-loki-part2) on how to collect, enrich, and visualize OPNSense logs using **Grafana Alloy** and **Loki** as the data source.

## 📊 Dashboard Overview

This basic dashboard includes:

- Source and destination IP visualizations
- GeoIP-resolved locations with world map panels
- Firewall action summaries (pass/block)
- Protocol and port breakdowns
- Time-series charts for traffic volume

Ideal for anyone running OPNSense who wants deeper insight into network activity with geographical context.

## 🔧 Requirements

To use this dashboard, ensure you have the following setup:

- **Grafana** (v8+ recommended)
- **Grafana Alloy** as the data source for Grafana (for log aggregation and analysis)
- **Loki** as the log aggregator to collect OPNSense `filterlog` data
- **GeoIP enrichment** via your log pipeline in Loki (again, see the [blog post](https://roguesecurity.dev/blog/opnsense-loki-part2) )
- Grafana **worldmap** plugin (if using geo panels)

## 🚀 Getting Started

1. Clone this repository or download the `opnsense_filterlog_dashboard.json` file.
2. Open **Grafana** and go to **Dashboards > Import**.
3. Upload the JSON file or paste its content.
4. Select **Loki** as your data source when prompted.
5. Click **Import** to add the dashboard.

## 📚 Related Blog Post

See the full guide on how to collect, enrich, and visualize OPNSense logs with GeoIP and Grafana:

👉 [My Blog Post: Monitoring OPNSense Logs with Grafana Loki](https://roguesecurity.dev/blog/opnsense-loki) 

## 📝 Notes

- Based heavily on the work of extremempd. Thank you!

## 🛡️ License

GPLv3 License. See [LICENSE](LICENSE) for details.

Copyright 2025 ~ StarkZarn
