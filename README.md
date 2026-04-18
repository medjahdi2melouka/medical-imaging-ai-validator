# Medical Imaging Validation API (n8n)

AI-powered data validation workflow for medical imaging metadata (MRI, CT, PET, XRAY).

---

##  Features
- Validates medical imaging metadata
- Detects missing fields
- Checks modality type
- Detects duplicate records
- Returns structured clean JSON

---

##  API Usage

### Endpoint
POST /webhook/medical-imaging-validation

---

##  Input Example

```json
{
  "patient_id": "001",
  "study_date": "20230101",
  "modality": "MRI"
}