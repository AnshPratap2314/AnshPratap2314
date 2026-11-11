<div align="center"><img width="100%" src="https://capsule-render.vercel.app/api?type=rect&color=0:050816,45:101B3D,100:063B75&height=190&section=header&text=ANSH%20PRATAP&fontSize=48&fontColor=FFFFFF&fontAlignY=38&desc=AI%2FML%20%7C%20GENERATIVE%20AI%20%7C%20SOFTWARE%20ENGINEERING&descSize=15&descAlignY=64" alt="Ansh Pratap — AI/ML and software engineering" /><a href="https://github.com/AnshPratap2314">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=17&duration=2800&pause=900&color=38BDF8&center=true&vCenter=true&width=700&lines=Building+useful+AI-powered+products;Python+%7C+FastAPI+%7C+Machine+Learning;From+curiosity+to+working+software" alt="Typing introduction" />
</a>
<a href="https://linkedin.com/in/ansh-pratap-68156625b"><img src="https://img.shields.io/badge/LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="https://github.com/AnshPratap2314"><img src="https://img.shields.io/badge/GITHUB-111827?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
<a href="https://ansh-pratap-developer.ai.studio"><img src="https://img.shields.io/badge/PORTFOLIO-2563EB?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"/></a>
<a href="mailto:shakyaansh9756@gmail.com"><img src="https://img.shields.io/badge/EMAIL-DC2626?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>



PYTHON • MACHINE LEARNING • GENERATIVE AI • BACKEND ENGINEERING

I build and test AI-powered applications, with a focus on reliable APIs, responsible LLM integration, and practical machine-learning systems.
</div>01 / THE BUILDER
<table>
<tr>
<td width="58%" valign="top">Hi, I'm Ansh.
I'm a final-year B.Tech Computer Science & Engineering student at Mewar University, graduating in 2027.

I enjoy turning ideas into working software — especially products that combine Python, machine learning, APIs, and generative AI.

My recent work focuses on making AI features more dependable: validating model output, handling failures, protecting sensitive workflows, and writing tests for edge cases.

Currently focused on
- Applied AI / Machine Learning
- Generative AI and LLM-powered applications
- Python backend development
- Building, testing, and deploying useful products
</td>
<td width="42%" align="center" valign="middle"><img src="https://github-readme-stats.vercel.app/api?username=AnshPratap2314&show_icons=true&hide_border=true&bg_color=0B1224&title_color=38BDF8&text_color=E5E7EB&icon_color=60A5FA" width="100%" alt="GitHub statistics"/></td>
</tr>
</table>02 / WHAT I BUILD
<table>
<tr>
<td width="33%" valign="top"><img src="https://img.shields.io/badge/01-2563EB?style=flat-square" alt="01"/> AI APPLICATIONS
LLM-powered tools with structured outputs, validation, fallback paths, and clear boundaries around automated decisions.
</td>
<td width="33%" valign="top"><img src="https://img.shields.io/badge/02-7C3AED?style=flat-square" alt="02"/> MACHINE LEARNING
Python workflows for text classification, computer vision, data preparation, model evaluation, and experimentation.
</td>
<td width="33%" valign="top"><img src="https://img.shields.io/badge/03-DC2626?style=flat-square" alt="03"/> BACKEND SYSTEMS
REST APIs, authentication, persistence, input validation, testing, and deployment-focused engineering.
</td>
</tr>
</table>03 / FEATURED BUILDS
01 — MindCare AI
Safety-oriented mental health support chatbot

<a href="https://mindcare-ai-o1e5.onrender.com"><img src="https://img.shields.io/badge/OPEN_LIVE_DEMO-2563EB?style=for-the-badge" alt="Live demo"/></a>
<a href="https://github.com/AnshPratap2314/AI-Mental-health-chatbot"><img src="https://img.shields.io/badge/VIEW_SOURCE-111827?style=for-the-badge&logo=github&logoColor=white" alt="Source code"/></a>

Python FastAPI scikit-learn TF-IDF Logistic Regression Docker Render
Designed around a simple principle: safety decisions should not depend on an LLM behaving perfectly.

- Deterministic safety routing: a rule-based behavior/risk engine is authoritative. High-risk messages are routed to deterministic safety responses; the trained response model's risk output is not used to make safety decisions.
- Trained response model: TF-IDF + Logistic Regression trained on a 50,000-message synthetic dataset across 20 intents in English and Hinglish.
- Evaluation workflow: train/validation/test splits, duplicate and leakage audits, and hard-negative/challenge-case scripts.
- Backend hardening: session management, CORS validation, an authenticated audit endpoint, and 200+ pytest tests covering safety, sessions, and API security.
<details>
<summary><b>System flow</b></summary>```mermaid
flowchart TD
    A[User message] --> B[Input validation]
    B --> C[Deterministic risk analysis]
    C --> D{High risk?}
    D -- Yes --> E[Deterministic safety response]
    D -- No --> F{LLM available?}
    F -- Yes --> G[Generate response]
    F -- No --> H[Trained response model]
    G -- Invalid / error --> H
    H --> I[Validated fallback response]
```
</details><sub>Uses synthetic, non-clinical data. It is not clinically validated and is not a medical or diagnostic tool.</sub>
02 — AI Interview Simulator
AI-assisted interview practice and evaluation platform

<a href="https://ai-based-interview-simulator-1.onrender.com/"><img src="https://img.shields.io/badge/OPEN_LIVE_DEMO-2563EB?style=for-the-badge" alt="Live demo"/></a>
<a href="https://github.com/AnshPratap2314/ai-based-interview-simulator"><img src="https://img.shields.io/badge/VIEW_SOURCE-111827?style=for-the-badge&logo=github&logoColor=white" alt="Source code"/></a>

Python FastAPI Pydantic SQLite Gemini API JavaScript
- Structured answer evaluation: Gemini evaluates candidate answers against a Pydantic schema; deterministic checks flag very short, off-topic, language-mismatched, or inconsistent evaluations for review.
- Persistent state: SQLite-backed interview sessions and candidate history, separate candidate/session credentials with expiry, and rate limiting with Retry-After.
- Adaptive interviews: question difficulty adjusts using a rolling average of recent scores. Curated questions cover Technical, HR, and AI/ML tracks across three difficulty levels.
- JD and résumé analysis: extracts requirements and helps create a personalized interview question plan.
- Testing: 76 pytest tests, including a fake Gemini client so tests can run without an API key.
<details>
<summary><b>Architecture</b></summary>```mermaid
flowchart TD
    A[Browser UI] --> B[FastAPI]
    B --> C[Authentication, expiry, rate limiting]
    C --> D[Interview engine]
    C --> E[Gemini evaluation]
    D --> F[(SQLite)]
    E --> G[Pydantic validation]
    G --> H[Review flags]
    H --> F
```
</details>03 — StudyVerse AI
Collaborative AI learning workspace · Team project

<a href="https://study-verse-ai-eight.vercel.app/"><img src="https://img.shields.io/badge/OPEN_LIVE_DEMO-2563EB?style=for-the-badge" alt="Live demo"/></a>
<a href="https://github.com/AnshPratap2314/StudyVerse-AI"><img src="https://img.shields.io/badge/VIEW_SOURCE-111827?style=for-the-badge&logo=github&logoColor=white" alt="Source code"/></a>

Node.js Express MongoDB JavaScript Gemini OpenAI Groq
- Multi-provider AI gateway integrating Gemini, OpenAI, and Groq.
- Role-based agent workflow with router, researcher, teacher, critic, and synthesizer roles.
- Document Q&A / RAG workflow for asking questions over uploaded study material.
- JWT authentication, hashed passwords, Mongoose models, and per-user data isolation.
- Backend test files cover security regression, data isolation, and API contracts.
<sub>Team project. See the repository for the current implementation and contribution details.</sub>
04 — Aishie
Voice-controlled desktop assistant · macOS prototype

<a href="https://github.com/AnshPratap2314/Aishie-AI-Assistant"><img src="https://img.shields.io/badge/VIEW_SOURCE-111827?style=for-the-badge&logo=github&logoColor=white" alt="Source code"/></a>

Python SpeechRecognition OpenCV face_recognition PyAutoGUI AppleScript
- Face-recognition gate using face embeddings and distance thresholds.
- Installed-app monitoring with watchdog, a change log, and voice-command lookup.
- JSON-based memory and macOS messaging automation through AppleScript.
- Wake-word detection and fuzzy command matching help handle imperfect speech transcripts.
<sub>Prototype features require internet access for selected services and macOS for automation.</sub>
04 / THE TOOLKIT
<div align="center">LANGUAGES
<img src="https://skillicons.dev/icons?i=python,cpp,c,java,js,html,css,mysql&theme=dark" alt="Python, C++, C, Java, JavaScript, HTML, CSS, MySQL"/>AI / DATA / BACKEND
<img src="https://skillicons.dev/icons?i=opencv,sklearn,tensorflow,fastapi,nodejs,express,mongodb,sqlite&theme=dark" alt="OpenCV, scikit-learn, TensorFlow, FastAPI, Node.js, Express, MongoDB, SQLite"/>TOOLS & PLATFORMS
<img src="https://skillicons.dev/icons?i=git,github,docker,postman,vscode,pycharm,linux,aws&theme=dark" alt="Git, GitHub, Docker, Postman, VS Code, PyCharm, Linux, AWS"/></div>Area	Skills
Programming	Python, JavaScript, C, C++, SQL
AI / ML	scikit-learn, TF-IDF, Logistic Regression, NLP, OpenCV, NumPy, Pandas, Keras
Generative AI	Gemini API, prompt engineering, structured-output validation, OpenAI API integration
Backend	FastAPI, REST APIs, Pydantic, authentication, rate limiting, input validation
Databases	SQLite, MySQL; MongoDB exposure through StudyVerse AI
Testing & delivery	Pytest, Git/GitHub, Docker basics, Render, Vercel
Web	HTML, CSS, JavaScript


05 / EXPERIENCE & LEARNING
<table>
<tr>
<td width="50%" valign="top">AI Intern
Internship Studio (iStudio)
Oct 2025 – Jan 2026
- Automated recurring data-preprocessing steps with Python.
- Refined LLM prompt templates for structured outputs.
- Used exploratory data analysis to inspect label noise and class imbalance.
</td>
<td width="50%" valign="top">AI & ML Industrial Trainee
CTTC Bhubaneswar
Apr – May 2025
- Built a face detection and recognition attendance system using OpenCV, SVM, and LBPH on a self-collected dataset.
- Benchmarked SVM, KNN, Decision Tree, and Neural Network classifiers on the same data.
</td>
</tr>
</table>Education
B.Tech — Computer Science & Engineering
Mewar University · 2023–2027 (expected) · CGPA: 7.8/10
Certifications & Programs
- Google AI Essentials
- Google Prompting Essentials
- IBM SkillsBuild — AI Fundamentals
- HP LIFE — Data Science & Analytics
- NVIDIA 6G Developer Program — Selected participant
06 / GITHUB SIGNAL
<div align="center"><img height="170" src="https://github-readme-stats.vercel.app/api?username=AnshPratap2314&show_icons=true&hide_border=true&bg_color=0B1224&title_color=38BDF8&text_color=E5E7EB&icon_color=60A5FA" alt="GitHub stats"/><img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=AnshPratap2314&layout=compact&hide_border=true&bg_color=0B1224&title_color=38BDF8&text_color=E5E7EB" alt="Most used languages"/><img width="95%" src="https://github-readme-streak-stats.herokuapp.com/?user=AnshPratap2314&hide_border=true&background=0B1224&ring=38BDF8&fire=F97316&currStreakLabel=38BDF8&sideLabels=E5E7EB&dates=94A3B8" alt="GitHub contribution streak"/></div><sub>GitHub language charts describe repository contents; they are not a measure of overall proficiency. Stats are served by third-party services and may occasionally be unavailable.</sub>
07 / LET'S CONNECT
<div align="center">HAVE AN IDEA? LET'S BUILD IT.
Open to AI/ML internships, Generative AI opportunities, Python/backend roles, collaborations, and learning from builders.

<a href="https://ansh-pratap-developer.ai.studio"><img src="https://img.shields.io/badge/PORTFOLIO-2563EB?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"/></a>
<a href="https://linkedin.com/in/ansh-pratap-68156625b"><img src="https://img.shields.io/badge/LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="mailto:shakyaansh9756@gmail.com"><img src="https://img.shields.io/badge/EMAIL-DC2626?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>



CURIOUS BY DEFAULT. BUILDING WITH INTENT.
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:063B75,100:050816&height=75&section=footer" width="100%" alt=""/></div>
