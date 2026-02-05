# 🧠 Niti-Setu  
### Voice-Based Scheme Eligibility Engine for Farmers

---

## 📌 Problem Overview

Every year, the Government of India launches **100+ agricultural schemes** with a combined budget exceeding **₹50,000 crores**.  
However, **less than 30% of eligible farmers** successfully access these benefits.

### Key Challenges
- Scheme guidelines buried inside long, complex PDF documents
- Eligibility rules written in bureaucratic language
- No personalized eligibility guidance
- High rejection rate due to incorrect or incomplete applications

---

## 🎯 Project Goal

**Niti-Setu** converts complex government scheme PDFs into **simple, personalized Yes/No eligibility decisions with official proof**, using voice-based interaction.

> From “reading 50-page PDFs” →  
> **“Speak your details and get verified eligibility in seconds.”**

---

## 🧩 System Overview

Farmer Voice Input
↓
Speech-to-Text
↓
Structured Farmer Profile
↓
RAG Engine (PDF + LLM)
↓
Eligibility Decision
↓
Proof Card + Next Steps

---

## 🔑 Key Features *(Phase 1 – MVP)*

### 1️⃣ Voice-Enabled Farmer Profile Input *(Phase 1)*

- Voice input (Hindi / English)
- Manual form fallback
- Captured details:
  - State
  - District
  - Land holding (acres/hectares)
  - Crop type
  - Social category
- Output: Structured farmer profile stored in database

---

### 2️⃣ Scheme PDF Ingestion & Processing *(Phase 1)*

- Upload official government scheme PDFs
- Text extraction and chunking
- Vector embedding generation
- Focus on:
  - Eligibility criteria
  - Beneficiary definitions
  - Exclusions

**Supported Schemes (MVP):**
- PM-KISAN  
- PM-KUSUM  
- Agri-Infrastructure Fund  

---

### 3️⃣ RAG-Based Eligibility Engine *(Phase 1)*

- Retrieval-Augmented Generation using LangChain
- Semantic search over scheme PDFs
- Farmer profile matched against eligibility rules
- Binary output:
  - ✅ Eligible
  - ❌ Not Eligible

---

### 4️⃣ Proof Card Generator *(Phase 1)*

Each eligibility check generates a **Proof Card** containing:

- Eligibility status (e.g., Eligible for ₹6,000/year)
- Exact document proof snippet
- Page number and paragraph citation
- Next steps for application
- Required document checklist (basic)

---

### 5️⃣ User Dashboard *(Phase 1)*

- Farmer profile summary
- List of applicable schemes
- Expandable proof and citations
- Impact metrics:
  - Schemes analyzed
  - Eligibility checks performed
  - Average response time

---

## 🚀 Level-Up Features *(Phase 2)*

### 🔹 Multilingual Text-to-Speech *(Phase 2)*
- Read results aloud in:
  - Hindi
  - Marathi
  - Tamil

---

### 🔹 Document Checklist Generator *(Phase 2)*
- Auto-generate required documents per scheme
- Reduce application rejection rates

---

### 🔹 Scheme Comparison Engine *(Phase 2)*
- Compare benefits across eligible schemes
- Recommend the best scheme for the farmer

---

## ⚙️ Tech Stack

### Backend
- Node.js
- Express.js
- MongoDB (including vector storage)

### AI / ML
- LangChain (RAG orchestration)
- LLM: OpenAI / Gemini / LLaMA
- Embeddings:
  - text-embedding-ada-002
  - sentence-transformers

### Speech
- Web Speech API
- Google Cloud Speech-to-Text (optional)

### Frontend
- React.js
- Browser SpeechRecognition API

---

## 📊 Implementation Status

| Module | Description | Status |
|------|------------|--------|
| Problem Analysis | Scheme understanding & user pain points | ✅ Completed |
| Feature Design | Phase 1 & Phase 2 feature planning | ✅ Completed |
| Architecture Design | End-to-end system workflow | ✅ Completed |
| PDF Ingestion Pipeline | Text extraction & chunking | ⏳ Planned |
| RAG Engine | Eligibility matching logic | ⏳ Planned |
| Voice Input Module | Speech-to-text integration | ⏳ Planned |
| Proof Card UI | Eligibility proof visualization | ⏳ Planned |
| User Dashboard | Profile & scheme display | ⏳ Planned |
| Level-Up Features | Phase 2 enhancements | ⏳ Planned |

---

## 🧪 Validation Plan

- Test with **10 real farmer profiles**
- Manual verification against official PDFs
- Measure:
  - Accuracy of eligibility decisions
  - Response time (<10 seconds target)
  - Explanation clarity

---

## 📈 Expected Impact

- Improved scheme awareness
- Reduced eligibility confusion
- Lower application rejection rates
- Increased trust through document-backed decisions

---

## 📂 GitHub Repository Plan

**Current:**
- Project documentation
- Feature roadmap
- Architecture design

**Future:**
- Backend APIs
- PDF ingestion & RAG engine
- Frontend dashboard
- Voice interface integration

---

## 🏁 Conclusion

**Niti-Setu** acts as a **digital consultant for farmers**, transforming government bureaucracy into an accessible, voice-driven, and trustworthy experience.

---
