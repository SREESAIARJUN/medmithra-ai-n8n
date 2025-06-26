
# 🩺 MedMithra AI – Clinical Insight Assistant (n8n WhatsApp Workflow)

Welcome to the official n8n workflow powering **MedMithra AI**, a multimodal clinical assistant that lets doctors **analyze cases, labs, audio notes, and radiology images** directly via WhatsApp.

---

## 🚀 Features

This n8n workflow enables seamless real-time clinical interactions with MedMithra AI over WhatsApp. The backend pipeline supports:

### 🧠 AI-Powered Analysis
- GPT-4o/Whisper/Vision via OpenAI API
- Auto-generates SOAP notes, differential diagnoses, investigations & treatments
- Supports natural language + audio dictation input

### 📎 Multimodal Input Support
- 📝 Text (typed or dictated)
- 📄 PDFs, CSVs, and other lab documents (via WhatsApp document upload)
- 🖼️ Radiology images (JPG/PNG/DICOM)
- 🎤 Audio clips (converted to text with Whisper)

### 🔄 Smart Orchestration
- AI assistant context handling with memory
- Command routing via Switch and Condition logic
- Auto-generates concise text and optional audio responses
- Optional PDF generation of the AI-generated clinical summary

---

## 🛠️ Workflow Overview

- `WhatsApp Trigger`: Starts when a message is received on WhatsApp
- `Check Input Type`: Detects message type (Text, Image, Audio, Document)
- `Formatter Nodes`: Format inputs for AI use
- `AI Clinical Assistant`: GPT-4o model orchestrator
- `Media Handling`: Downloads, analyzes, and parses attachments
- `PDF Generator`: Converts output to printable format
- `Text & Audio Responder`: Sends back human + voice reply

---

## 📱 Access MedMithra on WhatsApp

> **🔵 LIVE BOT:**  
Chat with the AI directly at  
👉 **+1 555 630 0396**

> **🔐 Want access to the development/test instance?**  
Message **+91-7013889449** on WhatsApp  
Include your **name and phone number** to request access.

---

## 🧾 Output Format

The assistant returns a structured JSON response with:
```json
{
  "soap_note": {
    "subjective": "...",
    "objective": "...",
    "assessment": "...",
    "plan": "..."
  },
  "differential_diagnoses": [],
  "recommended_investigations": [],
  "treatment_options": [],
  "file_interpretations": [],
  "overall_confidence_score": 0.94,
  "text_reply": "..."
}
```

---

## 🧩 Tech Stack

| Component        | Tech Used               |
|------------------|-------------------------|
| Messaging        | WhatsApp Cloud API      |
| Orchestration    | n8n Workflow Automation |
| AI Inference     | OpenAI GPT-4o, Whisper  |
| File Handling    | HTTP / Cloud Downloads  |
| Output Delivery  | WhatsApp Replies (Text & Audio) |
| PDF Rendering    | HTML-to-PDF Generator   |

---

## 📎 Tags

`#healthcare` `#multimodal` `#whatsapp` `#n8n` `#ai-assistant` `#clinical`

---

## 📞 Support

If you face issues with the workflow or want to extend it:
- Ping @Arjun via WhatsApp: +91-7013889449
- Or raise a GitHub issue if integrated into a public repo

---

MedMithra AI is designed to **speed up clinical workflows**, **reduce cognitive load**, and offer a **natural assistant for modern doctors.**
