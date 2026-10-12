<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&pause=1200&color=58A6FF&center=true&vCenter=true&width=760&lines=Hi%2C+I'm+Ansh+Pratap;AI%2FML-Focused+Software+Developer;Python+%7C+FastAPI+%7C+Generative+AI" alt="Typing SVG" />
</div>

<div align="center">

Final-year B.Tech CSE student · Mewar University · Expected 2027 · Rajasthan, India

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/ansh-pratap-68156625b)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:shakyaansh9756@gmail.com)

</div>

---

## About

I build Python/FastAPI backends that combine machine learning and LLM features with the engineering around them: validated APIs, persistent sessions, authentication, rate limiting, and automated tests. My recent work is a safety-first mental health chatbot and a Gemini-powered interview platform, both deployed on Render.

**Looking for:** AI/ML Engineer, Generative AI / LLM application, Python Developer, and Backend Developer internships and fresher roles.

---

## Skills

- **Languages:** Python, JavaScript, C, C++, SQL
- **Backend & APIs:** FastAPI, REST, Pydantic, session/token auth, rate limiting, input validation
- **AI/ML:** scikit-learn, TF-IDF, Logistic Regression, NLP, text classification, OpenCV, face_recognition, NumPy, Pandas, Keras
- **Generative AI:** Google Gemini API, structured LLM output validation, prompt engineering, OpenAI API (optional integration)
- **Data & Frontend:** SQLite, HTML/CSS, vanilla JavaScript
- **Testing & Tools:** Pytest, Git/GitHub, Docker (basic), Render
- **Exposure:** Node.js, Express, MongoDB (team project), RAG (fundamentals)

---

## Featured Projects

### MindCare AI: Safety-Oriented Mental Health Support Chatbot
[Live demo](https://mindcare-ai-o1e5.onrender.com) · [Source](https://github.com/AnshPratap2314/AI-Mental-health-chatbot)

`Python` `FastAPI` `scikit-learn` `Docker` `Render`

- **Safety-first routing:** a rule-based behavior/risk engine is authoritative. High-risk messages never reach the LLM, and the trained model's risk output is never used for safety decisions.
- **Trained response model:** TF-IDF + Logistic Regression on a 50,000-message synthetic dataset (20 intents, English + Hinglish) predicting intent, mood, topic and risk, with a deterministic fallback when the optional LLM is off or fails.
- **Evaluation hygiene:** train/validation/test splits with duplicate and leakage audits, plus separate hard-negative and challenge-case evaluation scripts.
- **Hardening:** session management, CORS validation, an authenticated audit endpoint, and 200+ pytest tests covering safety, sessions and API security.

*Synthetic data only. Not clinically validated, and not a medical or diagnostic tool.*

### AI Interview Simulator
[Live demo](https://ai-based-interview-simulator-1.onrender.com/) · [Source](https://github.com/AnshPratap2314/ai-based-interview-simulator)

`Python` `FastAPI` `Pydantic` `SQLite` `Gemini API` `JavaScript` `Render`

- **Structured evaluation:** Gemini scores answers against a Pydantic schema, with provider retry and validation errors surfaced as proper API responses. Deterministic checks flag answers for human review (very short, off-topic, language mismatch, inconsistent scores).
- **Persistent state:** SQLite-backed interview state, candidate history and summaries, separate candidate and session credentials with expiry, rate limiting with `Retry-After`, and idempotent evaluation requests.
- **Adaptive difficulty:** the next question's difficulty moves up or down based on a rolling average of recent scores.
- **JD / résumé intelligence:** extracts requirements from a job description and a résumé, matches them, and builds a personalized question plan.
- **Tests:** 76 pytest tests, using a fake Gemini client so no API key is needed.

### Aishie: Voice-Controlled Desktop Assistant (macOS prototype)
[Source](https://github.com/AnshPratap2314/Aishie-AI-Assistant)

`Python` `SpeechRecognition` `pyttsx3` `OpenCV` `face_recognition` `PyAutoGUI` `AppleScript`

- Wake-word detection with fuzzy matching, spoken responses, and fuzzy-matched command routing.
- Face-recognition gate using face embeddings and distance thresholds before the assistant starts.
- Installed-app monitoring with `watchdog` (change log plus a voice command to query it), JSON-based memory, and messaging via AppleScript.
- Uses Google's speech recognition API and Wikipedia, so it needs an internet connection.

---

## Experience & Training

**AI Intern, Internship Studio (iStudio)** · Oct 2025 – Jan 2026
- Automated recurring data-preprocessing steps in a training pipeline with Python.
- Redesigned LLM prompt templates to enforce a structured output schema.
- Used EDA to identify label noise and class imbalance ahead of deployment.

**AI & ML Industrial Trainee, CTTC Bhubaneswar** · Apr – May 2025
- Built a face detection and recognition attendance system (OpenCV, SVM, LBPH) on a self-collected dataset.
- Benchmarked SVM, KNN, Decision Tree and Neural Network classifiers on identical data.

---

## Education & Certifications

**B.Tech, Computer Science & Engineering**, Mewar University (2023 – 2027, expected)

Google AI Essentials · Google Prompting Essentials · IBM SkillsBuild: AI Fundamentals · HP LIFE: Data Science & Analytics

---

## GitHub Activity

<div align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=AnshPratap2314&show_icons=true&theme=github_dark&hide_border=true" alt="GitHub stats" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=AnshPratap2314&layout=compact&theme=github_dark&hide_border=true" alt="Top languages" />
  <br/>
  <img src="https://streak-stats.demolab.com?user=AnshPratap2314&theme=github-dark-blue&hide_border=true" alt="Contribution streak" />
</div>

---

<div align="center">

[GitHub](https://github.com/AnshPratap2314) · [LinkedIn](https://linkedin.com/in/ansh-pratap-68156625b) · [shakyaansh9756@gmail.com](mailto:shakyaansh9756@gmail.com)

</div>
