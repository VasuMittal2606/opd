# Historical OPD Dataset

## Overview
This dataset contains historical hospital Outpatient Department (OPD) records. Each row shows how many patients visited a particular department during a particular hour of a given day. It is suitable for analysing patient footfall and for forecasting OPD demand.

- **File:** `historical_opd_dirty_updated.csv`
- **Rows:** about 50,500
- **Columns:** 6
- **Period covered:** 2025 to 2026

## Columns

| Column | Description | Example |
|---|---|---|
| `date` | Calendar date of the record | 2025-08-21 |
| `day_of_week` | Name of the weekday (Monday to Sunday) | Thursday |
| `hour` | Hour of the day (24-hour clock) when the visits were counted | 13 |
| `department` | OPD department the patients visited | Neurology |
| `is_holiday` | Whether the day was a working day (`open`) or a `holiday` | open |
| `patient_count` | Number of patients seen in that department during that hour | 40 |

## Departments
- Cardiology
- Dermatology
- General Medicine
- Neurology
- Orthopedics
- Pediatrics

## Granularity
One row represents one combination of **date + hour + department**.

## Possible Uses
- Studying peak hours and busy weekdays
- Comparing patient load across departments
- Measuring the effect of holidays on OPD visits
- Building demand forecasting models for staffing and resource planning
