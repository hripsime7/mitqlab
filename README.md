# MitqLab — Armenian Data Science Course

> **"Տվյալագիտություն հիմունքներից մինչև Machine Learning"**  
> A complete, free, offline-capable Data Science course in Armenian — built for high school students in Armenia, powered by Gemma 4.

🔗 **Live demo:** https://hripsime7.github.io/mitqlab/

---

## What is MitqLab?

MitqLab is a fully interactive, browser-based Data Science course taught entirely in Armenian (Հայերեն). It was built to make data science education accessible to Armenian-speaking students who have no access to quality materials in their native language.

The course runs in a single HTML file — no installation, no server, no dependencies. A student opens the link and starts learning immediately.

---

## The Problem It Solves

Data science education is almost entirely in English. For students in Armenia — especially outside Yerevan — this is a real barrier. MitqLab removes that barrier by delivering a full curriculum in Armenian, with an AI tutor that answers questions in Armenian, powered by Gemma 4.

---

## Features

### 📚 5 Complete Learning Modules (2 hours total)
| Module | Topics |
|--------|--------|
| Մ1 · Mathematics & Statistics | Mean, Median, Mode, Outliers, Correlation |
| Մ2 · Pandas | DataFrames, filtering, cleaning, dropna, fillna |
| Մ3 · Machine Learning | Linear Regression, Decision Tree, KNN |
| Մ4 · Data Visualization | Matplotlib — line, bar, pie, scatter charts |
| Մ5 · Real-world Applications | Medicine, finance, sports, engineering |

### 🤖 AI Tutor powered by Gemma 4
- Answers student questions **in Armenian** in real time
- Context-aware: knows which module the student is on
- **Two modes:**
  - **Ollama (offline)** — runs Gemma 4 locally, works without internet
  - **Google AI (cloud)** — uses Gemini API with model fallback chain
- Thinking-token cleanup so Gemma's internal reasoning never leaks to students
- Quick-prompt buttons: Explain · Hint · Code · Practice

### 💻 In-Browser Python Execution
- Powered by **Pyodide** — runs real Python in the browser
- Students write and run NumPy, Pandas, Matplotlib code with one click
- Matplotlib plots render inline as images
- No installation needed

### 🎓 Quiz & Certificate
- 15-question final exam covering all 5 modules
- 80% passing threshold (12/15)
- Personalized downloadable PNG certificate on completion
- Progress bar tracks completion across modules

---

## How Gemma 4 Is Used

Gemma 4 (`gemma-4-31b-it` via Google AI Studio, or `gemma4:e4b` via Ollama) serves as the AI tutor. The integration includes:

- **System prompt** scoped to the student's active module and topic list
- **Few-shot anchoring** with a sample Armenian Q&A to lock response format
- **`thinkingConfig: MINIMAL`** to suppress reasoning overhead on cloud mode
- **Empty thought block injection** (`<|channel>thought<channel|>`) per Gemma 4 docs to stabilize no-thinking behavior
- **Regex-based thought tag stripping** to catch any leaked `<think>`, `<thought>`, or `<|think|>` tokens before they reach the student
- **Model fallback chain:** if `gemma-4-31b-it` fails, tries `gemma-4-26b-a4b-it` → `gemma-3-27b-it` → `gemini-2.0-flash-lite` → `gemini-1.5-flash-8b`

---

## Running Locally with Ollama (Offline Mode)

1. Download and install Ollama from [ollama.com](https://ollama.com)
2. Pull the model:
   ```
   ollama pull gemma4:e4b
   ```
3. Start Ollama with CORS enabled:
   - **Mac / Linux:** `OLLAMA_ORIGINS=* ollama serve`
   - **Windows (PowerShell):** `$env:OLLAMA_ORIGINS="*"; ollama serve`
4. Open the site and enter your IP address (`127.0.0.1` if running locally)
5. To stop: press `Ctrl + C` in the terminal

> The model is 5.3 GB. Responses may take 10–60 seconds depending on hardware.

---

## Tech Stack

| Technology | Purpose |
|-----------|---------|
| Vanilla HTML/CSS/JS | Single-file app, zero build step |
| Pyodide | In-browser Python runtime |
| Gemma 4 (Ollama) | Offline AI tutor |
| Gemini API | Cloud AI tutor with fallback |
| Matplotlib via Pyodide | In-browser chart rendering |
| GitHub Pages | Instant deployment |

---

## Social Impact

- **Language:** Entire course and AI tutor operate in Armenian
- **Free:** No cost to students or schools
- **Offline-capable:** Works without internet via Ollama — important for schools with limited connectivity
- **No installation:** Opens in any browser, on any device
- **Completeness:** Covers statistics → Pandas → ML → visualization → real applications in one session
ood Hackathon](https://www.kaggle.com/competitions/gemma-4-good-hackathon)** on Kaggle.  
The hackathon required using Gemma — this project runs Gemma 4 locally via Ollama as its primary AI tutor. The Google AI option is an optional fallback for users who cannot run Ollama locally.
