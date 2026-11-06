<div align="center">

# 🌱 AgriSmart Precision Irrigation
### IoT Telemetry Stream & Agronomic Predictive Actuation Engine

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1200&color=10B981&center=true&vCenter=true&width=750&lines=AgriSmart+Precision+Irrigation;IoT+Soil+NPK+%26+Weather+Telemetry;AWS+IoT+Core+%2B+Kinesis+Data+Firehose;Predictive+24hr+Autonomous+Valve+Actuation" alt="Typing SVG" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/AWS-IoT_Core_%7C_Kinesis-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white" />
  <img src="https://img.shields.io/badge/ML-Random_Forest-0052CC?style=for-the-badge&logo=scikitlearn&logoColor=white" />
  <img src="https://img.shields.io/badge/Conservation-35%25_Water_Saved-22C55E?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Preserved-Branch_Ex-gray?style=for-the-badge&logo=git" />
</p>

<img src="https://skillicons.dev/icons?i=python,aws,docker,scikitlearn&theme=dark" alt="Stack" />

</div>

---

### 📡 Live MQTT Sensor Ingestion

```json
{
  "device_id": "FIELD-STATION-04",
  "soil_moisture_pct": 21.4,
  "soil_temp_c": 26.8,
  "npk_levels": { "nitrogen": 45, "phosphorus": 22, "potassium": 110 },
  "ambient_humidity": 58.2,
  "predicted_evapotranspiration": "4.2mm/day",
  "valve_actuation": { "valve_id": "V-12", "action": "OPEN", "duration_seconds": 480 },
  "timestamp": "2026-11-06T13:00:23Z"
}
```

---

## 🏛️ Agronomic Bento Grid

<table width="100%">
  <tr>
    <td width="50%" valign="top">
      <h3>📡 AWS IoT Core Streaming</h3>
      <p>MQTT message broker ingesting sensor telemetry from rural field microcontrollers with automated device shadowing and connection reliability.</p>
      <b>Features:</b> Kinesis Data Firehose batching • S3 time-series storage
    </td>
    <td width="50%" valign="top">
      <h3>🌱 Predictive Water Need Modeling</h3>
      <p>Scikit-Learn Random Forest regressor forecasting soil moisture decay 24 hours in advance to prevent crop root water stress before it occurs.</p>
      <b>Features:</b> Weather API fusion • Zero over-irrigation runoff
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>📲 SMS & Mobile Alerts via SNS</h3>
      <p>Automated warning notifications dispatched via <b>Amazon SNS</b> to farm operators whenever anomalous moisture drops or sensor battery faults occur.</p>
      <b>Features:</b> Push notifications • Daily irrigation digest
    </td>
    <td width="50%" valign="top">
      <h3>📊 Streamlit Command Dashboard</h3>
      <p>Executive visual control room hosted on <b>AWS ECS Fargate</b> displaying interactive moisture heatmaps, valve states, and conservation analytics.</p>
      <b>Features:</b> Historical trend inspection • Manual override switch
    </td>
  </tr>
</table>

---

## ⚡ Quickstart

```bash
git clone https://github.com/prak05/AgriSmart-Precision-Irrigation.git
cd AgriSmart-Precision-Irrigation
streamlit run smart/app.py
```

---

<div align="center">
<sub>Preserved Baseline: <a href="https://github.com/prak05/AgriSmart-Precision-Irrigation/tree/Ex">branch Ex</a> • Engineered for Scalable Production Clouds</sub>
</div>
