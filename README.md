# AgriSmart Precision Irrigation — IoT Telemetry & Agronomic AI

[![AWS IoT Core](https://img.shields.io/badge/AWS-IoT%20Core%20%7C%20Kinesis-FF9900?logo=amazon-aws&logoColor=white)](#aws-cloud-architecture)
[![Machine Learning](https://img.shields.io/badge/AI-Random%20Forest%20%7C%20Scikit-0052CC)](#iot--ml-pipeline)
[![Branch Status](https://img.shields.io/badge/Preservation-Ex%20Branch-22C55E)](#branch-architecture)
[![License: MIT](https://img.shields.io/badge/License-MIT-gray.svg)](LICENSE)

> IoT-driven soil telemetry, evapotranspiration modeling, and automated valve actuation system delivering optimized water conservation for precision agriculture.

---

## 1. Executive Brief
Over-irrigation depletes water tables and leaches vital soil nitrogen. **AgriSmart Precision Irrigation** continuously streams moisture, temperature, humidity, and rainfall readings to predict water requirements 24-hours ahead, automating solenoid valve relays with zero manual intervention.

* **Preservation**: Original AICTE/Edunet project preserved on [`Ex`](https://github.com/prak05/AgriSmart-Precision-Irrigation/tree/Ex).
* **Cloud Architecture**: AWS IoT Core telemetry ingestion, Amazon Kinesis Firehose, and Streamlit executive dashboard.

---

## 2. AWS Cloud Architecture

```mermaid
flowchart TD
    Sensors["Soil NPK, Moisture & Weather Sensors"] --> IoTCore["AWS IoT Core (MQTT Broker)"]
    IoTCore --> Firehose["Amazon Kinesis Data Firehose"]
    Firehose --> S3Lake["Amazon S3 (Telemetry Time-Series Lake)"]
    IoTCore --> LambdaRules["AWS Lambda (Threshold & Anomaly Detector)"]
    LambdaRules --> SNSAlert["Amazon SNS (SMS & Mobile Alerts to Farmers)"]
    S3Lake --> Athena["Amazon Athena (Aggregated Analytics)"]
    Athena --> Streamlit["Streamlit Dashboard (AWS ECS Fargate)"]
    LambdaRules --> Valve["Edge Microcontroller (Relay Valve Actuator)"]
```

---

## 3. Branch Architecture
* [`main`](https://github.com/prak05/AgriSmart-Precision-Irrigation/tree/main): IoT Core telemetry pipeline with AWS Lambda automation.
* [`Ex`](https://github.com/prak05/AgriSmart-Precision-Irrigation/tree/Ex): Preserved student project prototype.
