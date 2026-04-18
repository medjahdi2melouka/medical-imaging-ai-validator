# API Documentation - Medical Imaging AI Validator

## Overview
This API validates medical imaging metadata (MRI, CT, PET, XRAY) and returns clean structured results.

---

## Endpoint

POST /webhook/medical-imaging-validation

---

## Input Format

### Single Record

```json
{
  "patient_id": "001",
  "study_date": "20230101",
  "modality": "MRI"
}

