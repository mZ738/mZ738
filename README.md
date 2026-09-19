## Marvin Z

Long-time systems administrator, with time spent in IT security and site
reliability engineering along the way. Infrastructure automation, monitoring,
and making things observable — at work and at home.

I prefer open source wherever it does the job, and I try to give back rather than
just consume: fixes and features go upstream instead of living in a private fork,
and I sponsor projects I rely on.

I maintain the **[Proxmox VE integration for Home Assistant](https://github.com/dougiteixeira/proxmoxve)**.
New features are developed and tested in [my fork](https://github.com/mZ738/proxmoxve-integration)
before they go upstream — that repo is the beta channel if you want to try them early.

### Skills

| | |
|---|---|
| **Currently** | SAP Basis (HANA, S/4HANA, ERP) · Prometheus · Grafana · Microsoft SQL Server · PowerShell · Python · Bash |
| **Home lab** | Proxmox VE · Home Assistant · OPNsense · Wazuh · NetBox · Zigbee / MQTT · Frigate · AdGuard Home |
| **Also experienced with** | Kubernetes · Google Kubernetes Engine · Terraform · Google Cloud Platform · CI/CD · SRE practices · information security · vulnerability management |

### The home lab

A multi-node Proxmox VE cluster with HA failover, a virtualised OPNsense routing a
segmented VLAN network, and Home Assistant tying the house together.

Enterprise tooling, scaled down to a house:

- **Wazuh** as a SIEM, with agents reporting from the hosts
- **NetBox** as IPAM and inventory, feeding Prometheus service discovery automatically
- **Elasticsearch** behind the firewall's deep packet inspection reporting
- **A self-hosted secret store**, so no credentials sit in config files
- **Cluster HA failover** with node affinity rules, over a dedicated migration network
- **GPUs passed through into containers** for camera object detection and local LLM inference
- **Redundant filtering DNS**, so name resolution survives a node going down

Most of what I publish here started as something I needed there first.
