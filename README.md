# GhostNet — Wi-Fi Motion Detection Using D-Link DAP-1610

GhostNet Lite is a zero-budget, software-only motion and human presence detection system
that uses Wi-Fi signal distortions as a sensing mechanism. No sensors. No cameras. 
Only a D-Link DAP-1610 Wi-Fi extender and Python.

## Features
- Real-time RSSI and latency monitoring
- ML-based motion classification
- Privacy-friendly (no images or audio)
- Zero hardware modifications
- Patentable methodology

## Tech Stack
- Python
- Scikit-learn
- NumPy / Pandas
- Bash (ping, iwconfig)

## Dataset
Collected 3 categories:
- No motion
- Light motion
- Intrusion motion

## Architecture
Router → D-Link Extender → Laptop → Python Collector → ML Model → Output

## Patent Novelty
First-of-its-kind use of a Wi-Fi extender to perform motion detection using 
network-layer distortion patterns.

## How to Run
1. Run `collector.py` to record Wi-Fi metrics.
2. Label dataset and run `train.py`.
3. Run `detect.py` for live prediction.

## Applications
- Intrusion detection
- Smart homes
- Elderly care
- Privacy-safe monitoring
