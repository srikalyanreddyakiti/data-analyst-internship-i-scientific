# data-analyst-internship-i-scientific

This project was developed during my internship at iScientific Tech and focuses on creating a smart transformer health monitoring system using weighted performance indicators and a calculated Health Index formula. The goal is to assess transformer performance based on key parameters and predict potential failures before they happen.

---

## Overview

Transformers are critical for power transmission. Their failure can lead to large-scale outages and costly repairs. This system calculates a **Transformer Health Index (THI)** using real-time operational data such as:

- Temperature at R, Y, B phases  
- Current at R, Y, B phases  
- Oil temperature  

Each parameter is scored and weighted to produce a single health index value (0 to 1) that indicates the condition of the transformer.

---

## Health Index Formula

The formula used to compute the health index is:

```
Health Index = (0.2 × TR_score) + (0.2 × TY_score) + (0.2 × TB_score) +  
               (0.15 × IR_score) + (0.15 × IY_score) + (0.1 × IB_score) + (0.1 × TO_score)
```

Each indicator is normalized using:

```
Indicator Score = (Value - Min) / (Max - Min)
```

---

## Key Features

- Customizable weights for transformer-specific conditions  
- Health index output to guide predictive maintenance  
- Scalable design for integration with machine learning models  

---

## Contents

- `Transformer Health Index Monitoring Formula - report.pdf` – Detailed technical explanation of the formula  
- `TRANSFORMER HEALTH INDEX.pdf` – Presentation overview with project objectives and potential for AI integration  
- `inventory-website/` – Frontend files (if any) used to visualize transformer data or deploy the solution  

---

## Future Scope

- Integration with AI/ML models to predict Remaining Useful Life (RUL)  
- Real-time dashboard for health monitoring  
- IoT-based sensor integration  

---

## Developed by

**Akiti Sri Kalyan Reddy**  
Data Science and Artificial Intelligence  
