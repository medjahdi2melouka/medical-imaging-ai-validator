## ⚙️ Setup Instructions

### 1. Create Webhook Endpoint (n8n)

In n8n:

- Create a new workflow
- Add a **Webhook node**
- Set:
  - Method: POST
  - Path: medical-imaging-validation
- Activate the workflow

Your endpoint will look like:

https://YOUR-N8N-URL/webhook/medical-imaging-validation


---

### 2. Connect Email (Gmail)

To enable email notifications:

- Add a **Gmail node** in n8n
- Connect your Gmail account using OAuth2
- Set:
  - To: your email or dynamic user email
  - Subject: Validation Result
  - Message: formatted output from workflow

---

### 3. How to Use the API

Send a POST request:

```json id="req1"
{
  "patient_id": "001",
  "study_date": "20230101",
  "modality": "MRI"
}
```

