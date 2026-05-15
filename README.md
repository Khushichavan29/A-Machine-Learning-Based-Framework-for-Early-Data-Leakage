
# 🔐 A Machine Learning-Based Framework for Early Detection of Data Leakage in Multi-Tenant Cloud Environments

> A proactive, ML-driven security framework that detects data leakage threats in multi-tenant cloud environments **before exfiltration occurs** — combining anomaly detection, behavioral profiling, and real-time alert pipelines.

[![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Cloud](https://img.shields.io/badge/Cloud-Multi--Tenant-1D9E75?style=flat-square&logo=amazonaws&logoColor=white)]()
[![Status](https://img.shields.io/badge/Status-Research%20%2F%20Active-blue?style=flat-square)]()

---

## Overview

Multi-tenant cloud environments share physical infrastructure across multiple clients, creating a persistent risk of unintended or malicious data leakage between tenants. Traditional rule-based detection systems react **after** a breach — this framework shifts the paradigm to **early, predictive detection** using machine learning.

The system continuously monitors access patterns, network flows, and resource usage across tenant boundaries. It builds behavioral baselines per tenant, flags statistical deviations, and classifies suspicious activity in real time — raising alerts before data leaves the environment.

---

## Key Features

- **Tenant-aware behavioral profiling** — per-tenant baselines built from historical access and resource logs
- **Multi-model ML pipeline** — combines anomaly detection, classification, and ensemble methods
- **Early warning system** — detects pre-exfiltration signals such as abnormal query volumes, lateral access, and privilege escalation patterns
- **Real-time alert engine** — low-latency scoring pipeline with configurable risk thresholds
- **Cross-tenant boundary monitoring** — flags inter-tenant access attempts and shared-resource abuse
- **Explainable detections** — SHAP-based feature attribution so analysts understand *why* a flag was raised
- **Evaluation suite** — precision, recall, F1, AUC-ROC, and false-positive rate benchmarks across attack scenarios
- **Modular architecture** — swap classifiers, feature extractors, or alert sinks without touching the core pipeline

---


## Streamlit Dashboard

The interface lets you:

- Upload raw tenant logs or use the bundled sample dataset
- View **live anomaly scores** per tenant in real time
- Inspect **behavioral baselines** and deviation heatmaps
- Drill into flagged events with **SHAP explanation charts**
- Configure alert thresholds and risk sensitivity
- Compare model performance (precision, recall, AUC-ROC) side by side
- Export alert logs and evaluation reports as CSV / PDF

---



## Future Extensions

- Integrate with **live cloud provider APIs** (AWS CloudTrail, Azure Monitor, GCP Audit Logs)
- Add **federated learning** support so tenant models train without sharing raw data
- Build a **graph-based** cross-tenant relationship model for lateral movement detection
- Deploy as a **Kubernetes sidecar** for zero-config cloud-native integration
- Add **streaming mode** via Apache Kafka for sub-second detection latency

---
