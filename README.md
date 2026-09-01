# S-CALIBER

Official dataset and implementation for:

**S-CALIBER: Microscopic Requirement-Aware Efficient and Reliable Sensor Calibration**

S-CALIBER is a lightweight Transformer-based sensor calibration framework designed for accurate, efficient, and reliable on-device inference under resource-constrained environments.

## Repository Contents

This repository provides:

- **Outdoor Dataset**  
  SensEURCity-based calibration data from **Antwerp, Oslo, and Zagreb**, including PM10, PM2.5, and PM1 measurements.

- **Indoor Dataset**  
  A self-collected long-term indoor sensor dataset containing approximately **148K 1-minute samples** collected over approximately **15 weeks**.

- **S-CALIBER Code**  
  Implementation of the proposed S-CALIBER model and experimental pipeline.

## Dataset Download

The complete dataset used in our experiments, including both **Outdoor** and **Indoor** data, is also available separately on Google Drive:

**[Download S-CALIBER Dataset (Google Drive)](https://drive.google.com/file/d/1Rwwam6iDixXF3lJlwzpNL7-D50cbx2ch/view)**

## Dataset

### Outdoor

The outdoor experiments use the **SensEURCity** dataset with co-located low-cost and reference sensors from:

`Antwerp` · `Oslo` · `Zagreb`

Targets:

`PM10` · `PM2.5` · `PM1`

### Indoor

The indoor dataset was collected in a laboratory environment from **January 22, 2026 to May 5, 2026**.

Calibration targets and sensor pairs are:

| Target | Low-Cost Sensor | Reference / Proxy Sensor |
|---|---|---|
| PM1 | PPD42NS | PMS7003 |
| CO | MQ135 | MQ9 |
| CO₂ | MQ135 | MG811 |
| Temperature | DHT11 | DHT22 |
| Humidity | DHT11 | DHT22 |

Raw measurements were collected at approximately **1 Hz** and resampled to **1-minute intervals**, resulting in approximately **148K samples**.

## S-CALIBER

S-CALIBER consists of three main components:

- **Sequence Lens Projector (SLP)** — efficient time-series compression
- **Efficient Bitwise Attention (EBA)** — lightweight hash-based attention
- **Stable Hash Optimization** — efficient and stable binary hash learning

The model is designed to jointly consider seven deployment-oriented requirements covering **accuracy, real-time performance, and resource efficiency**.

## Citation

If you use this dataset or code in your research, please cite:

> **S-CALIBER: Microscopic Requirement-Aware Efficient and Reliable Sensor Calibration**

Citation information will be updated upon publication.

## License

Please refer to the repository license for usage conditions.
