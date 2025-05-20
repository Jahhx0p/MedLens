# 💊 MedLens

**MedLens** is a smart assistant that scans a user's list of medications—either entered manually or extracted via image recognition from prescription labels—and checks for potential drug interactions and side effects. It cross-references with medical databases like **DrugBank** and **openFDA**, and uses NLP to explain the results in user-friendly language.

Designed to support safe medication management, MedLens helps users understand their prescriptions, flag dangerous combinations, and make informed decisions with accessible, AI-powered insights.

## 📌 Features

- 📷 **Medication Input & Recognition**:
  - Manual entry or OCR-based extraction from prescription labels
  - Auto-suggest and autocomplete for drug names
  - Supports multiple input languages and formats

- ⚠️ **Drug Interaction Detection**:
  - Cross-references drug combinations using DrugBank/openFDA APIs
  - Identifies interaction severity: minor, moderate, severe
  - Lists contraindications and redundant medications

- 🧠 **NLP-Powered Explanations**:
  - Summarizes side effects, usage warnings, and interactions
  - Converts clinical terms into plain-language descriptions
  - Highlights urgent risks with clear visual cues

- 📖 **Medication Insights & History**:
  - Stores user medication profiles locally or securely in the cloud
  - Tracks changes in prescriptions over time
  - Offers reminders and optional journaling for effects tracking

- 🔐 **Privacy & Security**:
  - No health data stored without user consent
  - OCR and analysis can run entirely on-device
  - End-to-end encryption for all synced data

## 🛠️ Tech Stack

- **Frontend**: React Native, Expo, React Navigation
- **Backend**: Python (Flask), Node.js (Express)
- **AI & NLP**: spaCy, OpenAI API, Tesseract.js for OCR
- **APIs**: DrugBank, openFDA
- **Storage**: SQLite (mobile), Firebase (optional sync)
- **Security**: HTTPS, OAuth2, AES encryption

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- Python 3.9+
- Expo CLI
- DrugBank/openFDA API keys

### Clone & Run

```bash
git clone https://github.com/your-username/medlens.git
cd medlens
npm install
npx expo start
