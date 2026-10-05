# NagarDrishti 

### AI-Powered Civic Governance & Citizen Feedback Platform

> **Speak. Track. Verify. Measure.**

**Team:** Citecks  
**Hackathon:** HackSprint 2026  
**Track:** Track 04 — PS 41

NagarDrishti is an Applied AI civic-tech platform designed to connect citizens, civic projects, and governance monitoring through Indian-language voice interaction.

The platform enables citizens to report civic issues through voice, converts their speech into structured feedback using AI, links complaints to relevant local projects, tracks project/complaint status, and allows citizens to verify whether an officially resolved issue was actually fixed.

---

## 🧠 Tech Stack

### AI & Language — **Sarvam AI**
- **Sarvam Saarika** — Speech-to-Text
- **Sarvam Translate / LLM** — Translation & language understanding
- **Sarvam Bulbul** — Text-to-Speech
- Indian-language & code-mixed voice processing

### AI Application Layer
- **Spring AI** — AI orchestration and prompt workflows
- Structured AI output
- Complaint classification
- Information extraction
- Duplicate complaint detection / clustering
- AI-assisted governance insights

### Backend
- **Java**
- **Spring Boot**
- **Spring Security**
- **JWT Authentication**
- REST APIs
- Business & governance workflows

### Frontend
- **React.js**
- **Leaflet** — Project/location visualization
- **Chart.js / Recharts** — Governance analytics

### Database & Storage
- **PostgreSQL** — Users, projects, complaints, status history, verification and analytics
- **Object Storage / Local Storage** — Voice recordings

### DevOps & Deployment
- **Docker**
- **Cloud Deployment**
- **Git & GitHub**

---

## 🏗️ Architecture

```text
                    🎙️ CITIZEN
                         │
                  Voice Feedback
                         │
                         ▼
              ┌─────────────────────┐
              │     🧠 SARVAM AI    │
              │                     │
              │  Saarika STT        │
              │  Translate / LLM    │
              │  Bulbul TTS         │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │      SPRING AI      │
              │                     │
              │ AI Orchestration    │
              │ Prompt Workflows    │
              │ Structured Output   │
              └──────────┬──────────┘
                         │
                         ▼
              ┌─────────────────────┐
              │    JAVA + SPRING    │
              │       BOOT          │
              │                     │
              │ REST APIs           │
              │ Complaint Workflow  │
              │ Project Monitoring  │
              │ Citizen Verification│
              │ Trust Gap           │
              └──────────┬──────────┘
                         │
                  ┌──────┴──────┐
                  ▼             ▼
           PostgreSQL      Spring Security
                           + JWT
                  │
                  ▼
             React Frontend
                  │
          ┌───────┴────────┐
          ▼                ▼
      Citizen UI       Officer Dashboard
