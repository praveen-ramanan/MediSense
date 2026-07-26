# MediSense

> Know Your Medicines. Reduce Your Risks.

MediSense is a medication safety assistant that helps patients and caregivers identify potential drug-drug interactions from prescriptions using a deterministic interaction engine and plain-language explanations.

Unlike systems that rely on LLMs for medical reasoning, MediSense performs interaction detection through a curated drug interaction dataset. The LLM is used only to explain verified interactions in a patient-friendly manner.

---

## Problem

Patients taking medicines from multiple doctors or pharmacies often face the risk of harmful drug interactions.

Manually checking every prescription is time-consuming, and most patients have no accessible way to verify potential interactions before taking their medications.

---

## Solution

MediSense allows users to:

- Create a patient profile
- Upload or type prescriptions
- Extract medicines using OCR
- Normalize brand names to generic names
- Detect known drug interactions
- Receive easy-to-understand explanations
- Clearly distinguish between known interactions and unknown combinations

---

## Features

- Patient profile management
- Prescription image upload
- OCR-based medicine extraction
- Brand → Generic medicine normalization
- Deterministic drug interaction lookup
- Context-aware plain-language explanations
- Explicit handling of unknown interactions
- Risk-level visualization
- Safety-first design

---

## System Architecture

![Architecture](docs/architecture.png)

---

## Tech Stack

### Frontend
- React
- Next.js

### Backend
- FastAPI

### AI
- Gemini API (Explanation only)

### OCR
- Tesseract OCR

### Data Processing
- RapidFuzz
- Brand-to-generic lookup

### Dataset
- Curated Drug Interaction Dataset (JSON/CSV)

---

## Workflow

Patient Profile

↓

Prescription Upload / Manual Entry

↓

OCR

↓

Medicine Name Normalization

↓

Drug Interaction Lookup

↓

Context-Aware Explanation

↓

Risk Report

---

## Future Scope

- Drug-condition contraindication checking
- Drug-allergy detection
- Medication reminder system
- Doctor dashboard
- Electronic Health Record integration
- Multi-language support

---

## Disclaimer

MediSense is intended as an educational and decision-support tool.

It does **not** replace professional medical advice, diagnosis, or treatment.

Always consult a qualified healthcare professional before making medication decisions.

---

<img width="1236" height="806" alt="image" src="https://github.com/user-attachments/assets/6b10f72b-ad37-4755-a5be-659ffed6a40d" />
<img width="742" height="817" alt="image" src="https://github.com/user-attachments/assets/e994292b-7c78-464a-bdd0-60364db63095" />

