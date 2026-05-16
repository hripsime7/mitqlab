# MitqLab · Տվյալագիտություն

> An interactive, Armenian-language Data Science education platform — delivered entirely as a single HTML file, no installation required.

---

## Overview

MitqLab is a self-contained web application that teaches Data Science from the ground up, in Armenian. It combines structured lesson modules, a live Python sandbox, an AI tutor, an AI-generated personalised learning roadmap, a graded final exam, and a downloadable certificate — all in one file.

---

## Features

### 5 Structured Learning Modules

Each module contains explanations, worked examples, interactive questions, runnable code snippets, and a set of practice tasks with checkboxes. Progress through the modules is tracked by a top progress bar.

| Module | Topic | Duration |
|--------|-------|----------|
| Մ1 | Mathematics & Statistics — Mean, Median, Mode, Outliers, Correlation | 20 min |
| Մ2 | Data & Pandas — DataFrame, filtering, data cleaning, NaN handling | 25 min |
| Մ3 | Machine Learning — Linear Regression, Decision Tree, KNN | 30 min |
| Մ4 | Data Visualisation — Matplotlib: Line, Bar, Pie, Scatter charts | 20 min |
| Մ5 | Real-world Applications — Medicine, Finance, Engineering, Sport | 20 min |

Completing each module unlocks the next and advances the overall progress bar. A **Final Project & Summary** module (★) wraps everything up with a mini end-to-end project (hours vs. score analysis).

---

### In-Browser Python Sandbox (Laboratory)

A full Python runtime powered by **Pyodide** (v0.26.4) runs directly in the browser — no server, no installation.

- Write and execute Python 3 code in a code editor with syntax-coloured output
- Pre-loaded packages: `numpy`, `matplotlib`, `pandas`
- Matplotlib charts render inline as images inside the output panel
- **"Ask AI" button** — sends your current code and its output directly to the AI tutor for analysis or debugging
- Clear button to reset the editor

---

### Dual-Panel Laboratory Layout

The laboratory splits the screen into two panels side by side:

**Left panel — Python Sandbox** (described above)

**Right panel — AI Tutor Chat**, with:
- A fixed input bar that stays pinned at the bottom regardless of conversation length
- Quick-prompt buttons: Math test, Code test, Hint, Explain
- Image attachment support for multimodal questions (attach a screenshot or diagram)
- A **Chat** tab and a **Learning Path** tab (see below)
- Choice of AI backend: Ollama (local/private) or Gemma 4 Cloud (Google AI Studio)

---

### AI Tutor

A context-aware AI assistant embedded in both the main page (floating widget) and the laboratory panel.

- Powered by **Gemma 4** — choose between local Ollama models (gemma4:e4b · e2b · 26b · 31b) or Google AI Studio cloud (gemma-4-31b-it · gemma-4-26b MoE)
- Responds in **Armenian or English** — switchable at any time
- Always aware of the currently active module so answers stay on-topic
- Quick-action buttons: Explain · Hint · Code example · Practice exercise
- Multimodal: attach images to your question
- Full streaming responses rendered in real time
- Learning path tracker tab shows concepts covered during the conversation

---

### AI-Powered Personalised Learning Roadmap

Inside the Laboratory's "Ուսուցման Ուղի" (Learning Path) tab, the AI Wizard generates a fully personalised study plan.

Fill in:
- **Topic** — Python, Mathematics, Data Science, or Machine Learning
- **Current level** — Zero, Beginner, Intermediate, or Advanced
- **Goal** — Fundamentals, Competition/Olympiad, ML project, or Job
- **Timeframe** — a slider from 1 to 180 days
- **Age** (optional)
- **Learning needs** (optional) — Dyslexia, ADHD, Visual impairment, Hearing impairment, Motivation issues

The AI generates a structured, day-by-day roadmap table tailored to all inputs. The result can be:
- **Downloaded as CSV** for use in any spreadsheet app
- **Downloaded as PNG** for sharing or printing

---

### Final Quiz

A 15-question multiple-choice exam covering all 5 modules.

- Pass threshold: **80%** (12/15 correct)
- Each question shows instant feedback with a plain-language explanation
- Correct and incorrect options are colour-coded after submission
- Passing the quiz automatically unlocks the Certificate page

---

### Downloadable Certificate

On passing the quiz, a personalised certificate is generated on an HTML5 Canvas and offered for download as a **PNG image**.

- Enter your name to personalise it
- Displays your score (e.g. 14/15 · 93%)
- Styled with the MitqLab branding, decorative border, and the MitqLab logo

---

### Progress Tracking

- Module completion is tracked per-session and reflected in a top progress bar
- Completed modules are visually marked in the navigation
- Practice task cards can be toggled as done/undone and state is remembered
- Learning path conversation history persists across tab switches within a session
- API keys, Ollama IP, preferred model, and language preference are saved to `localStorage` and restored automatically on the next visit

---

## Tech Stack

| Layer | Technology |
|-------|------------|
| Runtime | Vanilla HTML · CSS · JavaScript (single file) |
| Python engine | [Pyodide](https://pyodide.org) v0.26.4 |
| Python packages | NumPy · Matplotlib · Pandas |
| AI (local) | [Ollama](https://ollama.com) — Gemma 4 family |
| AI (cloud) | Google AI Studio — Gemma 4 31B / 26B MoE |
| Fonts | Playfair Display · Source Code Pro · Libre Baskerville (Google Fonts) |
| Analytics | Google Analytics (GA4) |

---

## Getting Started

No build step, no dependencies to install.

1. Download or clone the repository.
2. Open `index.html` in any modern browser.
3. Python loads automatically in the background (requires internet for the Pyodide CDN on first load).
4. To enable the AI tutor, either:
   - **Ollama (local/private):** Install [Ollama](https://ollama.com/download), run `ollama run gemma4:e4b`, then enter your IP address (`127.0.0.1` for local) in the tutor settings.
   - **Gemma 4 Cloud:** Get a free API key from [aistudio.google.com/apikey](https://aistudio.google.com/apikey) and paste it into the tutor settings.

---

## Language

The platform is fully in **Armenian (Հայերեն)** with full support for English in AI tutor conversations. The AI tutor language can be toggled between 🇦🇲 Armenian and 🇬🇧 English at any time from the tutor settings panel.

---

## Project Structure

```
index.html          ← Entire application (styles, markup, and scripts)
README.md           ← This file
```

---

## Credits

Built by Hripsime 2026
