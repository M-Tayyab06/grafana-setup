# Grafana Setup Guide (Ubuntu/Debian)

![License](https://img.shields.io/github/license/M-Tayyab06/grafana-setup?color=blue)
![Stars](https://img.shields.io/github/stars/M-Tayyab06/grafana-setup?style=social)
![Issues](https://img.shields.io/github/issues/M-Tayyab06/grafana-setup)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)
![Ubuntu](https://img.shields.io/badge/Ubuntu-22.04-orange?logo=ubuntu)

# Grafana Setup Guide (Ubuntu/Debian)

This repository contains step-by-step instructions for installing **Grafana OSS** on Debian/Ubuntu using the official APT repository.

---

## 📥 Installation

```bash
# Install required dependencies
sudo apt-get install -y adduser libfontconfig1

# Add Grafana GPG key
wget -q -O - https://packages.grafana.com/gpg.key | sudo apt-key add -

# Add Grafana APT repo
echo "deb https://packages.grafana.com/oss/deb stable main" | sudo tee /etc/apt/sources.list.d/grafana.list

# Update package list
sudo apt-get update

# Install Grafana
sudo apt-get install grafana -y
