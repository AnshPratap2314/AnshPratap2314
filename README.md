<div align="center"><img src="https://capsule-render.vercel.app/api?type=rect&color=0:070B18,45:10264A,100:168BFF&height=190&section=header&text=ANSH%20PRATAP&fontSize=52&fontColor=F8FAFC&fontAlignY=40&desc=AI%2FML-FOCUSED%20SOFTWARE%20DEVELOPER&descSize=17&descAlignY=66&animation=fadeIn" width="100%" alt="Ansh Pratap — AI/ML-focused software developer" />
PYTHON · MACHINE LEARNING · GENERATIVE AI · BACKEND ENGINEERING
I build and test Python/FastAPI backends that add ML and LLM features, with validation, persistence and failure handling built in.

<a href="https://github.com/AnshPratap2314">
  <img src="https://img.shields.io/badge/GitHub-AnshPratap2314-168BFF?style=for-the-badge&logo=github&logoColor=white" alt="GitHub profile" />
</a>
<a href="https://ansh-pratap-developer.ai.studio">
  <img src="https://img.shields.io/badge/PORTFOLIO-Visit-22D3EE?style=for-the-badge&logo=googlechrome&logoColor=07111F" alt="Portfolio" />
</a>
<a href="mailto:shakyaansh9756@gmail.com">
  <img src="https://img.shields.io/badge/CONTACT-Email-FF4655?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
</a></div><div align="center">01 / INTRODUCTION   02 / TECHNICAL ARSENAL   03 / FEATURED BUILDS   04 / EXPERIENCE
</div>01 / MORE THAN JUST CODE
<table>
<tr>
<td width="62%" valign="top">Building intelligent systems with engineering discipline.
I'm a final-year B.Tech Computer Science & Engineering student at Mewar University (2023–2027 expected), focused on AI/ML, Generative AI, Python development and backend engineering.

My work includes a safety-oriented mental health chatbot and an LLM-powered interview platform. Both projects emphasize responsible AI integration: validating model output, handling failure paths, maintaining persistent state and testing system behavior.

I also work with computer vision and NLP, and I'm looking for AI/ML Engineer Intern, Generative AI Engineer Intern, Python Developer, Backend Developer and entry-level Software Engineer opportunities.
</td>
<td width="38%" valign="top">PROFILE SNAPSHOT
FIELD	DETAILS
Education	B.Tech CSE
University	Mewar University
Timeline	2023–2027 (expected)
Focus	AI/ML · GenAI · Backend
Core stack	Python · FastAPI
Engineering	Validation · Persistence · Testing


</td>
</tr>
</table>WHAT I FOCUS ON
<table>
<tr>
<td width="33%" valign="top">01 — INTELLIGENT SYSTEMS

Machine learning, text classification, NLP and LLM-powered application features.
</td>
<td width="33%" valign="top">
02 — BACKEND ENGINEERING

FastAPI, structured APIs, authentication, persistence, rate limiting and input validation.
</td>
<td width="34%" valign="top">
03 — RELIABLE AI

Structured output validation, deterministic safety controls, fallback handling and regression testing.
</td>
</tr>
</table>02 / THE TECHNICAL ARSENAL
<sub>TOOLS CHANGE. THE ENGINEERING FUNDAMENTALS STAY.</sub>
<table>
<tr>
<td width="50%" valign="top">01 — PROGRAMMING LANGUAGES
<img src="https://skillicons.dev/icons?i=python,js,c,cpp&theme=dark" alt="Python, JavaScript, C and C++" />Python JavaScript C C++ SQL
02 — AI / MACHINE LEARNING
<img src="https://skillicons.dev/icons?i=opencv,sklearn&theme=dark" alt="OpenCV and scikit-learn" />scikit-learn TF-IDF Logistic Regression NLP OpenCV face_recognition NumPy Pandas Keras
03 — GENERATIVE AI
Gemini API OpenAI API (optional integration) Prompt Engineering Structured Output Validation
</td>
<td width="50%" valign="top">04 — BACKEND & APIs
<img src="https://skillicons.dev/icons?i=fastapi&theme=dark" alt="FastAPI" />FastAPI REST Pydantic Token Authentication Rate Limiting Input Validation
05 — DATABASES & FRONTEND
<img src="https://skillicons.dev/icons?i=sqlite,html,css,js&theme=dark" alt="SQLite, HTML, CSS and JavaScript" />SQLite HTML CSS Vanilla JavaScript
06 — TESTING & DEVELOPMENT TOOLS
<img src="https://skillicons.dev/icons?i=pytest,git,github,docker&theme=dark" alt="Pytest, Git, GitHub and Docker" />Pytest Git GitHub Docker (basic) Render
07 — ADDITIONAL EXPOSURE
Node.js Express MongoDB RAG fundamentals

<sub>Node.js, Express and MongoDB are listed as exposure through the StudyVerse AI team project.</sub>
</td>
</tr>
</table>03 / FEATURED BUILDS
<sub>FROM PROBLEM DEFINITION TO IMPLEMENTATION — PROJECTS BUILT AROUND PRACTICAL ENGINEERING CHALLENGES.</sub>
01 — MINDCARE AI
A safety-oriented mental health support chatbot

A chatbot designed around a key constraint: risk decisions must remain deterministic, while ML and LLM components are used only where appropriate.
<p>
<a href="https://mindcare-ai-o1e5.onrender.com"><img src="https://img.shields.io/badge/LIVE_DEMO-168BFF?style=for-the-badge&logo=render&logoColor=white" alt="MindCare AI live demo" /></a>
<a href="https://github.com/AnshPratap2314/AI-Mental-health-chatbot"><img src="https://img.shields.io/badge/SOURCE_CODE-263B60?style=for-the-badge&logo=github&logoColor=white" alt="MindCare AI source code" /></a>
</p>
Python FastAPI scikit-learn TF-IDF Docker Render
<table>
<tr>
<td width="50%" valign="top">
ENGINEERING FEATURES
- A rule-based behavior/risk engine is authoritative.
- High-risk messages never reach the LLM.
- The trained model's risk output is never used for safety decisions.
- TF-IDF + Logistic Regression response model trained on a 50,000-message synthetic dataset covering 20 intents in English and Hinglish.
- Predicts intent, mood, topic and risk.
</td>
<td width="50%" valign="top">VALIDATION & HARDENING
- Train, validation and test splits.
- Duplicate and leakage audits.
- Hard-negative and challenge-case scripts.
- Session management and CORS validation.
- Authenticated audit endpoint.
- 200+ pytest tests covering safety, sessions and API security.
</td>
</tr>
</table>THE ENGINEERING CHALLENGE

An LLM can produce an unsafe reply to a message in crisis. MindCare makes the risk decision first using deterministic rules, then gates LLM use behind that decision. If the LLM is disabled, errors, or returns invalid output, the system falls back to the trained response model and templates.
<details>
<summary><strong>VIEW REQUEST FLOW</strong></summary>```mermaid
flowchart TD
    A[Incoming message] --> B[Validate input]
    B --> C[Deterministic risk analysis]
    C --> D{High risk?}
    D -- Yes --> E[Deterministic safety response]
    D -- No --> F{LLM enabled?}
    F -- Yes --> G[LLM response]
    F -- No --> H[Trained response model]
    G -- Error or invalid output --> H
    H --> I[Response]
    E --> I
```
</details><sub>DATA & SAFETY NOTE: Uses synthetic, non-clinical data. Not clinically validated and not a medical or diagnostic tool.</sub>
02 — AI INTERVIEW SIMULATOR
An interview practice platform with LLM-based answer evaluation, persistent sessions and job-description analysis.
<p>
<a href="https://ai-based-interview-simulator-1.onrender.com/"><img src="https://img.shields.io/badge/LIVE_DEMO-168BFF?style=for-the-badge&logo=render&logoColor=white" alt="AI Interview Simulator live demo" /></a>
<a href="https://github.com/AnshPratap2314/ai-based-interview-simulator"><img src="https://img.shields.io/badge/SOURCE_CODE-263B60?style=for-the-badge&logo=github&logoColor=white" alt="AI Interview Simulator source code" /></a>
</p>
Python FastAPI Pydantic SQLite Gemini API JavaScript
<table>
<tr>
<td width="50%" valign="top">
INTERVIEW INTELLIGENCE
- Gemini evaluates answers against a Pydantic schema.
- Deterministic checks flag very short, off-topic or language-mismatched answers and inconsistent scores for human review.
- Adaptive question difficulty uses a rolling average of recent scores.
- Curated question bank across Technical, HR and AI/ML tracks, with three difficulty levels.
- Job-description and résumé analysis extracts requirements and builds a personalized question plan.
</td>
<td width="50%" valign="top">STATE, SECURITY & TESTING
- SQLite-backed interview state and candidate history.
- Separate candidate and session credentials with expiry.
- Rate limiting with Retry-After.
- Evaluation requests are idempotent through an X-Evaluation-Id header.
- Provider retries are limited to transient errors.
- 76 pytest tests using a fake Gemini client; no API key required.
</td>
</tr>
</table>THE ENGINEERING CHALLENGE

LLM output can be malformed, and network retries can double-score an answer. The platform validates and rejects malformed output, retries providers only for transient errors, and uses idempotent evaluation requests to prevent duplicate scoring.
<details>
<summary><strong>VIEW SYSTEM ARCHITECTURE</strong></summary>```mermaid
flowchart TD
    A[Browser UI] --> B[FastAPI]
    B --> C[Authentication, expiry and rate limiting]
    C --> D[Interview engine and adaptive difficulty]
    C --> E[Gemini evaluation]
    E --> F[Pydantic validation and review flags]
    D --> G[(SQLite)]
    F --> G
```
</details>03 — STUDYVERSE AI
An AI learning workspace — team project

A learning workspace where students can chat with an AI tutor, generate study packs, flashcards and quizzes, and ask questions over uploaded documents.
<p>
<a href="https://study-verse-ai-eight.vercel.app/"><img src="https://img.shields.io/badge/LIVE_DEMO-168BFF?style=for-the-badge&logo=vercel&logoColor=white" alt="StudyVerse AI live demo" /></a>
<a href="https://github.com/AnshPratap2314/StudyVerse-AI"><img src="https://img.shields.io/badge/SOURCE_CODE-263B60?style=for-the-badge&logo=github&logoColor=white" alt="StudyVerse AI source code" /></a>
</p>
Node.js Express MongoDB JavaScript Gemini OpenAI Groq
<table>
<tr>
<td width="50%" valign="top">
AI & DOCUMENT WORKFLOWS
- Multi-provider AI gateway across Gemini, OpenAI and Groq.
- Role-based agents: router, researcher, teacher, critic and synthesizer.
- Document Q&A using processing and retrieval over uploaded study material.
</td>
<td width="50%" valign="top">ACCOUNTS & QUALITY
- JWT authentication with hashed passwords.
- Mongoose models and per-user data isolation.
- Five backend test files covering security regression, data isolation and API contracts.
</td>
</tr>
</table>04 — AISHIE
Voice-controlled desktop assistant — macOS prototype
<p>
<a href="https://github.com/AnshPratap2314/Aishie-AI-Assistant"><img src="https://img.shields.io/badge/SOURCE_CODE-263B60?style=for-the-badge&logo=github&logoColor=white" alt="Aishie source code" /></a>
</p>
Python SpeechRecognition OpenCV face_recognition PyAutoGUI AppleScript
- Face-recognition gate using face embeddings and distance thresholds before the assistant starts.
- Installed-app monitoring with watchdog, including a change log and a voice command to query it.
- JSON-based memory and messaging through AppleScript.
- Requires internet access for Google speech recognition and Wikipedia, and macOS for automation features.
THE ENGINEERING CHALLENGE

Spoken transcripts are noisy, so exact string matching can miss commands. Wake-word detection and command routing use fuzzy matching to tolerate recognition errors.
04 / HOW THE SYSTEMS ARE BUILT
<sub>IMPLEMENTATION PATTERNS VISIBLE IN THE PROJECTS ABOVE.</sub>
<div align="center"><table>
<tr>
<td align="center" width="25%">
01
DEFINE
Identify the input, requirements and constraints.
</td>
<td align="center" width="25%">
02
ENGINEER
Build APIs, application logic and persistence.
</td>
<td align="center" width="25%">
03
VALIDATE
Validate structured output and test failure paths.
</td>
<td align="center" width="25%">
04
DELIVER
Deploy the application and expose its workflow.
</td>
</tr>
</table></div>EXAMPLES FROM MY PROJECTS
- MindCare AI: deterministic risk analysis → gated LLM response → trained-model/template fallback.
- AI Interview Simulator: authenticated request → interview/evaluation logic → schema validation and review flags → persistent SQLite state.
- StudyVerse AI: multi-provider AI gateway → role-based agents → document retrieval and Q&A.
- Aishie: speech input → fuzzy command matching → desktop automation.
05 / EXPERIENCE & BUILDER CREDENTIALS
<sub>LEARNING THROUGH TRAINING, EXPERIMENTATION AND PROJECT WORK.</sub>
<table>
<tr>
<td width="50%" valign="top">AI INTERN
Internship Studio (iStudio)

OCT 2025 — JAN 2026
- Automated recurring data-preprocessing steps in a training pipeline with Python.
- Redesigned LLM prompt templates to enforce a structured output schema.
- Used exploratory data analysis to identify label noise and class imbalance ahead of deployment.
</td>
<td width="50%" valign="top">AI & ML INDUSTRIAL TRAINEE
CTTC Bhubaneswar

APR — MAY 2025
- Built a face detection and recognition attendance system using OpenCV, SVM and LBPH on a self-collected dataset.
- Benchmarked SVM, KNN, Decision Tree and Neural Network classifiers on identical data.
</td>
</tr>
</table>EDUCATION
B.Tech — Computer Science & Engineering

Mewar University · 2023–2027 (expected)
CERTIFICATIONS
<table>
<tr>
<td>Google AI Essentials</td>
<td>Google Prompting Essentials</td>
</tr>
<tr>
<td>IBM SkillsBuild: AI Fundamentals</td>
<td>HP LIFE: Data Science & Analytics</td>
</tr>
</table>06 / GITHUB DEVELOPER DASHBOARD
<sub>A LIVE VIEW OF MY PUBLIC GITHUB PROFILE.</sub>
<div align="center"><img src="https://github-readme-stats.vercel.app/api?username=AnshPratap2314&show_icons=true&hide_border=true&bg_color=070B18&title_color=168BFF&icon_color=22D3EE&text_color=F8FAFC&ring_color=A855F7" height="170" alt="GitHub profile statistics for AnshPratap2314" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=AnshPratap2314&layout=compact&hide_border=true&bg_color=070B18&title_color=168BFF&text_color=F8FAFC" height="170" alt="Most-used languages in public repositories" />
<img src="https://streak-stats.demolab.com?user=AnshPratap2314&hide_border=true&background=070B18&ring=168BFF&fire=FF4655&currStreakLabel=22D3EE&sideLabels=A7B4CC&currStreakNum=F8FAFC&sideNums=F8FAFC&dates=7C8BA5" width="80%" alt="GitHub contribution streak for AnshPratap2314" />
<img src="https://github-readme-activity-graph.vercel.app/graph?username=AnshPratap2314&bg_color=070B18&color=F8FAFC&line=168BFF&point=22D3EE&area=true&hide_border=true" width="100%" alt="GitHub contribution activity graph for AnshPratap2314" /></div><sub>Language percentages reflect repository size, not overall skill. These cards are generated dynamically by third-party services and may occasionally be unavailable.</sub>
07 / LET'S BUILD SOMETHING GREAT.
<div align="center">OPEN TO INTERNSHIPS, ENTRY-LEVEL ROLES & COLLABORATION
Ideas, opportunities and thoughtful engineering — let's connect.

<a href="https://ansh-pratap-developer.ai.studio"><img src="https://img.shields.io/badge/PORTFOLIO-Visit%20Portfolio-168BFF?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Visit portfolio" /></a>
<a href="https://linkedin.com/in/ansh-pratap-68156625b"><img src="https://img.shields.io/badge/LINKEDIN-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="Connect on LinkedIn" /></a>
<a href="https://github.com/AnshPratap2314"><img src="https://img.shields.io/badge/GITHUB-Explore%20Projects-263B60?style=for-the-badge&logo=github&logoColor=white" alt="Explore GitHub projects" /></a>
<a href="mailto:shakyaansh9756@gmail.com"><img src="https://img.shields.io/badge/EMAIL-Get%20in%20Touch-FF4655?style=for-the-badge&logo=gmail&logoColor=white" alt="Send an email" /></a>



Curious by default. Building with intent.
</div>
